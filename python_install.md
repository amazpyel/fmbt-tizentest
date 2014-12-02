How to install python on emulator
================
1. Download [python-base](https://download.tizen.org/releases/2.2/tizen-2.2/repos/tizen-base/ia32/packages/i586/python-base-2.7.1-1.4.i586.rpm)
2. Download [libpython](https://download.tizen.org/releases/2.2/tizen-2.2/repos/tizen-base/ia32/packages/i586/libpython-2.7.1-1.4.i586.rpm)
3. Launch Emulator
4. Push and install:
- sdb root on
- sdb push *.i586.rpm /tmp
- sdb shell rpm -i /tmp/*.i586.rpm
