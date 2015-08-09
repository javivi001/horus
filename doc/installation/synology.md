# Horus installation in Synology DSM ![][synology-logo]

[return to Home](../../README.md)

Firts of all, you need a Synology Nas updated, with ssh access with root credentials. [Guide](http://forum.synology.com/wiki/index.php/Enabling_the_Command_Line_Interface)

Then, you have to Install [Debian Chroot](https://synocommunity.com/package/debian-chroot) addming the Synocomunity repo. As they says:

Step 1:- Log into your NAS as administrator and go to Main Menu → Package Center → Settings and set Trust Level to Synology Inc. and trusted publishers.

Step 2:- In the Package Sources tab, click Add, type SynoCommunity as Name and http://packages.synocommunity.com/ as Location and then press OK to validate.

Step 3:- Go back to the Package Center and enjoy SynoCommunity's packages in the Community tab.


At these point, we have two methods to install:


### The easy one (Automatic)

Open a ssh connection with your synology Nas and follow these instrucctions

```bash
ssh root@<yournas>.local -p XXXX

... wait ...

/var/packages/debian-chroot/scripts/start-stop-status chroot

... Now we are in the console of Debian Chroot ...

cd
wget https://github.com/javivi001/horus/blob/develop/syno-horus.sh
bash syno-horus.sh

... Make coffe and take patience, but everything will work with only a pair of cuestions at beginig ...
```

### The manual one


TODO


[synology-logo]: ../images/synology.png
