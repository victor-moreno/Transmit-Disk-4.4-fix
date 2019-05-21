# Transmit-Disk-4.4-fix

Transmit Disk is not working for recent OSX versions.
Here is a fix:

1. Install latest osxfuse:
https://osxfuse.github.io/

2. Open terminal:
```
sudo -s
cd /Library/Filesystems/transmitdisk.fs/Contents
mv Extensions E
ln -s  ../../osxfuse.fs/Contents/Extensions Extensions
````
