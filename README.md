Downpatching
=============
1. [steam://open/console](steam://open/console)
2. Run the command for your platform below.
3. Steam will download the content to a folder in Steam\steamapps\content\app_535480\depot_xxxx (the output of the command will tell you where)
- yadda,yadda, remember to back up anything important

| build   | os      | command                                          | notes         |
| ---     | --      | -----                                            | ---           |
| 3424016 | Windows | download_depot 535480 535481 1209251613183946467 | moon jump first discovered in this patch     |
| 3424016 | OSX     | download_depot 535480 535482 1888243660282583313 | moon jump first discovered in this patch     |
| 3424016 | Linux   | download_depot 535480 535483 4121286783973719701 | moon jump first discovered in this patch     |
| 3481968 | Windows | download_depot 535480 535481 5093099090628805935 | current patch |
| 3481968 | OSX     | download_depot 535480 535482 4361402942138657640 | current patch |
| 3481968 | Linux   | download_depot 535480 535483 1619880232980530908 | current patch |

Method shamelessly stolen from https://speedsouls.com/darksouls2:Downpatching

Quad Input
==========
This method will allow you to try out the game with 4 characters using one controller. I found the results pretty disappointing, but the data's here so others can test.

This is loosely based on this [Parsec KB article](https://support.parsecgaming.com/hc/en-us/articles/360012652092-Playing-Games-With-Two-Keyboards-Emulating-A-Controller-With-A-Keyboard) that explains how to map a secondary keyboard as a controller.

- Install [Parsec](https://parsecgaming.com/), click 'Yes' to install controller support. Alternatively, could probably just install drivers from https://github.com/nefarius/ViGEm but I didn't want to mess with figuring out which specific drivers to use at the time.
- Set up a mappings in UCR https://github.com/Snoothy/UCR that maps inputs from controller 1 to controller 2,3,4. There will need to be a mapping for each button on the controller to the same button on each controller, as well as the axes for L2/R2. I have included my [context.xml](./context.xml) from my UCR folder in the hopes someone can just reuse my mappings (still needs to be tested)
- Activate the profile for your mappings in UCR. Steam should see all 4 controllers connected.
- Launch Sundered, go to "Multiplayer" in the options, ensure all 4 characters are set to a controller.
- Start a new game or load a save, the other characters should spawn as soon as input is detected on one of the other controllers.
- In one instance I had to restart Steam completely to get it working
- FWIW, I am using a Dualshock 4, so you may have to change the input controller in the config if you are using something else.
