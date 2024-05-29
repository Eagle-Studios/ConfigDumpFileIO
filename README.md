# ConfigDumpFileIO
An extension used to dump the All in One Config more efficiently in Arma 3

## How To Use
**Steps were taken from the Bohemia.net Forum Post, and properly placed here for ease of access**
_https://forums.bohemia.net/forums/topic/191737-updated-all-in-one-config-dumps/?tab=comments#comment-3175049_

- Download the release from https://github.com/Eagle-Studios/ConfigDumpFileIO/releases/tag/1.1.1
- Move the dumpconfig.sqf and ConfigDumpFileIO_x64.dll to Arma 3 root directory (Which is where the Arma.exe is stored)
- Load the ARMA 3 Launcher and be sure to select the Parameters --> Enable File-Patching and Disable Battle eye.
- Launch ARMA 3 with ONLY mods you want to dump
  - Adding unnessacry mods will mean there is more config to export AND more things for you to look through.
  - Run Arma, On the Main Menu, select Editor, VR, then immediatly play the scenario (Enter is the shortcut!)
  - Press Escape to bring up the Options Menu and most importantly the debug console.
    - On the debug console, in the execute section, paste the following:
    ``` [configFile] call compile preprocessFileLineNumbers "dumpConfig.sqf" ```
  - Now click the LOCAL EXE button
  - Wait until Arma finishes processing.
    - Arma may freeze once or several times. Doing anything to "stop" this as it'll create a game crash. Let it do its thing, until its no longer freezing etc.
    - Once the process has been completed, and you can quit the game. 
  - You should find the dumped file in your ARMA 3 root directory (Where the .Sqf/.Dll you pasted earilier are, aka where the Arma.exe is stored.)
    - If there is no such file, then it didnt work. Go back and try again, it's possible you missed something or quit too early.
