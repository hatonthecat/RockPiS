# RockPiS
testing my pre-2022 RockPiS, which requires Linux &lt;5.x

![image](https://github.com/hatonthecat/RockPiS/assets/76194453/4ecfd7b2-407d-4e63-b946-d887a9b0acc5)

from: https://wiki.radxa.com/RockpiS/hardware/models

I have the RS308-D2 (256MB)- I plan to use Ethernet & SSH once it is set up but the first image I installed was actually a non-legacy version that is unsupported for RockPi S (debian bullseye kde b37), as I purchased mine in 2020. 

Edit: my first install with B37 actually did post a blue light (activity), although I was not able to get an IP address when connected to the Ethernet. The legacy version did not boot at all (just a green power led), thus it is possible that I can try the newer kernel if it has been updated.  

https://forum.radxa.com/t/rock-pi-s-linux-images-not-booting/17032

https://wiki.radxa.com/RockpiS

Currently setting up adb: https://wiki.radxa.com/Rock/windows_adb

https://wiki.radxa.com/RockpiS/getting_started

https://wiki.radxa.com/RockpiS/hardware

https://www.oracle.com/java/technologies/downloads/#jdk21-windows

https://wiki.radxa.com/RockpiS/ssh

https://wiki.kobol.io/helios64/maskrom

https://wiki.radxa.com/RockpiS/downloads

https://armbian.lv.auroradev.org/archive/rockpi-s/archive/

https://github.com/radxa-build/rock-pi-s/releases/tag/20220801-0043

https://github.com/radxa/rock-pi-s-images-released/releases (4.4x)

Found an image with Xfce pre-installed; figured this should be easy enough to VNC into. May install a minimal build later on.

997 MB Sep 24, 2021:

https://github.com/radxa/rock-pi-s-images-released/releases/download/rock-pi-s-v20210924/shajin_debian_buster_xfce4_arm64_20210924_0444-gpt.img.gz

shajin_debian_buster_xfce4_arm64_20210924_0444-gpt.img

Kernel version: 4.4.143-65-rockchip-g58431d38f8f3

U-Boot version: 2017.09-02378-g6de46245e6

https://forum.radxa.com/t/vnc-server-chromium-gimp-etc/4466

https://github.com/t2age/RPS/tree/master/vnc
