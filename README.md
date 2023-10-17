# RockPiS
testing my pre-2022 [RockPi S](https://wiki.radxa.com/RockpiS
), ~~which may require Linux &lt;5.x~~

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/4ecfd7b2-407d-4e63-b946-d887a9b0acc5)

from: https://wiki.radxa.com/RockpiS/hardware/models

I have the RS308-D2 (256MB)- I plan to use Ethernet & SSH once it is set up but the first image I installed was actually a non-legacy version that is unsupported for RockPi S (debian bullseye kde b37), as I purchased mine in 2020. 

Edit: my first install with B37 actually did post a blue light (activity), although I was not able to get an IP address when connected to the Ethernet. The legacy version did not boot at all (just a green power led), thus it is possible that I can try the newer kernel if it has been updated.  

I also read that some of the newer images have a different bootloader, and I am not yet able to see if it can load the OS. Since the board I am using doesn't have any NAND flash, I wasn't planning on installing the OS anyways, but using the uSD card as a live-boot (and possibly removing it if loading an OS running in RAM) for something that can run in less than 256MB. My tests on the Raspberry Pi Zero v1.3 (not the 2W with a-53s) show that Raspup can boot from RAM using less than 512MB- and when idling uses around 100MB:

These videos were made last year that show the relative performance, showing that there would be enough room to run on 256MB:

https://www.youtube.com/watch?v=MMFIzx3Cm9Q

https://www.youtube.com/watch?v=inho4odu5gw

-----

https://xogium.performanceservers.nl/archive/rockpi-s/

https://forum.radxa.com/t/rock-pi-s-linux-images-not-booting/17032

Currently setting up adb: https://wiki.radxa.com/Rock/windows_adb

https://wiki.radxa.com/RockpiS/getting_started

https://wiki.radxa.com/RockpiS/hardware

https://www.oracle.com/java/technologies/downloads/#jdk21-windows

https://wiki.kobol.io/helios64/maskrom

https://www.thanassis.space/rockpis.html

https://nobytes.blogspot.com/2019/09/how-to-set-up-rock-pi-s.html

https://www.perl.com/article/the-rock-pi-s-or-how-to-get-gpio-input-without-a-library/

https://wiki.radxa.com/RockpiS/downloads

https://armbian.lv.auroradev.org/archive/rockpi-s/archive/

https://github.com/radxa-build/rock-pi-s/releases/tag/20220801-0043

https://github.com/radxa/rock-pi-s-images-released/releases (4.4x)

https://wiki.radxa.com/RockpiS/hardware/revisions

Found an image with Xfce pre-installed; ~~figured this should be easy enough to VNC into. May install a minimal build later on.~~

997 MB Sep 24, 2021: https://github.com/radxa/rock-pi-s-images-released/releases/download/rock-pi-s-v20210924/shajin_debian_buster_xfce4_arm64_20210924_0444-gpt.img.gz (<-did not work)

https://www.armbian.com/rockpi-s/#kernels-archive-all 

https://forum.radxa.com/t/vnc-server-chromium-gimp-etc/4466

https://github.com/t2age/RPS/tree/master/vnc

Armbian 22.08 Trunk Focal 5.15.58 Jul 31, 2022 https://github.com/radxa-build/rock-pi-s/releases/tag/20220801-0043 

https://forum.armbian.com/forum/200-rock-pi-s/ 

https://forum.radxa.com/c/rockpiS

(https://github.com/radxa-build/rock-pi-s/releases/download/20220801-0043/Armbian_22.08.0-trunk_Rockpi-s_focal_current_5.15.58_xfce_desktop.img.xz)https://github.com/radxa-build/rock-pi-s/releases/download/20220801-0043/Armbian_22.08.0-trunk_Rockpi-s_focal_current_5.15.58_xfce_desktop.img.xz (688MB) (takes up ~5.6GB on 8GB uSD card, flashed with Balena Etcher) Blue blinking LED and...I got an IP address:

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/17d1bdb5-ce7b-4181-8642-e0e164e23a73)

Now going to try SSH.

Putty did not work, yet.

Got a ping though

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/02407329-0c85-4e5c-ae98-5dc0121c59aa)

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/3042efc9-6737-4891-999d-e3761b69c537)

It's possible VNC isn't installed on Armbian. Will have to try the adb method. I had already installed Java and the Android SDK but I probably missed a directory or creating the "special folder" and ini files, since it didn't work the last time. (assuming this method lets me remote in). Could be Access Control. Might not be rock@rockpis.local but debian 

https://wiki.radxa.com/RockpiS/ssh I was able to ssh rock@192.168.1.25 and got 

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/1a3ad5d7-7627-4a3f-92a9-a62604341ab1)

but when I typed the password rock it said denied. 

Back to PuTTY:

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/0f54f65a-973a-4071-9f06-2326bf0ff5ae)

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/e53a3b92-cf70-4efb-9ab6-bf2b84bf8ae0)

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/64cf6ea9-9835-4c4f-b24d-1dfd5935f66d)
