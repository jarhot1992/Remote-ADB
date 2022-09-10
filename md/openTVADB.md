##### How to open mobile ADB
Different models of phones may be slightly different!
1. Open system setting app
2. Click 'Device Preferences'
   - <img src="./../image/openTVAdb/1.png" width="640" height="360">
3. Click 'About'
   - <img src="./../image/openTVAdb/2.png" width="640" height="360">

4. Click on 'Android TV OS build' or 'Build number' until developer mode is enabled
   - <img src="./../image/openTVAdb/3.png" width="640" height="360">
   - <img src="./../image/openTVAdb/4.png" width="640" height="360">

5. Click 'Developer options'
   - <img src="./../image/openTVAdb/5.png" width="640" height="360">

6. Enable 'USB debugging'
   - <img src="./../image/openTVAdb/6.png" width="640" height="360">

7. Click 'OK'
   - <img src="./../image/openTVAdb/7.png" width="640" height="360">
   - <img src="./../image/openTVAdb/8.png" width="640" height="360">

8.  Connect the USB cable.
9.  Open your PC shell or powershell and input 
    ```
    $ adb devices
    List of devices attached
    HT********	device

    $ adb tcpip 5555
    restarting in TCP mode port: 5555
    ```


