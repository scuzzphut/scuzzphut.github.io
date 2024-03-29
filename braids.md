
# [Back to Main](README.md)
## Through Hole Braids

This was built from the project at https://sound-force.nl/?page_id=3179

This project uses the open source hardware and software for the Mutable Instruments Braids module and makes it a DIY project by converting all the components to through-hole (as opposed to SMD) and utilising the freely available STM32 development board, commonly known as Bluepills, in place of the bare, SMD  STM32 microcontroller.
I ordered the PCBs from JLCPCB, using the Gerber files on the Soundforce site. I then ordered a front panel from [Pusherman](https://pushermanproductions.com/) 

_________________________________________________________________________________________________________

If you have a problem with your Bluepill not working after flashing the Braids.hex file from Soundforce, then you might be missing the bootloader.


Download the Braids bootloader Hex file from here 

https://github.com/hadesbox/eurorack-with-binaries/tree/master/build/braids_bootloader

Then : 

Hook up to USB with one of [these USB programmers](https://www.aliexpress.com/item/32650897782.html?spm=a2g0o.store_pc_allProduct.8148356.2.4cfe7fa8uE16Xa&pdp_npi=2%40dis%21GBP%21%EF%BF%A11.26%21%EF%BF%A11.26%21%21%21%21%21%400b0a050b16563199459717993e3303%2159712037485%21sh) 

Connect the programmer to the Bluepill according to this diagram

https://maker.pro/storage/qHO4fjd/qHO4fjduHRu1vlrTE1BBLS5BNqgOOLcwLD5vri2o.png

Set the Bluepill to "program" mode with the jumpers

https://maker.pro/storage/pHZODf2/pHZODf2gl1Sm2G5PN6lQJ5DlJRxnBNHhEOUjDJFp.jpeg

Run STM32CubeProgrammer and load the bootloader hex file.  Connect to the bluepill and hit download. 

Set the Bluepill to "normal" mode with the jumpers 

https://maker.pro/storage/p1x4wNc/p1x4wNcrRnZu0i7WvVDVl13kN7yBmUbYKCIctQxI.jpeg

Hit the reset button, then disconnect the Bluepill.

__________________________________________________________________
Here are the files I used

https://drive.google.com/drive/folders/1qnwXdYXiXw3sq80_oz1vbogOyd97HgBz?usp=sharing
