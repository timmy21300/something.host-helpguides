# How to use Screens on a Something.Host VPS.

This guide is designed to show you how to use screens on a VPS to keep the bot online, for this example we will use Terminus.

This is not an offical Something.Host guide.

Ensure you have already uploaded your Files to your VPS. You can use [Filezilla](https://filezilla-project.org/) to do this, a usefull guide can be [found here](https://support.something.host/en/article/transferring-files-from-and-to-your-vps-filezilla-1qa8arz/)

Login Details:
Username: root
Password: Obvious...


1. Connect to your VPS using Terminus or similar platform. 
2. In your VPS console type `apt-get install screen` and press return. This will install the ability to attach and detach from screens. 
![Run this in the console](http://zentool.xyz/images/Termius_z4szqfTBVO.png)
3. We now need to create a "screen", in this example we will call it 'test'. Run `screen -s test` to create your screen. 
![Run this too!](http://zentool.xyz/images/Termius_CdgCHIUFeT.png)
4. From this screen you can start your bot as normal. 
