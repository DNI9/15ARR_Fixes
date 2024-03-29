# Lenovo Ideapad 330 15ARR fixes for Linux

> Update for 2021: Everything seems to be working out of the box now (remember to update distro packages post installation) , for ubuntu base distros, go to drivers (usually in software) and select rtl8821ce and apply and then reboot.
> or go here and follow https://github.com/tomaspinho/rtl8821ce

Touchpad will work after updating kernel to 5.X + 

Update your kernel using UKUU
```
sudo add-apt-repository ppa:teejee2008/ppa
sudo apt-get install ukuu
```
## To Fix wifi (Old)
clone this repo and cd to "rtl8821ce"
I've already made a simple script, so just run it  
```
. run.sh
```
## Note 
install GCC if you encounter an error related to compiler

WiFi should start working after the process

## Black Screen Fix: 
If you face only black screen after starting installation, try setting "nomodeset" (without quotes) in the grub menu by pressing e
like this:
```
quiet splash nomodeset
```
hit ctrl + x or F10 to continue installling, after finishing  installation, update kernel to the stable , 5.x+ recommended and then update distro packages, distro should run fine now.

## References
[https://gist.github.com/debojyoti/228729498628e898497557db57619a28](https://gist.github.com/debojyoti/228729498628e898497557db57619a28)

[https://github.com/MSF-Jarvis/ideapad-330-linux](https://github.com/MSF-Jarvis/ideapad-330-linux)

[https://github.com/tomaspinho/rtl8821ce](https://github.com/tomaspinho/rtl8821ce)
