# Python script to change MAC address of Linux machine

_Becoming anonymous in a network and to avoid some network attacks where changing MAC Address becomes useful_

Need of changing MAC Address:

* To bypass MAC Address filtering
* To bypass certain kind of MITM spoofing attack
* To avoid device tracking in a public network

### Automation using Python

_Since it is not possible for us to manually change the MAC Address every time, we can automate the process of changing the MAC Address using Python. This script will keep changing the MAC Address in a constant period of time._

### Usage
```
git clone 
```

___

### Manual Changing MAC Address in Linux Machine
```
sudo apt-get update
sudo apt-get install ifconfig
```
After installing this package, we can change the MAC Address using:
```
sudo ifconfig <interface-name> down
sudo ifconfig <interface-name> hw ether <new-mac-address> 
sudo ifconfig <interface-name> up
```
We can see the list of interfaces using:
```
ifconfig
```
