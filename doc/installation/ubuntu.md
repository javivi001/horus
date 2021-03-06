# Horus installation in Ubuntu ![][ubuntu-logo]

[return to Home](../../README.md)

Add our ppa for OpenCV and Horus

```bash
sudo add-apt-repository ppa:bqopensource/opencv
sudo add-apt-repository ppa:bqopensource/horus
```

Update your system

```bash
sudo apt-get update
```

Install Horus

```bash
sudo apt-get install horus
```

If user has no access to serial port, execute:

```bash
sudo usermod -a -G dialout $USER
```

Reboot the computer to apply the changes

```bash
sudo reboot
```

### Update Horus

If there is a new release just execute:

```bash
sudo apt-get upgrade
```

<br>

NOTE: our packages are hosted in launchpad.net

* [PPA OpenCV](https://launchpad.net/~bqopensource/+archive/ubuntu/opencv/)
* [PPA Horus](https://launchpad.net/~bqopensource/+archive/ubuntu/horus/)
* [PPA Horus-dev](https://launchpad.net/~bqopensource/+archive/ubuntu/horus-dev/)

[ubuntu-logo]: ../images/ubuntu.png