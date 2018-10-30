# TPL5110 Nano Power System Timer
Want to control your microcontroller's power? This may be the answer.

**Sponsored by www.PCBWay.com PCB** Prototype the Easy Way  
We are giving a free prototype for Christmas PCB and will choose one most popular design to be made 1,000 pcs to give away randomly as PCBWay 2018 Christmas Gift.

# See video #125 at https://www.youtube.com/ralphbacon  
(Direct link to video: https://youtu.be/Qms_iEL7Uqg)

In a previous video #122 we explored switching off an Arduino (or other µcontoller) by using the device itself. 

In **this** video we look at the TPL51110 device which does much the same thing but periodically - hence the **timer** part of the name.

Adafruit breakout board:  
https://learn.adafruit.com/adafruit-tpl5110-power-timer-breakout?view=all

An alternative breakout board:  
https://lowpowerlab.com/shop/product/147

Aliexpress source of bare SMD chip (lot of 10):  
https://www.aliexpress.com/item/10pcs-lot-TPL5110DDCR-TPL5110-ZALX-IC-6-SOT/32914309796.html

There are some caveats covered in the video, but here's some extra information you may find useful:

1. The minimum delay/switch on period is 100mS ±0.6%   
2. The maximum delay/switch on period is 2 hours ±0.6% (7200 seconds)  
3. To get *precise* timings you will need to parallel two 1% tolerance resistors (the datahsheet shows what values)  
4. The "DONE" signal back to the TPL5110 from your microcontroller is 100mS minimum  
5. The TPL5110 is *only* available as a surface mount device (and it is **tiny**)  
6. The TPL5110 expects to drive a P-channel MOSFET that switches the power line to the µController. HIGH is OFF and LOW is ON.  
7. This device plus supporting components consume about 20µA whilst in switch-off mode
8. This devices works on voltages from 1.8 volts to 5.5 volts
9. All pins are 5v tolerant **BUT must not exceed VDD + 0.3 volts** (so if running on 3.3 volts must not exceed 3.6v)
8. The Adafruit breakout module has a mximum current capability of 4 Amps
 
In a future video we'll look at the TPL5111 which is subtly different.

So having watched the video and understood how this device actually works, do you think it has a place in low-powered microcontroller devices (such as home automation, measuring, alarms and the like)?

Comments, observations and question under the video please, I'd love to hear your thoughts.

If you like this video please give it a thumbs up, share it and if you're not already subscribed please consider doing so :)

My channel and blog are here:  
------------------------------------------------------------------  
https://www.youtube.com/RalphBacon  
https://ralphbacon.blog  
------------------------------------------------------------------  
