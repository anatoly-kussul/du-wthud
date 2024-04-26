# WtHUD

PvP/PvE HUD for Dual Universe

BETA 0.7

can also use be used as a flying sctipt for you haulers.
Highly inspired by simplicity of Albatross hud, has very similar features, like fire-and-forget burn limiter (both in atmo and approaching from space), etc.

![HUD concept](/images/2.png?raw=true)

![HUD concept](/images/3.png?raw=true)

hold left shift (with remote control active) to see controls helper.

# v0.6

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

for xs ships link all of the above


# soundpack installation

unarchive sound archive into `~\Documents\NQ\DualUniverse\audio`

# lua params
```
showARCompass: enable AR compass on script startup
holdBrakeOnInit: hold brakes on script startup
autoRes: enable auto resistances on script startup
autoResMode:
   0 - Set max resists to highest incoming damage type
   1 - Set 50/50 resists to two highest incoming damage type (Deafult)
   2 - Set resists in ratio of incoming damage by all types
autoResMinHitCount: wait N hits before applying auto resists (default 0)
maxAngularSpeed: set hard limit on your rotational velocity in rads. (default 0 - no limit)
```

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
helper - toggle build helper
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
