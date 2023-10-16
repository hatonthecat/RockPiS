# RockPiS
testing my pre-2022 [RockPi S](https://wiki.radxa.com/RockpiS
), ~~which may require Linux &lt;5.x~~

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/4ecfd7b2-407d-4e63-b946-d887a9b0acc5)

from: https://wiki.radxa.com/RockpiS/hardware/models

I have the RS308-D2 (256MB)- I plan to use Ethernet & SSH once it is set up but the first image I installed was actually a non-legacy version that is unsupported for RockPi S (debian bullseye kde b37), as I purchased mine in 2020. 

Edit: my first install with B37 actually did post a blue light (activity), although I was not able to get an IP address when connected to the Ethernet. The legacy version did not boot at all (just a green power led), thus it is possible that I can try the newer kernel if it has been updated.  

https://forum.radxa.com/t/rock-pi-s-linux-images-not-booting/17032

Currently setting up adb: https://wiki.radxa.com/Rock/windows_adb

https://wiki.radxa.com/RockpiS/getting_started

https://wiki.radxa.com/RockpiS/hardware

https://www.oracle.com/java/technologies/downloads/#jdk21-windows

https://wiki.radxa.com/RockpiS/ssh

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

997 MB Sep 24, 2021:

https://github.com/radxa/rock-pi-s-images-released/releases/download/rock-pi-s-v20210924/shajin_debian_buster_xfce4_arm64_20210924_0444-gpt.img.gz (<-did not work)

shajin_debian_buster_xfce4_arm64_20210924_0444-gpt.img

Kernel version: 4.4.143-65-rockchip-g58431d38f8f3

U-Boot version: 2017.09-02378-g6de46245e6

https://forum.radxa.com/t/vnc-server-chromium-gimp-etc/4466

https://github.com/t2age/RPS/tree/master/vnc

Armbian 22.08 Trunk Focal 5.15.58 Jul 31, 2022 https://github.com/radxa-build/rock-pi-s/releases/tag/20220801-0043 

https://forum.armbian.com/forum/200-rock-pi-s/ 

(https://github.com/radxa-build/rock-pi-s/releases/download/20220801-0043/Armbian_22.08.0-trunk_Rockpi-s_focal_current_5.15.58_xfce_desktop.img.xz)https://github.com/radxa-build/rock-pi-s/releases/download/20220801-0043/Armbian_22.08.0-trunk_Rockpi-s_focal_current_5.15.58_xfce_desktop.img.xz (688MB) Blue blinking LED and...I got an IP address:

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/17d1bdb5-ce7b-4181-8642-e0e164e23a73)

Now going to try SSH.

Putty did not work, yet.

Got a ping though

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/02407329-0c85-4e5c-ae98-5dc0121c59aa)

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/3042efc9-6737-4891-999d-e3761b69c537)

It's possible VNC isn't installed on Armbian. Will have to try the adb method. I had already installed Java and the Android SDK but I probably missed a directory or creating the "special folder" and ini files, since it didn't work the last time. (assuming this method lets me remote in). Could be Access Control. Might not be rock@rockpis.local but debian 

