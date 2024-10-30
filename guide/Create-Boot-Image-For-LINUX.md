# Create Boot Image For LINUX

## If You have linux boot image or You using [KALI LINUX](https://github.com/Xyy155/Triple-Boot-on-Xiaomi-Pad-5/releases/tag/image) You don't have to do that

> [!NOTE]
> ### If you have [KALI LINUX](https://github.com/Xyy155/Triple-Boot-on-Xiaomi-Pad-5/releases/tag/image) You can find linux.boot.img BUT USE IT ONLY FOR THIS KALI IMAGE!

### Prerequisites
- Brain
 
- [mklonimg.cmd (Windows)](https://git.timoxa0.su/timoxa0/mklonimg/raw/branch/main/mklonimg.cmd)

- [mklonimg.sh (Linux/macOS)](https://git.timoxa0.su/timoxa0/mklonimg/raw/branch/main/mklonimg.sh)

- [Python 3](https://www.python.org/downloads/)

- [dtb and vmlinuz](https://www.mediafire.com/folder/orb4j5rxb2wew/vmlinuz_and_dtb)

### Creating boot image

1. #### Download mklonimg.cmd for Windows or mklonimg.sh for Linux/macOS

2. #### Install Python (for Windows select Add Python 3.x to PATH)

3. #### Download dtb and vmlinuz 

4. #### Open cmd (on Windows) or terminal (on Linux/macOS)

5. #### Run mklonimg
##### Windows
```
.\mklonimg.cmd path\to\vmlinuz path\to\dtb
```
##### Linux/macOS
```
bash mklonimg.sh path/to/vmlinuz path/to/dtb
```

8. #### Image will be created in current working directory with name linux.boot.img

### Done!

# [NEXT STEP: Booting Programs](/guide/Booting-Programs.md)
