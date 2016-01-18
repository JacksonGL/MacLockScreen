# MacLockScreen
Macbook lock screen without disconnecting Wi-Fi

Introduction
----------------------
A Simple tool that locks screen without disconnecting the Wi-Fi on Macbook.

For earlier version of Mac the following command works (more details about this solution, can be found [here](http://apple.stackexchange.com/questions/71884/wi-fi-disconnects-when-i-lock-the-mac)):
```
cd /System/Library/PrivateFrameworks/Apple80211.framework/Versions/Current/Resources
sudo ./airport en1 prefs DisconnectOnLogout=NO
```
The above solution sometimes does not work on new version of Macbook. The alternative is this tool if you are bothered by reconnecting Wi-Fi every time after locking the screen.


Requirements
----------------------
This small tool is only useful on Macbook.


Install MacLockScreen
----------------------
Use the following command to install This software:
```
chmod 755 ls.sh
sudo cp ls.sh /opt/local/bin
```

Use MacLockScreen
-----------------
To lock the screen of your Mac without disconnecting the Wi-Fi, type the following command in terminal:
```
ls.sh
```