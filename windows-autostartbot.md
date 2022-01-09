# How to automatically start your Bot on VPS start up

This is not an offical something.host guide.

1. In your bot directory create a `start.bat` file. The contents of this file should be:
```@echo off
echo Starting...
:main
node main.js
echo Restarting Bot...
goto main```
