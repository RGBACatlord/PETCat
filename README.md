![PCatSmall](https://github.com/RGBACatlord/PETCat/assets/37526906/bc898245-afd5-439d-88b1-4a545938287a)

# PETCat
This is a custom build of TF2 based off Team Comtress, tailored to creation of Team Fortress 2 unusual effects.
All changes are in the Particle Editor only.

# New Features
Some of these features are unique to PCAT while others are simply ported from new engine branches.
Features are as follows:

* AutoView
  * When enabled, the particle preview window will zoom and position the view based off the particle system's bounding box.
* Lock Preview
  * When on, the particle preview will stay viewing the selected system, so you can work on children and see how it affects the parent.
* Toggles in both preview windows
  * Render Axes (Helpful for workshop images/videos)
  * Render Control Points (Renders axes at all CPs)
  * Render Grid
* Keyboard Shortcuts
  * Definition Browser
    * 1: New System
    * 2: Copy Selected System
  * Particle Preview
    * 1: Toggle Axes
    * 2: Toggle AutoView
    * 3: Toggle Grid
    * 4: Toggle CP Axes
    * 5: Restart the preview
  * These can be disabled by tool window or globally with
```cpet_disable_keybinds_(all/modelpreview/systembrowser/particlepreview)```
* Console
  * Adds a new console window
* Particle Definition Browser
  * Added Copy and Replace
    * Will duplicate selected systems and replace every occurence of a word with another
    * Child Highlighting: Children of the selected definition will be highlighted
* Properties
  * Booleans show as true or false now (Disable with cpet_properties_bool_as_text 0), and takes 'true' and 'false' as valid values.
  * Custom properties window colors can be set through the CoolerPET menu button
  * Added Keybinds
    * 1: Add new function
    * A: Move selected function up
    * D: Move selected function down
* Model Preview
  * Adds an entirely new tool window to PET: see how the effect looks on a player in-editor
  * Includes a slider for effect Z offset
  * Switch preview class, animation and team
  * Includes a toggle to add an Unusual Cap to the player model
  * ```cpet_mdl_test_offset_(x/y/z)``` int (default 0): Particle system offset
  * ```cpet_mdl_realign_on_change``` 0/1 (default 1): Reset camera on class/anim change

# Installation

Download the latest release, extract it, and run the auto install batch file.
Specify your TF2's install location, and specify where you want PETCat to go.
It will make a copy of TF2 but with PETCat modifications, and place an easy access shortcut on your desktop.

Your particle editor's layout might be slightly screwed on first launch - fix it with View->Default Layout

# FAQ

**Will this trigger VAC?**

*You can't actually join servers with this as it's an old build of the game, and so there's no reason to run secure.
I highly suggest against running secure as this is a modified client.*

**Can you add X feature / fix X bug?**

*Probably. Go ahead and start an issue and I'll take a look.*

**Is Valve ok with this?**

*I asked Valve directly and I'm still waiting for a reply, so I can only assume they don't care!*

# Planned Features

* Changeable preview background images
* More model preview hats
* Toggle for live grid previews in definition browser
* Replace children by substring (i.e. swap ueffect_blah_red with ueffect_blah_blue)
* Add new animations to model preview
* More handy shortcuts and macros
* ~~pitch to valve for official inclusion~~
