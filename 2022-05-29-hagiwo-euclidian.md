# [Back to Main](README.md)
## Hagiwo's Euclidian sequencer.

I placed an order with JLCPCB for the [panel and pcb from here.](https://github.com/Testbild-synth/Hagiwo_009_030_sequencer) 

![Untitled.jpg]({{site.baseurl}}/Untitled.jpg)


My plan was to use an [STM32 bluepill](https://www.aliexpress.com/item/1609750475.html?spm=a2g0o.order_list.0.0.21ef1802q0V3jR) that I had in the parts bucket, but the bluepills are not direct replacements for real Arduino Nano boards. (Nano has 30 pins, bluepill has 40) Another lesson learned.

Arduino nanos are very expensive at the moment, but I picked up a 3-pack of [Elegoo clones from Amazon](https://www.amazon.co.uk/gp/product/B072BMYZ18/ref=ppx_yo_dt_b_asin_title_o02_s00?ie=UTF8&psc=1) for £20. 

These are the same ATMega chip as the official Nano, but they use a different communications chip (CH340). 

All you have to do is download and install [the driver from the Elegoo site](http://69.195.111.207/tutorial-download/?t=Nano3.0) and you can program them with Hagiwo's software.

One minor gripe with this module is that there is no clock reset input, so when you stop / start your clock the module just continues from where it left off. 
