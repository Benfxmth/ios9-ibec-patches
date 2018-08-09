# ios9-ibec-patches

Files for patching iBEC from clearing boot-partition variable when booting an iOS 9 iBEC with xerub's iOS 7 iBoot exploit for iPhone5,2. To apply the patches, first download the .ipsw file from here: https://ipsw.me. Then, decrypt the iBEC with xpwntool from Odysseus by typing `xpwntool /path/to/orig/iBEC /path/to/decrypted/iBEC -iv <iv_here> -k <key_here>`. You can find the keys here: 
https://www.theiphonewiki.com/wiki/Firmware/iPhone/9.x#iPhone5.2C2 
Now, download the .patch files, to patch the iBEC, run this command: `bspatch /path/to/decrypted/iBEC /path/to/patched/iBEC /path/to/.patch` There are 2 different .patch files, one enables verbose booting, and the other does not.
