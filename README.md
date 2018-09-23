#Instructions for setuping DualBoot (Specificaly for ASUS ZENBOOK  - dualboot windows 7 with ubuntu)

With this setup you can delete all the files on disk. Backup everything important!

1. **Installation of Windows UEFI**  
Its important that both Ubuntu and Windows are the same type: legacy or UEFI (and UEFI is more up do date)  
To instal windows UEFI :
    1. Make a bootable USB with RUFUS, and make it type UEFI
    1. On the computer you are installing Windows on go to bios and do:
        1. Boot->Launch CSM-> [Enabled]  (turn on the suport for legacy sysetems)
        1. Advanced->USB configuration->XHCI Pre-Boot Mode -> [Disabled] (Disable USB 3.0 in bios, because this usually works only with USB 2.0)
    1. Install Windows UEFI with pressing ESC on boot and choosing UEFI type
    1. (If during instalation you get an error about GPT formatting) Follow [THIS](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/windows-setup-installing-using-the-mbr-or-gpt-partition-style) tutorial
    
1. **Install Linux**  
After installing Windows, replace the Win USB stick with Linux USB stick (made with RUFUS or PowerISO) and install Linux as you normally would.

1. **Reenable USB 3.0**  
After installing both OSs be shure to enable USB 3.0 again in BIOS->Advanced->USB configuration->XHCI Pre-Boot Mode -> [Enabled]       
    