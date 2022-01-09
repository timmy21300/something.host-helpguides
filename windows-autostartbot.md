# How to automatically start your Bot on VPS start up (Windows)

This is not an offical something.host guide.

1. Create a `start.bat` file in your bot folder. This file should contain the following
```bat
@echo off
echo Starting...
:main
node bot.js
echo Restarting Bot...
goto main
```

1. Open `Task Scheduler` in Administrator mode
![Open Task Scheduler](http://zentool.xyz/images/mstsc_Hdd6wS8owO.png)

2. Select `Create Task` on the right panel.

3. Select a name for your task and select `Run whether user is logged on or not` (With out selecting this option the bot will not start) Then select `triggers` and create a new trigger.
![Set Task Name](http://zentool.xyz/images/mstsc_urX1yZQ6gh.png)

4. Ensure the trigger `Begin the task` is set to `At startup` then press `OK`

5. Then click actions and create a new action. The action will need to be set to `Start a program`. The Program/Script should be `C:\Windows\System32\cmd.exe`. 
