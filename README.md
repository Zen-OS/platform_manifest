## Building Android ##

*Please note: This is only required if you've never built a ROM on the current machince you're using.

[Setting Up Build Environment](https://raw.githubusercontent.com/nathanchance/Android-Tools/master/Guides/Building_AOSP.txt)

## Repo Init ##
```bash
repo init -u https://github.com/Zen-OS/platform_manifest.git -b pie
```
## Sync Source ##
```bash
repo sync -c -f --force-sync --no-tag --no-clone-bundle -j$(nproc --all)
```
## Build Time (Linux x86_64 ONLY) ##
```bash
. build/envsetup.sh
brunch zen_<DEVICE>-userdebug (or zen_<DEVICE>-user)
```
