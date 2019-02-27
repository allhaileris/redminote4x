# redminote4x

### Diag mode:
```bash
adb shell
su
setprop sys.usb.config diag,adb
```

### Reset modem firmware:
```bash
# Boot into TWRP recovery.
# From TWRP’s main screen, select Advanced » then Terminal.
# Type the following commands in terminal (one by one):

dd if=/dev/zero of=/dev/block/bootdevice/by-name/modemst1
dd if=/dev/zero of=/dev/block/bootdevice/by-name/modemst2

# Reboot device.
```
