# Linux-on-Android

## How To Install Linux on Android

***This subject will discuss how to install Linux on android.***

#  requirements

-  basic knowledge of Linux command line.
-  an android with version 7 up to...
-  install termux app.
-  install andronix app.
-  install VNC for Gui ( optional ) but I prefer to install it.

Download apps


1.  Termux app [Download Termux](https://play.google.com/store/apps/details?id=com.termux&hl=ar&gl=US)
2.  Andronix app [Download Andronix](https://play.google.com/store/apps/details?id=studio.com.techriz.andronix&hl=ar&gl=US)
3.  VNC app [Download VNC](https://play.google.com/store/apps/details?id=com.realvnc.viewer.android&hl=ar&gl=US)
 
# Steps

after installing all apps

- Step One update & upgrade termux >` apt upgrade -y & apt update -y` ( each command is alone not in the same line )

- Step Two open your andronix and choose your preferred type of Linux dist ( choose to install ) will copy the download link as a command )

- Step Three open termux app and pass the command and press Enter. will download the dist. during installation will ask you about your language and password.

- Step Four after the installation is done. you need to open your dist but how!? write `ls` command to display the files where you are. go to download directory cd download display the files in this directory ls in my android i have installed ubuntu . in your case, you will find your dist ended with `.sh`. how to execute this file!? with bash command For Example `bash start-ubuntu.sh` will open Linux dist as cli . you can write Linux commands and do what you would like to do such as you have Linux.

- Step Five Now we have Linux as a command-line interface. but we want to open it as Gui. do not be impress! we will get Linux as Gui with VNC open VNC app. Press the + sign. you will be asked for IP Adress:Port and the name of your computer. IP Adress will be the loopback address `127.0.0.1:1` The port will be 1 the name Write any name you like after you answer you will be asked too for password of this dist . remember the password that you have entered during the installation.

The installation is successfully Done.

# Note

no one has spoken about the issue after a while of installation. issues such as connection error about the port do not worry It is simple this issue because of vnc server need to be reopening . But how!? open your dist as cli `bash start-ubuntu.sh` Write `vncserver-stop` will kill vnc process and write `vncserver-start` will start vnc process. That's it Go to vnc and try again will open.

Another issue with the password was forgotten. Go to your dist as cli and write `vncpasswd` you will be asked to Assign new password .

I hope This article be useful for you.
