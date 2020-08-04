# Internal OPL3 ISA 8 bits

![alt text](ISAOPL3.png "ISAOPL3")

The schematic is Based on Texelec's Resound OPL v1.1 board:

https://www.tindie.com/products/TexElec/resound-opl3-4-channel-sound-card-8-bit-isa/

# version 1.2

* Track two vias forgotten in development of version 1.1

# version 1.1

* Modification of YMF762 and YAC512 footprint dimensions

* Silkscreen of 74HC245 changed to 74HCT245

* Added two resistors in the back layer to solve the problem of version 1.0

# version 1.0

Symptoms:

The first start is always correct, it works and you can hear it perfectly, clear FM OPL3 sound ... but after approximately 2 minutes, it stops working. Normally a sleep period without connecting makes it work again, but there have been cases in which it stops working forever...  (that should be because component 74245 was not TTL, I've already put a TTL in it, now it always works after a rest period):

https://youtu.be/4GyFgOpV200

FIX: 

Specifically the primary 1uF capacitors were left charged, I have solved this by adding a couple of resistors. Finally, and after several fixes, we have it running at full capacity:

https://www.youtube.com/watch?v=0QMfLWs73HM

