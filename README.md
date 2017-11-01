# SL030
A driver package for the SL030 RFID tag reader

http://blog.whaleygeek.co.uk/raspberry-pi-rfid-tag-reader

NOTE: if you want this to run without sudo, there is a mod to do to
gpio.c to add in the extra device tree path for the sudo-less GPIO.
You can find a version of the code for  that at 
https://github.com/whaleygeek/pyenergenie

For use with SKPang Electronics SL030 RFID module,
with a SL030 Raspberry Pi cable, and a Raspberry Pi
running Raspbian Wheezy.

product numbers: RFID-SL030, RSP-SL030-CAB
http://skpang.co.uk/blog/archives/946

Run this program as follows:

```
   sudo python rfid_example.py
```

or

```
sudo python3 rfid_example.py
```