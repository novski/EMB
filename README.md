# EMB

Embedded-Rack is a multi SoC Powersupply with i2c connections.
It can be used to power up to 13 Raspberry Pi's and
 one Microcontroller to monitor Powerconsumption in Rackcase.

## How to

- Get a 19 inch DIN Rack similar to this from [schroff](https://schroff.nvent.com/products/19-subracks).

- Create a Backcover like in the drawing of /powersupply 
accordingly to your powersupply. I use this [MeanWell RSP-200-5](https://www.meanwell.com/productPdf.aspx?i=437)

- Connect a Poweroutlet (with fuse) and solder it to the 
psu and the psu to the backplane with carefully chosen cable 
diameter regarding your psu. 

- Get some Backplane connectors with 24x2.54mm pinn's 
like this from [aliex](https://de.aliexpress.com/wholesale?catId=0&initiative_id=SB_20220409111809&SearchText=pcb+edge+connector).

- Solder some connectors to a daughter-card and push your SoC 
on it.
pi: [mouser](http://ch.mouser.com/Search/ProductDetail.aspx?R=M20-6102045virtualkey57420000virtualkey855-M20-6102045)

- Stick the daughter-board in to the backplane.

## Powermeasureing

The i2c connection between all SoC's can be used as plane 
communication while adding an TI INA219 can be interessting 
to measure power over a board separate. Check the adafruit 
repo's for software and the schematic for parts.

## Disclaimer

All granted for free as in speech, without waranty.
(means that you can use, modify, share, sell if you like. 
But don't try to sue me for mistakes you do yourself.)
Be carefull with Power and re-calculate all wires according 
to your needs.  