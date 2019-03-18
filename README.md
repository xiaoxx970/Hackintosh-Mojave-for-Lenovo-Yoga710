# Mojave-for-Lenovo-Yoga710
I've been attempt making my laptop work with mojave for like one month, and bought a DW1820 wireless card to fix network problem.  Also there's a lot of problem like brightness, bluetooth, app store, etc. It's all work now.

The most tricky part is to drive DW1820(What? I bought it for hackintosh!), I do found kext driver for my card from RehabMan, but seems not work at all. Every time I boot up I see this![](error1.jpg)
Maybe something wrong with Bluetooth since it's connected via USB. But I fixed it by just delete `BrcmPatchRAM2.kext` and `BrcmFirmwareData.kext`, and add the address of bluetooth's USB port to `FakePCIID.kext`, it workd fine then. no  need of other kext driver.

Here's my hardware:
- Processor: Intel Core i5-7200U
- Graphics: Intel HD Graphics 620, NVDIA Geforce 940MX
- Memory: 4096 MB, 2133 MHz, DDR4, 1/1 slots occupied, Single-Channel
- Display: 14 inch 16:9, 1920 x 1080 pixel 157 PPI, Multitouch
- Mainboard: Intel Kaby Lake-U Premium PCH

# What works well:
- Graphics, Brightness(and save brightness)
- Keyboard & Trackpad
- Audio
- Battery
- Airprot
- Bluetooth
- HDMI output with audio
- Headphone jack include microphone

# What is not working:
- NVDIA Geforce 940MX
- Touch screen
- Sleep function(just about work, it wake immediately after sleep)
- SD card reader

# Something you need attention:
- brightness can be adjust at setting, you can add a key map yourself.
- You can enable HIDPI https://github.com/xzhih/one-key-hidpi

I'm just put my clover files here, hope there's help for you. As for installing detals, check here:[Hackintosh Installer University](https://github.com/huangyz0918/Hackintosh-Installer-University)

## Download link: [CLOVER.zip](https://xiaoxx.cc/hackintosh-of-yoga710/CLOVER.zip)