# GrapheneOS for normal usage: privacy without paranoia

This repository aims to provide a simple guide to set up GrapheneOS on Google Pixel devices. It is intended for users who want better privacy and control of their mobile device without sacrificing usability or spending much time.

I created this repo because when I looked for resources on how to set up GrapheneOS, almost every one I found aimed at users with extreme privacy concerns (at the expense of usability). I just wanted a practical, everyday smartphone experience with better privacy and control, without giving up much usability or spending excessive time configuring it.

<br>

## Instalation


Open up a web browser and go to the [official installation page](https://grapheneos.org/install/) (here I am going to explain de [WebUSB-based installer](https://grapheneos.org/install/web) because is the easiest method).
Before continuing check if your browser, OS and mobile are supported.

> All Google Pixel devices from Pixel 6 through Pixel 10 Pro Fold are supported by GrapheneOS but you can check your specific model on [https://grapheneos.org/releases](https://grapheneos.org/releases)

> Only Chromiun based browsers are supported: Chromium (outside Ubuntu), Vanadium, Google Chrome, Microsoft Edge, Brave (without Shields enabled). Do not use incognito mode on the browser

> Almost every major OS is supported but you can check yours in [https://grapheneos.org/install/web#prerequisites](https://grapheneos.org/install/web#prerequisites)

<br>
First, the OEM unlocking option needs to be enabled from within the phone's operating system. To do this, enable the Developer options menu: go to **Settings > About phone/tablet** and tap the **Build number** menu entry until you see a message confirming that developer mode is enabled. Then, navigate to **Settings > System > Developer options** and enable **OEM unlocking**. (On some devices, you must be connected to Wi-Fi to enable this feature, as it checks if the phone has been reported as stolen.) (**Verizon Pixel phones cannot** have their bootloader unlocked, which is a requirement for installing GrapheneOS.)



Next, boot the phone into the bootloader interface. Reboot the phone and hold the volume down button. (On some Windows systems, you may need to install [fastboot drivers](https://grapheneos.org/install/web#connecting-device).)

Now, connect the phone to your computer with a USB-C cable. In your browser, click **[Unlock bootloader](https://grapheneos.org/install/web#unlocking-the-bootloader)**, select your phone in the pop-up window, and click **Connect**. On your phone, you will see **Do not unlock the bootloader** next to the power button. Press the volume up or down button to change the option to **Unlock the bootloader**, then press the power button to confirm.

Click on **[Download release](https://grapheneos.org/install/web#obtaining-factory-images)** to download the GrapheneOS factory images for your device. Once the download is complete, you can click on **Flash release**. This will automatically flash the firmware and wipe all previous data. **Important: Do not interact with the device until the flashing process is finished.**

After the flashing step is complete, click on **Lock bootloader**. This is crucial for the security and integrity of the device. On your phone, you will see **Do not lock the bootloader** next to the power button. Press the volume up or down button to change it to **Lock the bootloader**, then press the power button to select that option. The screen should then display "Device state: locked". Press **Start** by pressing the power button.

> Every time you switch your device on or off, you will see a warning on the screen. This is normal and occurs because you are not running Google's official OS.

&nbsp;

Finally, you just need to complete the initial GrapheneOS setup. For security purposes, you should now disable OEM unlocking again. Go to **Settings > About phone/tablet** and tap the **Build number** menu entry if developer mode isn't already enabled. Then, navigate to **Settings > System > Developer options** and disable **OEM unlocking**. You can now also disable the Developer options menu if you wish.
