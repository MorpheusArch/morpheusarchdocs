# MorpheusArch Docs
Documentation for MorpheusArch Linux
# Attention
Initially I was going to make this repo private but github requires ££/$$ for a private repo. At this point in time the documentation is a Work in Progress.

# Create a bootable USB 

The recommended way is with the use of the dd command some tools exist for creating bootable flash drives but they are neither recommended nor officially supported. 

 sudo dd bs=4M if=MorpheusArch.iso of=/dev/sdX

# if is always before of

Failure to do so WILL result in the loss of data.

Remember to replace <MorpheusArch> with the current release of MorpheusArch and 
 
Also remember to replace /dev/sdX with your flash drive. You can find your flash drive with use of the command:
  
lsblk
  
# Select the USB as the boot media

This varies from device to device. You need to enter the boot order in the BIOS of the system you are booting into.

# Boot from the USB

Once it is booted you'll be presented with the login screen. Login as root with no password and you can begin recovering data.
