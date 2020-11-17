# SL030
A driver package for the SL030 RFID tag reader.

For use with SKPang Electronics SL030 RFID module,
with a SL030 Raspberry Pi cable, and any model Raspberry Pi,
product numbers: RFID-SL030, RSP-SL030-CAB

[SKPang product info](http://skpang.co.uk/blog/archives/946)

![PiZero with SL030](pizeroW_SL030.png "PiZeroW+SL030")

Works on all Pi models, with Python2 and Python3.

## Example Program

Run the example as follows:

```
   python rfid_example.py
```

or

```
    python3 rfid_example.py
```

Then bring a tag close to the reader, and you should see it's ID number
displayed on the console. The red light on the front of the reader board
also lights when it detects a tag.

You can use any mifare tag - such as an oyster card, an NFC enabled credit
or debit card, and many sticky labels and key fobs that are advertised as
'Mifare compatible' (13.56MHz tags). This does NOT include hitag tags,
so make sure you get the right tag before you use this card.

The driver only supports the 'read id' method of the card, as that is the
most common use case, and what I needed for the projects that I was building
at the time. The Mifare standard does support readable and writeable
memory locations on cards that have memory, and other secure key transactions.


## Notes

1. The 20/08/2020 build of RaspberryPi OS Lite doesn't have RPi.GPIO installed
for Python3 (does for Python2). You can install it manually though: 
[instructions here](https://github.com/whaleygeek/SL030/issues/1#issuecomment-728889189)

2. On older Pi's you will have to prefix commands with sudo,
but all newer Pi's and OS's support the gpiomem mod where you
no longer need root access to use the GPIO.

Last tested 17/11/2020

@whaleygeek

17 Nov 2020
