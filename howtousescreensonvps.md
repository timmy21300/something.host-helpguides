# How to use Screens on a Something.Host VPS.

This guide is designed to show you how to use screens on a VPS to keep the bot online, for this example we will use Terminus.

This is not an offical Something.Host guide.

Ensure you have already uploaded your Files to your VPS. You can use [Filezilla](https://filezilla-project.org/) to do this, a usefull guide can be [found here](https://support.something.host/en/article/transferring-files-from-and-to-your-vps-filezilla-1qa8arz/)

Login Details:
Username: root
Password: Obvious...
Post: 22

### Creating a Screen!

1. Connect to your VPS using Terminus or similar platform. 

2. In your VPS console type `apt-get install screen` and press return. This will install the ability to attach and detach from screens. 

![Run this in the console](http://zentool.xyz/images/Termius_z4szqfTBVO.png)

3. We now need to create a "screen", in this example we will call it 'test'. Run `screen -s name` to create your screen. Replace name with something more suited to your session e.g. `testbot`. Hit return after!

![Run this too!](http://zentool.xyz/images/Termius_lSBZ217bsg.png)

4. From this screen you can start your bot as normal.

![Started Bot](http://zentool.xyz/images/Termius_ULzWHW2dDL.png)

5. Once your bot has started, we can detach from the screen. Your bot will continue to run. To do this press `Ctrl + A + D`, a message will appear telling you the detach was successful.

![Success](http://zentool.xyz/images/Termius_BCseHXyj3T.png)

6. You can close Terminus and your bot will continue to run. 

### Attaching to an existing screen!

1. In your VPS console type `screen -x name`, replace `name` with the name you set your screen as. In this example it was `testbot`. 

![Your Bot!](http://zentool.xyz/images/Termius_3LKdeLYvQ2.png)

2. That's it, you can stop and restart your bot as normal.

