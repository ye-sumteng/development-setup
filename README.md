# Development Setup
**Prepare development environment**
- **Boot Partition**: The location where we will put Ubuntu GRUB.
- **Swap Partition**: The partition used to swap files , its function is to add memory if the RAM is full. 
- **Root Partition**: The location where we will install Ubuntu.
- **Home Partition** (Optional): Home is the location where we will store personal files (documents, music, pictures, etc.). Because it is optional, we can add it or make it one with the Root partition. 

## Instal Ubuntu and setup dualboot on Windows 7
**Preparation for Ubuntu installation:**
- Windows 7 based Computer or Laptop
- USB Flashdisk (minimum **4 GB** ), you can also use a DVD disc.
- Ubuntu 20.04.01 LTS ISO file ( [download here](https://ubuntu.com) ).
- Rufus ( [download here](https://rufus.ie/en_US/) ).

### Setup Dualboot
*After the computer starts up but Ubuntu GRUB does not appear, but instead goes directly to Windows, you need to add the Ubuntu bootloader option in the MBR. For that please follow the steps below,* Download the EasyBCD application via [this link](https://www.techspot.com/downloads/3112-easybcd.html).

After download and install EasyBCD, do this:

1. Clicking **Add New Entry**
2. switching to the **Linux / BSD** tab
3. in the Type section, select **GRUB (Legacy)**
4. in the Name section enter **Ubuntu 10.04.01**
5. in the Drive section select the boot partition where the Ubuntu boot loader was installed earlier
6. hen click the **Add Entry** button .

![The following is an example of an **EasyBDC** image](https://www.konyoha.com/wp-content/uploads/2017/08/cara-install-dual-boot-ubuntu-windows-18.jpg)

When finished, select Edit Boot Menu and make sure the resultis like the image![](https://www.konyoha.com/wp-content/uploads/2017/08/cara-install-dual-boot-ubuntu-windows-19.jpg). 


Finally, please restart your computer again and the boot options will appear to select Windows or Ubuntu.
