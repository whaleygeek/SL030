# SL030
A driver package for the SL030 RFID tag reader.

Works on all Pi models, with Python2 and Python3.

Note that the 20/08/2020 build of RaspberryPi OS Lite doesn't have RPi.GPIO installed
for Python3 (does for Python2). You can install it manually though: 
https://github.com/whaleygeek/SL030/issues/1#issuecomment-728889189

For use with SKPang Electronics SL030 RFID module,
with a SL030 Raspberry Pi cable, and any model Raspberry Pi.

Last tested 17/11/2020

product numbers: RFID-SL030, RSP-SL030-CAB
http://skpang.co.uk/blog/archives/946

On older Pi's you will have to prefix commands with sudo,
but all newer Pi's and OS's support the gpiomem mod where you
no longer need root access to use the GPIO.

Run this program as follows:

```
   python rfid_example.py
```

or

```
    python3 rfid_example.py
```

@whaleygeek

17 Nov 2020
