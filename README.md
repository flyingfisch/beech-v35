Beechcraft V35 Bonanza for flightgear
=====================================
###Under Construction, many features may not work.

For Users
=========
##[Aircraft Help](http://forum.flightgear.org/viewtopic.php?f=4&t=22808&start=75)

Software Requirements
---------------------
###[YASim Version 32 or newer](#how-to-install-yasim-32-on-flightgear-300)

For Developers
==============

Notes on certain files
---------------------
* **beech-v35-indev.xml**: flyingfisch's first try at a YASim FDM

* **beech-v35-new.xml**: another attempt by flyingfisch at a YASim FDM

* **Blender/beech35.blend**: Main blend file

* **Blender/beecha35int.blend**: Interior

* **Blender/beech35_uvexample.blend**: modification of beech35.blend with i4dnf's UV Map.

* **blankinst.blend**: Blank instrument model




Appendix
--------

###How to install YASim 32 on Flightgear 3.0.0

1. Download the source for [flightgear](http://mirrors.ibiblio.org/pub/mirrors/flightgear/ftp/Source/) and [simgear](http://mirrors.ibiblio.org/pub/mirrors/simgear/ftp/Source/).
2. Install the dependency packages for your operating system (OSG, Boost, Glut (FreeGlut), OpenAL, plib)
3. Extract the source code for flightgear and simgear, which you downloaded in step 1.
4. Build simgear according to the instructions in `./INSTALL`. For *nix, you could do:

  >cd <simgear_dir>
  
  >cd ../
  
  >mkdir sgbuild
  
  >cmake ../simgear* -DCMAKE_BUILD_TYPE=Release
  
  >make
  
  >sudo make install

5. Download [YASim 32](http://emilianh.go.ro:6980/flightgear/misc/YASim.zip) and extract into `<flightgear_dir>/src/FDM/`
6. Then build flightgear according to the instructions in `./INSTALL`. For *nix, you could do:

  >cd <flightgear_dir>
  
  >cd ../
  
  >mkdir fgbuild
  
  >cmake ../flightgear* -DCMAKE_BUILD_TYPE=Release -DWITH_FGPANEL=OFF
  
  >make
  
  >sudo make install
  
7. Change your flightgear executable in FGRun to the new FG executable. You will see it in the output for `sudo make install` as something like `/usr/local/bin/fgfs`


