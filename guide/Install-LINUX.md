# Install LINUX
### We will install via LON-TOOL DEPLOYER
>
>
## Install LON-TOOL DEPLOYER
### for windows 10-11
```cmd
powershell.exe -C "irm https://s.tx0.su/ltw | iex"
```
>
### for LINUX/MAC OS
```cmd
curl -Ls s.tx0.su/ltl | bash
```
## Install LINUX on NABU
#### Reboot to FastBoot to use  LON-TOOL DEPLOYER
```cmd
adb reboot bootloader
```
### deploy image
```cmd
lon-tool deploy /PATH/TO/IMAGE.LNI
```
>[!WARNING]
>When LON-TOOL say
>
>Found compatible partition table. Do you want to change it? [y/N]
>
>PLEASE SAY NO!
>

### Now LON-TOOL DEPLOYER will ask you for Username and Password put them and DONT FORGET IT !

### Wait for LON-TOOL DEPLOYER to flash LINUX

### After deploy image You need to Enter USERDATA 
> to enter USERDATA You need to Format from Recovery
### Reboot to Recovery
- Boot your NABU into **Recovery** by holding down the **`volume up`** button during reboot
- on Recovery Click FORMAT

#### Reboot to FASTBOOT
- Boot your NABU into **fastboot** by holding down the **`volume down`** button during reboot

### Disable Vbmeta
#### You Can Download Image [HERE](https://www.mediafire.com/file/pjy486vglviww10/vbmeta_disabled.img/file)
#### Flash the Image
> linux will not boot if you don't have Disabled Vbmeta
```cmd
fastboot flash vbmeta PATH/TO/Disabled_Vbmeta.IMG
```

### Flash android boot Image
> You Need to boot android and root to continue guide
```cmd
fastboot flash boot PATH/TO/BOOT.IMG
```
> Now Reboot to Android
```cmd
fastboot reboot
```

# [NEXT STEP: ROOT Android](/guide/ROOT-Android.md)
