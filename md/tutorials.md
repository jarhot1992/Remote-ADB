## Tutorials(updating)
#### How to open and connect adb
- [⚡Open and connect adb(From google)](https://developer.android.com/studio/command-line/adb)
- [👍Connect adb (Android 4.x ~ Android 13)](./connectADB4x_13.md)
- [Pair and connect adb (Android 11 ~ Android 13)](./connectADB11_13.md)
- [👍Open mobile adb(Android 4.x ~ Android 13)](./openMobileADB4x_13.md)
- [Open mobile adb(Android 11 ~ Android 13)](./openMobileADB11_13.md)
- [Open TV adb](./openTVADB.md)


#### FAQ
1. ##### 32 or 64 bit libraries?
   - Default:32-bit.32-bit library compatibility is stronger.
   - 64-bit libraries are more stable.
   - 64-bit libraries are faster.If it takes too long to connect the device, you can try to switch the 64-bit library.
   - 64-bit libraries are recommended for Android 12 and above.

2. ##### Failed: Unable to start pairing client.
   1. 🥝 Check your pair port. [Pair and connect adb (Android 11 ~ Android 13)](./connectADB11_13.md)
   2. If it still doesn't work, you can try to switch the 64-bit library in the settings.
   3. If it still doesn't work, you can try to switch to another connection mode. [👍Connect adb (Android 4.x ~ Android 13)](./connectADB4x_13.md)


3. ##### How to use the app locally?
   1. Open and connect adb.[How to open and connect adb](./md/tutorials.md)
   2. Disable pairing mode.
   3. Default IP 127.0.0.1 and default port 5555 is local mode.
      - <img src="./../image/connectADB4x_13/1.jpeg" width="270" height="300">

4. ##### *lib/arm/libfs.so inaccessible or not found.
   - Solution 1:Click reset the app.
   - Solution 2:Reinstall the app.

5. ##### error: device unauthorized.This adb server\'s $ADB_VENDOR_KEYS is not set
   - Solution 1:Click restart app.
   - Solution 2:
   ```
    $ adb kill-server
    $ adb start-server
      * daemon not running; starting now at tcp:5037
      * daemon started successfully
   ```

6. ##### error: more than one device/emulator
   Input \"adb devices\".Use \"adb -s IP:PORT\" select a specific device.
   ```
   $ adb devices
     List of devices attached
     192.168.3.100:5556      device
     192.168.3.101:5555      device
   $ adb -s 192.168.3.101:5555 shell
     console:/ $
   ```
7. ##### sh:<stdin>[] ** inaccessible or not found
   - Please confirm that the command you entered is correct.
   
8. ##### Google Intel Chromebooks are not supported.  Intel x86(x64) chip is not supported(Only support arm chip).  Please use Google official adb for intel x86(x64).
