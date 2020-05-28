Dark Souls 3 PvP Watchdog
=======================

## About

This is a port of the original Dark Souls PvP Watchdog made by /u/eur0pa with additions made by myself (/u/TheSpicyChef) and /u/LukeYui. The aim is to bring something to Dark Souls 3 that will mitigate 90% of what cheaters can do. For the remaining 10%, it will back up your save game every time a session is made so that your progress is protected.

## What it does

This tool identifies cheaters and attempts to mitigate the damage which they can do through multiple methods.

 * It will detect stat and soul level anomalies of other players, allowing your to remove the offender.
 * It will prevent items being forced into your inventory by other players
 * It will detect players that auto-revive upon being killed
 * It will prevent dangerous effects such as curse from being applied to you during PvP.
 * It will mitigate and patch a wide range of exploits including multiple crashes.
 * It will block people dropping and giving you gestures or impossible weapons which you can't drop if picked up.
 * It will attempt to mitigate framerate drops caused by bullets.
 * It will play a sound when invading or getting invaded, useful if the game is out of focus.
 * It will let you reconnect to the game server after being sent to the main menu for FPS issues without needing to restart the game.
 * If enabled, it can autokick detected cheaters when hosting.
 * If enabled, it can backup saves every time a new session is established and store a set amount of backups before deleting the oldest.
 * It will detect known cheaters using alt accounts and flag them preemptively.

## Can this softban

The only instance this will softban is if you have used version 1.02 or version 1.03. These versions had a hook for the auto revive detection that was detected by the anticheat. From 1.04 we removed the offending hook however if you have used either of those versions, you will have been flagged. This was due to a section of the anticheat not being bypassed which was unfortunately missed until the update had been pushed to the public repo. Going forward from this we have gone back to assess the anticheat further and are awaiting ban waves before releasing updates. If you have been banned, get in contact with namco as if its your first ban, you can be unbanned after a period of time.


## How to use it

 1. Get the package from the download page
 
 2. Extract everything into your Dark Souls III folder, generally "C:\Program Files (x86)\Steam\steamapps\common\DARK SOULS III\Game"
 
 3. Edit DS3PWSettings.ini to your likings - lines starting with ; describe what each setting does
 
 4. Play Dark Souls III unfettered by cheaters. Or at least, much less than before.


#### Example in-game overlay output

    (cheater, red color)
     !1 player1 (player1steam) [F1] to kick    [F5] to ignore   SL [Real 110-115]
     ^^ ^		^              ^               ^                ^ anomaly detected and details (if available)
     || |       |              +---------------+ commands (if available)
     || |       | 
     || |       + player steam name (if available) 
     || + player name
     |+ player id
     + cheating detected

    (ignored player or player that's being blocked and is currently leaving the session, green color)
     @2 player2 
     ^ ignored / whitelisted / leaving

    (common player, white)
     #3 player3 
     ^ no anomalies detected

## known issues

Post any bugs or issues to the issue tracker: [here](https://github.com/Jellybaby34/Dark-Souls-3-PvP-Watchdog/issues)
If Watchdog doesn't protect you from something, post it to the issue tracker.

## appendix

### keyboard shorctuts reference

[**F1**] ..... banish all detected cheaters

[**F5**] ..... ignore all detected cheaters

[**F9**] ..... toggle the in-game overlay

[**F10**] .... show the about window

[**F11**] .... Allow ignored cheaters to be kicked again

### changelog and latest fixes

** see CHANGELOG.txt **

### package contents

d3d11.dll ...................... the Dark Souls 3 PvP Watchdog DLL

DS3PWSettings.ini .............. the options file

changelog.txt .................. change history for the tool

readme.txt ..................... the text document you're currently looking at

WatchdogData ................... A data file used to store information used by watchdog

### resources

Original Dark Souls Watchdog: https://bitbucket.org/infausto/dark-souls-pvp-watchdog/

### thanks to

[Eur0pa](http://reddit.com/u/eur0pa) for the original code i've ported to Dark Souls III. Thank him for the original concept and tool. [Buy him a beer or something](https://paypal.me/eur0pa).

[LukeYui](http://reddit.com/u/LukeYui) for many of the fixes to the more obscure and malicious exploits and for getting me to continue working on this.
