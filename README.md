TF2 Scripts
====================
## important info
It is probably a good idea to turn on auto reload.

The class cfg scripts are executed after binds.cfg.  So binds in the class cfg will take precedence over the ones in binds.cfg

I like hiding certain viewmodels while seeing other view models. Generally I like hiding hitscan viewmodels, but keeping projectile/melee weapon view models.

---
## autoexec.cfg
Use this only if you have fast internet and very low ping (> 50ms).  This makes character models more closely align with hitboxes.

---
## binds.cfg
The bulk of my personal binds.  

- `+zoom` alias is written but not bound. It decreases FOV to "zoom" in.  Stabbystabby uses this to aim with Ambassador occasionally.  You may bind this if you wish.
- `+pyro` alias lets you switch to pyro with loadout3.  Ideally you have a homewrecker equipped on loadout3, so if you spawn and the teleporter is sapped, you can remove it as quickly as possible.
- `q`, `e`, and `r` are mapped to voice commands so you can troll your team/enemies.
- `t` is taunt, since I accidentally press `g` when trying to press `b` for `lastdisguise`.  `g` is bound to spray.
- `SHIFT` is crouch, since I used to play on mac.
- `-` toggles console since I accidentally press `~` when trying to press `1` for `slot1`.
- `]` explodes.  Deny demo heads, and explode when you do high fives.

---
## engineer.cfg
I never play engineer.  In fact, I should delete this script since it only helps engineers be more annoying.

- `p` toggles "battle engi mode," which is for Gunslinger, and lets you build mini's even faster.
  - in "battle engi mode" `MOUSE2` will destroy your sentry (if any) and bring up the blueprint to build a new sentry simultaneously.
- `MOUSE3` is a Sentry Jump script.  You'll probably need to practice using this if you want to use it in a real game.  You can sentry jump using the rockets of a level 3 sentry and the wrangler.

---
## medic.cfg
I used to play some competitive medic, but now I'm just a casual.

- `q` will initiate a random voice command.  You'll want to do this when you're about to get full charge, so you don't announce "I am fully charged!" to everyone (even the enemy).  
- `fake` alias is written, but not bound.  This will initiate the voice command to say "I am fully charged!" to fool the enemy into thinking you have full charge before you actually do.  I'm just a casual so these fancy tactics really don't matter shit.
- `r` invokes medic radar.  Holding `r` will lower the autocall for medic threshold to 0 health... so basically all your teammates will display a plus icon over their head so you can see them, even through walls.  Good when you get separated from your team.

I was working on a script for vaccinator such that `q`, `e`, and `r` would directly map to a resistance, instead of you needing to cycle with just `e`.  You would then be able to select a resistance without accidentally cycling over it.  I gave up... for now.

---
## pyro.cfg
Pretty simple.

- `MOUSE3` spins you super fast so you can flame in circles.  Hilarious pre-game, but actually very ineffective at spychecking.  Please don't use it in combat.

---
## spy.cfg
I have about 1000 hours on spy.

- `MOUSE3` quickly disguises you to sniper.  In pubs sniper is best disguise, becaues all pub snipers are retarded. So the enemy doesn't actually expect you to be doing anything.
- `MOUSEWHEELUP` and `MOUSEWHEELDOWN` triggers `lastdisguise` and changes weapons.
  - So, if you scroll the mouse, the enemy will see you change weapons as your disguised class.  You can see verification of the weapon you're holding on the bottom left.

---
## all classes cfg
The above were class specific scripts.  All classes have the following scripts.

- Crosshair style is changed based on class and on slot.  
- Viewmodels are hidden when you fire for the first time depending on class and slot.  Generally projectile weapons are shown, and hitscan are hidden.  Consider changing these to your own preferences.

Consider:

`alias equip1 "slot1; r_drawviewmodel 1; bind MOUSE1 +hide; cl_crosshair_file default"`

This displays the default crosshair, and hides the weapon when you shoot with slot1`.  You may change `+hide` to `+show`, or `default` to `crosshair3`.  Or whatever you prefer.

- Change Spawn script.  This literally saves my life a few times per game.  It is currently bound to `HOME` (a button on my mouse).  This script will change your class to medic.  If you use this in spawn, you will change class immediately.  So if a crit rocket is flying at you, you can teleport out of the way by changing class.  If you use the script again, you will switch back to your original class.  The switch back is a bit buggy, so you may need to manually switch classes.  If you are medic, it will switch your loadout, but will function the same.  You need to have different equipment sets for this to work.  (perhaps change your hat).

- For medic, ideally your first two loadouts use the same medigun, and your last two loadouts use the same medigun.  So you could have quick-fix, quick-fix on A and B.  Then kritz and kritz on C and D.  When you use Change Spawn script, your ubercharge will be preserved.  You may press `o` to switch between which set (A/B or C/D) you are using.
