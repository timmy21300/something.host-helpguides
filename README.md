# How to install Windows Server 2019 on a Something.Host VPS.

This is not an offical something.host help guide, use this at your own risk

### Note: This will not work Simple 2GB VPS.
### Note: This will erase all data on your VPS, ensure you have a backup of your data.

1. Purchase a [Something.Host Cloud VPS](https://www.zentool.xyz/hosting).
2. On the VPS Panel press F12 to Open Developer Tools
![Image](http://zentool.xyz/images/chrome_13NAG0x0Hk.png)
3. In the `Console` type `deployImage('windows-server-2019')` and press enter as shown above.

4. Press `confirm`
![Image](http://zentool.xyz/images/chrome_6izC7bqXLO.png)
5. You will be given a new password, ensure you take not of this. You will need it to login using RDP.
6. The install of Windows Server will comince, it can take sometime to install. You will notice the Power State and Installed OS will display `updating`, once the install is complete, this will change to Power State `running` and Installed OS `undefined` 
![Image](http://zentool.xyz/images/chrome_mbsqwNzwMd.png)
7. Once the install is complete, open Windows Remote Desktop. 
  The computer will be your VPS IP address e.g. `123.456.12.1`
  The username will be `Administrator`
  The password will be the password given from the something.host control panel.
