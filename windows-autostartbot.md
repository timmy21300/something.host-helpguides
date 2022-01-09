# How to automatically start your Bot on VPS start up (Windows)

1. Create a `start.bat` file in your bot folder. This file should contain below, replace `index.js` if your bot has ai different file. (Using this will alsowe restart your bot if is unexpectedly goes 'offline'.
```bat
@echo off
echo Starting...
:main
node index.js
echo Restarting Bot...
goto main
```

1. Open `Task Scheduler` in Administrator mode
![Open Task Scheduler](http://zentool.xyz/images/mstsc_Hdd6wS8owO.png)

2. Select `Create Task` on the right panel.

3. Select a name for your task and select `Run whether user is logged on or not` (With out selecting this option the bot will not start) Then select `triggers` and create a new trigger.

![Set Task Name](http://zentool.xyz/images/mstsc_urX1yZQ6gh.png)

4. Ensure the trigger `Begin the task` is set to `At startup` then press `OK`

5. Then click actions and create a new action. The action will need to be set to `Start a program`. The Program/Script should be your bot directory + `\start.bat` e.g. `C:\MyBot\start.bat`. The `Start in` field should be populated with your bot directory only e.g. `C:\MyBot\`.
![Edit Action](http://zentool.xyz/images/mstsc_phsVXlP4tz.png)

6. Select `Ok` and then `Ok` again. You will be prompted for your password, type this in. 
![Enter Password](http://zentool.xyz/images/mstsc_bMPPgpNgTL.png)

7. Your task is now setup. You can restart your VPS and the bot will start automatically. (You will not be able to see the CMD window when using this method)
