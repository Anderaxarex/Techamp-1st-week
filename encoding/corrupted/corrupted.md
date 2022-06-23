|---------- Challenge prompt ----------|

Corruption is a serious problem!
[downloadable: corrupted]

|---------- Challenge solution ----------|

upon opening the image with a hex editor like HxD [https://hxd.it.softonic.com/]
we can see that the first 12 bytes of the image have been replaced with 0x3F -> [?]
we can therefore replace those bytes with others found in fully functioning jpgs 
we were given in previous challenges. In my case I took them from "cards.jpg"
the new bytes now should read:

FF D8 FF E0 00 10 4A 46 49 46 00 01

NB: make sure you don't change any other bytes

once you saved them u can now open the image and see the flag

|---------- Challenge flag ----------|

the flag is in "corrupted.jpg"