Title: Chinese-HU-with-buttons-YT9216B-1-16-or-8227L-Upgrade-firmware

Because of one week searching like idiot on internet, mostly on Russian sites i can now read Cyrilic and speak something (Nazdrovje!!!) i found a way how to update Chinese crap HU to little bit decent software with ROOT, TWRP, and better radio app with RDS. Thanks to 4PDA forum and users!

If you have HU (head unit) with phisical buttons and USB socket on front then this tutorial is for you because you have similar crap like i have.

--- picture 1----

What was symptoms of not working flash procedure?
USB flash with XYAUTOUPG folder - hell yeah haha (no go)
flash with SP_Flash_Tool - are you insane? (no go)
trying boot with pressed buttons - why will you do that?
connecting to PC - not even bing bing sound like when you connect something
when you reset HU connected to PC you get USB not recognized popup and in device manager no id or description for device
other nasty stuff...
Conclusion:
Because rear 4 pin port is connected to front USB socket, something interfer connection and cannot be flashed ordinary way. Not even with 6 pin port on back.

Solution:
Dissasembly rear plate and disconnect ribbon cable from front USB socket to motherboard and flash in ordinary way

Prerequisites:
1.) Screwdriver
2.) HU with phisical buttons on front and USB socket, model 8227L or YT9216B with 1GB ram and 16GB rom. Mine has come with YT9216B_00002_V_004_20190826 version, Android 8.1 Go (chinese scam because it isn't 8.1) and MCU 3.1
3.) You need to make male-male USB cable (or buy it). You can take two old cables, cut booth and solder or tangle wires together. Take care of color matching (Black-black, White-white etc.)
4.) Download zip from 4pda (direct link to gdrive): YT9218_00002_V004_20190912 (UI1) ROOT , TRPW from user Maxkir (tnx dude)
5.) Download SP_Flash_Tool_v5.1924_Win
6.) Download SP_Driver_v2.0
7.) Windows 10 x64 PC
8.) PSU (12v, 1A is enough)
9.) Knife (sharp if you have)


OK lets go!
1.) First reboot PC to driver signature disable mode. Go to start, click shift + windows key on keyboard, and click power - restart. Go to troubleshoot - advanced options - startup settings - restart. When PC reboots hit F7 button

2.) Then extract SP_Driver_v2.0 from zip and install driverinstall.exe with admin rights (right click - run as administrator). You need few times click allow when installing drivers (or something in box with x)

3.) Extract YT9218_00002_V004_20190912

4.) Extract SP_Flash_Tool_v5.1924_Win and run like administrator. In Download Agent field link MTK_AllInOne_DA.bin and in Scatter-loading file link MT3367_Android_scatter.txt from extracted YT9218_00002_V004_20190912. Deselect preloader if is selected!!!!!

5.) Take apart your HU. Unscrew 4 screws on back plate. Then you will see one ribbon cable (flat cable) that goes from LCD site where is USB socket to motherboard. On motherboard disconnect this cable.

--- Picture 2 ----
6.) If you have 4 pin USB cable then connect this cable in back of HU in 4 pin port. If you have only 6 pin cable then try to modify connector on cable and cut away two empty "pins" and connect cable to 4 pin HU port

-- Picture 3 -----
7.) In SP_Flash_Tool_v5.1924_Win hit Download button

8.) Connect male-male USB cable with cable in step 6 and power on HU with ACC and B+ wire connected to plus terminal on PSU and black wire to negative terminal.

9.) Voila. Your PC start flashing stupid HU. Wait few minutes till SP_Flash_Tool_v5.1924_Win show new popup with flash successfull image. Disconnect cables and reboot HU with disconnecting PSU. Reconnect power and wait till HU load all stuff and boot to loader.

--- Picture 4 ----
10.) Change language from Russian to whatever you want.
--- Picture 5 ----
11.) Go to Car Settings - Factory Settings (PIN: 8888) - Color Setting and scroll to bottom and change slider AVDD to 2. With this you will eliminate screen flickering.
--- Picture 6 ----
12.) Go to Play Store, login, and update all apps.
--- Picture 7 ----
