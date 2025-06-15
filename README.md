# Fidelity-Active-Trader-Pro-linux-ubuntu
intall Fidelity Active Trader Pro in Ubuntu Debian Linux


here are the steps::  some steps may be Redundant. but these steps got ATP working.

my system - linux mint 22.1

download the 64bit setup file of ATP classic.

1.) install wine

```
sudo dpkg --add-architecture i386sudo dpkg --add-architecture i386

sudo wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/noble/winehq-noble.sources

sudo apt update

sudo apt install --install-recommends winehq-stable wine64 winetricks
```

2.) launch winetricks  -> select default wine -> install windows components

> I IGNORED the following error - You are using a 64-bit WINEPREFIX. Note that many verbs only install 32-bit versions of packages. If you encounter problems, please retest in a clean 32-bit WINEPREFIX before reporting a bug.

3.) install dotnet 4.6.2 and visual c++ 2015-2022.

4.) this will take a few steps of clicking through installers

5.) then exit winetricks. open terminal and cd to directory of setup file. type `wine setup.exe`and hit enter.

6.) installation took about 15min and then after it shows installed, I had to press ctrl+c to end the terminal output.

7.) there will be an icon on the desktop for Fidelity. Enjoy!!
