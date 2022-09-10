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