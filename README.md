# Lenovo Ideapad 330 15ARR fixes for Linux

Touchpad will work after updating kernel to 5.X + 
Update your kernel using UKUU
```
sudo add-apt-repository ppa:teejee2008/ppa
sudo apt-get install ukuu
```
## To Fix wifi
clone this repo and cd to "rtl8821ce"
I've already made a simple script, so just run it  
```
. run.sh
```
P.S. install GCC if you got an error related to compiler

WiFi should start working after the process

I don't know about other distros, i tried on Ubuntu 18.04

## References
[https://gist.github.com/debojyoti/228729498628e898497557db57619a28](https://gist.github.com/debojyoti/228729498628e898497557db57619a28)
[2](https://github.com/MSF-Jarvis/ideapad-330-linux)
[3](https://github.com/tomaspinho/rtl8821ce)
