# image-reconstruction

Out of necessity, I had to write some scripts to reconstruct single coil images from multichannel acquisition data.


THE THINGS YOU NEED:

1. pvtools - Bruker used to have nice support for image/data manipulation using matlab scripts. They no longer support this format, but I found some other user on GitHub who had a public repo with the code. I have forked it into this directory, and made minor modifications to help ease the transition from PV4 (?) to PV5/PV6.

2. BrukerImageImporter - If you want to reconstruct your single-channel images without scaling, use this simple tool. I have not commented very well, and I will go back to change that. However, it should be relatively self-explanatory.

3. BrukerImageRecon - This is the ONLY THING YOU WILL EVER NEED for offline reconstruction of multichannel images acquired using Cartesian k-space trajectory. Quite honestly, there is too much information in the headers to be parsed manually, so I have modified the old Bruker scripts to work with data I have aquired using the CryoCoil and PV6.01. Just point the script at the directory with your acqp, method, and fid files and it does the rest.


Enjoy!
Hari
