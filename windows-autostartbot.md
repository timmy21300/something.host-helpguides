# How to automatically start your Bot on VPS start up (Windows)

This is not an offical something.host guide.

1. In your bot directory create a `start.bat` file. The contents of this file should beas below, replace `main.js` with your bots main file. Using this file will also restart your bot is it unexpectedly shuts down.
```
@echo off
echo Starting...
:main
node main.js
echo Restarting Bot...
goto main
```

2. Open `Task Scheduler` in Administrator mode
![Open Task Scheduler](http://zentool.xyz/images/mstsc_Hdd6wS8owO.png)

3. Select `Create Task` on the right panel.

4. Select a name for your task and select `Run whether user is logged on or not` (With out selecting this option the bot will not start)
![Set Task Name](http://zentool.xyz/images/mstsc_urX1yZQ6gh.png)
