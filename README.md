# marioWorldSelect
A patch for the original Super Mario Brothers for the NES which enables world select from the start screen.

## Legal
Due to copyright law I cannot upload the original Mario Bros source code. I instead have created an .IPS patch file that can be applied to your personally owned ROM image of Super Mario Bros. IPS or "International Patching System", is a file format specifically for patching ROM and disk image files. I reccomend using LIPS to apply the patch:
http://fusoya.eludevisibility.org/lips/index.html

## How it works
On the title screen press the B button. This will change the world number in the top right corner and you will start the game on the first level of that world.

## The nitty gritty
There is a flag called WorldSelectEnableFlag that gets set once a second playthrough of the game is completed. I moved this flag to the beggining of the GameMenuRoutine so that it is automatically enabled when the game is started thus allowing the secret world select feature from the get-go. 

Reverse engineering NES games has been a fun way for me to start to learn assembly. If I find anything else interesting as I dig around in the source code I will provide future updates. 
