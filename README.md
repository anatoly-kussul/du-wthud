# WtHUD

PvP/PvE HUD for Dual Universe

hold left shift (with remote control active) to see controls helper.

![HUD concept](/images/1.png?raw=true)

# installation
gunner manual links:
- weapons
- radar
- databank
- ammo cont

remote controller manual links:
- space fuel tank (only one)
- same databank as in gunner seat


# soundpack installation

unarchive sound archive into `~\Documents\NQ\DualUniverse\audio`


# lua chat commands

{} - required param, [] - optional param
```
sh{size} - hide {size} targets from radar widget
ss{size} - show {size} targets on radar widget
(not sure if size filtering still works)
f[XXX] - show only XXX target on radar widget. (supports any number of targets with any separator, f alone clears filter)
addAll - add all visible targets to friendlist
clearAll - clear saved friendlist
addID {XXXXXX} - add ID friendlist (needs full ID, not last 3 digits)
info {pos} - A lot of useful info about coords
```

AR:
```
addar {pos} {name} [#rgb]
clearar [name]  -  clears all custom marks if no param specified
cleardead [xxx]  -  clears all dead marks if no param specified
```


# periscope scipt installation

place 2 programming boards and a manual switch.
Make a link from PB1 to switch and from switch to PB2.
install `periscope-autofix.json` in PB1, install `programming-board-2.json` in PB2.
Then you need to manually start the PB1 every time you are flying your ship to have a periscope.
