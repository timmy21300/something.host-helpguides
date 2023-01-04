# How to host your Discord Bot Maker (DBM) Bot on a Something.Host App Box

![Something.Host](https://zentool.xyz/images/somethinghostbanner.png)

This is not an offical something.host help guide, use this at your own risk

### 1. Purchase a Something.Host App Box service ([Click Here](https://something.host/en/products/discord-bot-hosting))

### 2. Head over to your services console, you will need to setup the programming language, which for DBM is node.js. Select Node 16.6, leave Setup command blank (we will change this later) ![SetupYourSomethingService](http://timmyis.gay/images/chrome_nAhSBcSGkq.png)

### 3. You can now go to 'Remote Access', this will give you all the details to be able to SFTP to your service and upload your files. Do not share your password with anyone! ![RemoteAccessTab](http://timmyis.gay/images/chrome_mq2tmXNFbj.png)

### 4. Using your SFTP login details connect to your service using a SFTP client. In this example we will be using Filezila, this is free to [download here](https://filezilla-project.org/download.php?type=client). Once downloaded, open Filezila and enter the login details provided on the something.host control panel. Example below; 

Host: 'sftp://' & Host IP Address on SomethingHost CP
Username: Username on SomethingHost CP
Password: Password on SomethingHost CP
Port: Usually 23 (however check on the SomethingHost CP)

![FilezilaConnectToService](http://timmyis.gay/images/filezilla_HAtSFwygDd.png)

### 2. Create your DBM Bot and navigate to your bot directory
![DBM-Image1](http://timmyis.gay/images/Discord_Bot_Maker_SOGQGC5t2c.png)
