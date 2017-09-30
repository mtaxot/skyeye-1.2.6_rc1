# skyeye-1.2.6_rc1
This is skyeye arm emulator version 1.2.6 that could be build after 2017.

In order to build successfully, I altered the file :device/nandflash/nandflash_smallblock.c at line 519.

original code is released in 2008.09.17 : if ((nf->fdump= open(dev->dump, FILE_FLAG)) < 0) 

alter it with: if ((nf->fdump= open(dev->dump, FILE_FLAG, 0777)) < 0)

I have compiled it successfully. If you use old OS, just change it back.

