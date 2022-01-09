# How to automatically start your Bot on VPS start up

This is not an offical something.host guide.

1. In your bot directory create a `start.bat` file. The contents of this file should beas below, replace `main.js` with your bots main file. Using this file will also restart your bot is it unexpectedly shuts down.
```@echo off
echo Starting...
:main
node main.js
echo Restarting Bot...
goto main```


2. Open `Event Scheduler` in Administrator mode
