TF2 Scripts
====================
### Important info
It is probably a good idea to turn on auto reload.
the class cfg scripts are executed after binds.cfg.  So binds in the class cfg will take precedence over the ones in binds.cfg

I like hiding certain viewmodels while seeing other view models. Generally I like hiding hitscan viewmodels, but keeping projectile/melee weapon view models.

I use shift to crouch, and - to open console. I hate opening console when trying to switch to slot1.

### autoexec.cfg
Just has some network configs... its generally good if you have low ping and fast internet. Don't use this file if you have high ping/slow internet, otherwise the game will by choppy.

### binds.cfg
The bulk of my personal binds.  I have zoom alias written, but it is not bound to anything. You may bind it if you are interested - it reduces the FOV to make it zoom in.  Stabbystabby uses it to aim with ambassador occasionally.  The idea of Pyro Switch is to switch to pyro with loadout #3. So if a spy saps a teleporter entrance as you spawn, you can switch to pyro with loadout #3, which you ideally have a homewrecker on.

q, e, and r are mapped to voice commands so you can troll your team/enemies.

Taunt is "t" because I keep accidentally pressing "g" when I mean to press "b" for lastdisguise as spy.  G is bound to spray.

### engineer.cfg
I never play engineer.  Though I wrote this script I don't remember exactly what it does.  Pressing "p" toggles "battle engi mode" which is essentially for Gunslinger.  I believe it lets you destroy your sentry and bring up the blueprint to build a new sentry with one button (right mouse).  There is also a Sentry Jump script to help you rocket jump with a level 3 sentry.

### medic.cfg
Pressing "q" will initiate a random voice command; you want to do this when you're just about to get full charge, so the medic doesn't announce to everyone (even the enemy) "I am fully charged!"  I have comment out binding "fake" to e, because it conflicts with vaccinator resistance switching with e.  In any case, fake announces "I am fully charged" so the enemy team falsely believes you have uber.  I'm just a casual so these fancy tactics really dont matter shit.  

Medic radar is bound to "r".  Holding "r" will lower the auto-call for medic threshold to 0 health... so basically all your teammates will have + icons display over their heads so you can see them through walls.  Good when you get separated from your team.

I was working on a script for vaccinator such that q, e, and r would directly map to a resistance, instead of you needing to cycle with just e.  You would then be able to select a resistance without accidentally cycling over it.  I gave up.

### pyro.cfg
MOUSE3 spins you super fast so you can flame in circles.  Hilarious pre-game, but actually very ineffective at spychecking.  Please don't use it in combat.

### spy.cfg
MOUSE3 quickly disguises you to sniper.  In pubs sniper is best disguise, becaues all pub snipers are retarded. So the enemy doesn't actually expect you to be doing anything.

Scrolling the mouse basically spams "lastdisguise" command and changes weapons.  So, if you scroll the mouse, the enemy will see you change weapons as your disguised class.  You can see verification of the weapon you're holding on the bottom left.

### all classes.cfg
The above were class specific scripts.  All classes have the following scripts.

Crosshair style is changed based on class and on slot.  Viewmodels are hidden when you fire for the first time depending on class and slot.  Generally projectile weapons are shown, and hitscan are hidden.  Consider changing these to your own preferences. Consider:

alias equip1 "slot1; r_drawviewmodel 1; bind MOUSE1 +hide; cl_crosshair_file default"

This displays the default crosshair, and hides the weapon when you shoot with slot1.  You may change +hide to +show, or default to crosshair3.  Or whatever you prefer.

Change Spawn script.  This literally saves my life a few times per game.  It is currently bound to "HOME" (a button on my mouse).  You may change this to anything you want... preferrably a button on your mouse for easy access.  This script will change your class to medic.  If you use this in spawn, you will change class immediately.  So if a crit rocket is flying at you, you can teleport out of the way by changing class.  If you use the script again, you will switch back to your original class.  The switch back is a bit buggy, so you may need to manually switch classes.  If you are medic, it will switch your loadout, but will function the same.  You need to have different equipment sets for this to work.  (perhaps change your hat).

For medic, ideally your first two loadouts use the same medigun, and your last two loadouts use the same medigun.  So you could have quick-fix, quick-fix on A and B.  Then kritz and kritz on C and D.  When you use Change Spawn script, your ubercharge will be preserved.  You may press "o" to switch between which set (A/B or C/D) you are using.
