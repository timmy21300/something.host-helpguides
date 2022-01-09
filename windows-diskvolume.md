# How to change a disk volume on a Windows VPS.

This is not an offical something.host guide.

1. Connect to your VPS using RDP. 
2. Search for `Computer Management` in the start menu, run it as Administrator.
![Open Computer Management](http://zentool.xyz/images/mstsc_jw71kBLNGd.png)

3. Open the `Disk Management` window. This is displayed in the left tree menu (as below). If you have any unallocated storage, it will show on the right (as highlighted in the red box)
![Open Disk Management](http://zentool.xyz/images/mstsc_2Z0tNhUxhO.png)

4. Select the volume you want to extend and right click, then click the `extend volume` option then `next`. (If this is greyed out, ensure you opened Computer Managment in Administrator Mode)

![Extend Volume](http://zentool.xyz/images/mstsc_KO9VQKTHij.png)

5. You will now need to select muw much disk space you want to add. By default, it will have the max storage you can extend it by, once you have selected the desired about press next.

![Select Volume to Extend by](http://zentool.xyz/images/mstsc_NdiRaczt4d.png)

6. Select `Next` and `Finish` to extend the volume.
