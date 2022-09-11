## Tutorials(updating)
#### How to open and connect adb
- [⚡Open and connect adb(From google)](https://developer.android.com/studio/command-line/adb)
- [👍Open mobile adb(Android 4.x ~ Android 13)](./openMobileADB4x_13.md)
- [Open mobile adb(Android 11 ~ Android 13)](./openMobileADB11_13.md)
- [Open TV adb](./openTVADB.md)
- [👍Connect adb (Android 4.x ~ Android 13)](./connectADB4x_13.md)
- [Pair and connect adb (Android 11 ~ Android 13)](./connectADB11_13.md)


#### FAQ
1. ##### The toolbox to disable apps doesn't work.

   Disable system application is not allowed.
   ```
   Security exception: Shell cannot change component state for com.android.bluetooth/null to 2

   java.lang.SecurityException: Shell cannot change component state for com.android.bluetooth/null to 2
        at com.android.server.pm.PackageManagerService.setEnabledSetting(PackageManagerService.java:21420)
        at com.android.server.pm.PackageManagerService.setApplicationEnabledSetting(PackageManagerService.java:21305)
        at com.android.server.pm.PackageManagerShellCommand.runSetEnabledSetting(PackageManagerShellCommand.java:1826)
        at com.android.server.pm.PackageManagerShellCommand.onCommand(PackageManagerShellCommand.java:212)
        at android.os.ShellCommand.exec(ShellCommand.java:104)
        at com.android.server.pm.PackageManagerService.onShellCommand(PackageManagerService.java:21884)
        at android.os.Binder.shellCommand(Binder.java:881)
        at android.os.Binder.onTransact(Binder.java:765)
        at android.content.pm.IPackageManager$Stub.onTransact(IPackageManager.java:4892)
        at com.android.server.pm.PackageManagerService.onTransact(PackageManagerService.java:4010)
        at android.os.Binder.execTransactInternal(Binder.java:1021)
        at android.os.Binder.execTransact(Binder.java:994)
   ```

2. ##### How to use the app locally?
   1. Open and connect adb.[How to open and connect adb](./md/tutorials.md)
   2. Disable pairing mode.
   3. Default IP 127.0.0.1 and default port 5555 is local mode.
      - <img src="./../image/connectADB4x_13/1.jpeg" width="270" height="300">

3. ##### *lib/arm/libfs.so inaccessible or not found.
   - Solution 1:Click reset the app.
   - Solution 2:Reinstall the app.

4. ##### error: device unauthorized.This adb server\'s $ADB_VENDOR_KEYS is not set
   - Solution 1:Click restart app.
   - Solution 2:
   ```
    $ adb kill-server
    $ adb start-server
      * daemon not running; starting now at tcp:5037
      * daemon started successfully
   ```

5. ##### error: more than one device/emulator
   Input \"adb devices\".Use \"adb -s IP:PORT\" select a specific device.
   ```
   $ adb devices
     List of devices attached
     192.168.3.100:5556      device
     192.168.3.101:5555      device
   $ adb -s 192.168.3.101:5555 shell
     console:/ $
   ```