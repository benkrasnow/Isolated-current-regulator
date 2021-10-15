# Isolated-current-regulator
Small linear current regulator powered by a 9V battery

Designed to provide a constant 8mA with up to 100V drop.  This circuit is adjustable from 0 to 100mA, and will quickly become thermally limited.  The transistor can hold back 400V, so the circuit could be operated at 2mA at 350V and still be within thermal limits of about 1 or 2W.

9V clip on Digikey: https://www.digikey.com/en/products/detail/keystone-electronics/968/151577

It's possible the TL431 would have been a more elegant and lower parts-count way of doing this.

When there isn't enough voltage across the terminals to achieve the set current limit (ie when it is disconnected), the circuit will put maximum current into the transistor base.  In this case, it is probably limited by the opamp.  I noticed about 25mA max, but it seems to be only 10mA when the circuit is set for 8mA.  Adding a 1K base resistor would lower this idle current, which is pretty wasteful, and still easily allow operation up to 100mA. 

![alt text](https://github.com/benkrasnow/Isolated-current-regulator/blob/main/3Drender.jpg?raw=true)
![alt text](https://github.com/benkrasnow/Isolated-current-regulator/blob/main/front.jpg?raw=true)
![alt text](https://github.com/benkrasnow/Isolated-current-regulator/blob/main/back.jpg?raw=true)
