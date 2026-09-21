This repository contains corrected game logic files for game [Mortyr 2093-1944](https://en.wikipedia.org/wiki/Mortyr).

These fixes are based on the English version of the game.
They work in the Polish version too, but English weapon and pick-up names are used instead of Polish ones.


#### Changes

Mostly minor improvements are done without significantly altering game logic or changing balance.
The non-comprehensive list of changes is:

* Icons for keys on future maps are fixed (golden, silver and blue keycards are used).
* Some missing entity sounds are added.
* Tower decorations (used on some future maps) don't disappear anymore when playing on some skill levels.
* State transitions for some entities are fixed.
* Bounding boxes of enemies are corrected to better match their visual size.
* Bounding boxes of decorations are corrected to better match their visual size.
* Bounding boxes of pick-ups are corrected so that they are no longer partially submerged into the ground.
* Shot start positions for enemies are corrected so that projectiles start flying roughly from the muzzle position of their weapon.
* Shot start positions for player's weapons are corrected so that projectiles start flying roughly from the muzzle position.
* Some visual effects (like lights) are slightly corrected.

What has not be and will not be changed:

* Game difficulty should remain the same, so, changes affecting it should be avoided.
* Although the game has many unused sounds in its resources intended to be used for some enemies, they can't be used, because the game's engine has some hard limit on the total number of sound files and/or their total size.
* A lot of engine-related issues can't be changed by providing another game logic files.


#### Installation

Just copy all files having *STD* extension from this repository into the *Data* directory (where *main.hal* file is located).
The game will use them instead of the same files stored within *main.hal* file.


#### Known issues

Changing game logic files may lead to desynchronization of prerecorded demos.
So, don't wonder if demos playing on game startup behave differently with these game logic fixes applied.

Old save files may or may not be compatible with these fixes.
So, it's recommended to avoid loading old saves and only to start a new game instead.
