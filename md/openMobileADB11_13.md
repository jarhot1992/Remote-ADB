<a id="how-to-open-mobile-adb"></a>

# How to Enable Mobile ADB: Android 11+ Wireless Debugging

Prepare the target phone for pairing with the legacy app. The original screenshots document Android 11–Android 13; the tutorial index also lists Android 14.

<a id="1-different-models-of-phones-may-be-slightly-different"></a>
<a id="2-this-tutorial-generally-requires-two-android-phones"></a>

## Before You Begin

- The illustrated legacy pairing workflow **generally requires two Android phones**.
- Menu names can differ between phone models and firmware.
- Use the same local Wi-Fi network for the target phone and the phone running the app.

## Steps

1. Open the phone's **Settings** app.
2. Tap **About phone**.

   <img src="./../image/openMobileAdb/01.png" width="270" height="480" alt="About phone in Android Settings">

3. Tap **Build number** repeatedly until developer mode is enabled.

   <img src="./../image/openMobileAdb/02.png" width="270" height="480" alt="Build number in device information">

   <img src="./../image/openMobileAdb/03.png" width="270" height="480" alt="Developer mode enabled">

4. Open **System**.

   <img src="./../image/openMobileAdb/04.png" width="270" height="480" alt="System settings">

5. Open **Developer options**.

   <img src="./../image/openMobileAdb/05.png" width="270" height="480" alt="Developer options entry">

   <img src="./../image/openMobileAdb/06.png" width="270" height="480" alt="Developer options screen">

6. Enable **USB debugging**.

   <img src="./../image/openMobileAdb/07.png" width="270" height="480" alt="USB debugging switch">

7. Tap **OK** to confirm.

   <img src="./../image/openMobileAdb/08.png" width="270" height="480" alt="Confirm USB debugging">

8. Enable **Wireless debugging**.

   <img src="./../image/openMobileAdb/13.png" width="270" height="480" alt="Wireless debugging switch">

   <img src="./../image/openMobileAdb/12.png" width="270" height="480" alt="Wireless debugging enabled">

## Pair and Connect

Continue with [Pair and connect ADB](connectADB11_13.md). Read the pairing IP address, port, and code from **Pair device with pairing code**. After pairing, use the connection address from the main Wireless debugging screen and disable pairing in the legacy app.

The original illustrated steps retain USB debugging. Android's current wireless debugging setup is documented separately in the [official ADB guide](https://developer.android.com/tools/adb#connect-to-a-device-over-wi-fi). DroidKit's newer methods are in the [video table](tutorials.md#connection-videos).

[All tutorials and FAQ](tutorials.md#how-to-open-and-connect-adb) · [Back to Remote-ADB](../README.md)
