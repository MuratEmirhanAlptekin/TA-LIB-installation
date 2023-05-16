this repo explains how to install TA-LIB on linux based systems  
for linux:  
requirments:  
you need to have python3-dev and make to run ta-lib on your system
for RedHat based distros:
```
sudo dnf install python3-devel
sudo dnf group install "C Development Tools and Libraries" "Development Tools"
```
for Debian based distros:
```
sudo apt-get install python3-dev
sudo apt-get install build-essential
```
first you have to install ta-lib itself 
```
wget http://prdownloads.sourceforge.net/ta-lib/ta-lib-0.4.0-src.tar.gz
tar -xvf ta-lib-0.4.0-src.tar.gz
cd ta-lib
```
and then build it
```
./configure --prefix=/usr
make
sudo make install
```
and then if you want to use Python wrapper
```
pip install ta-lib
```
if you encounter any problems feel free to ask 
