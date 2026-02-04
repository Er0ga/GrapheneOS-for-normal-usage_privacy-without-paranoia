# GrapheneOS for normal usage: privacy without paranoia

This repository aims to provide a simple guide to set up GrapheneOS on Google Pixel devices. It is intended for users who want better privacy and control of their mobile device without sacrificing usability or spending much time.

I created this repo because when I looked for resources on how to set up GrapheneOS, almost every one I found aimed at users with extreme privacy concerns (at the expense of usability). I just wanted a practical, everyday smartphone experience with better privacy and control, without giving up much usability or spending excessive time configuring it.
<br>

---

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

---
## Getting Apps

On Graphene OS you have an app called **App Store** in which there are the GrapheneOS official apps (Auditor, Camera, Info, Messaging, PDF Viewer) , [Accrescent](https://accrescent.app/) and the ones of the Google Ecosystem (mirror) (Android Auto, Google Play Store, Google Play services and Markup).


### App Stores

[F-Droid](https://f-droid.org/): The premier app store for Open Source Android applications, prioritizing privacy and user freedom. The store for Open Source apps that I recomend. Apps cannot deppend on Google Play Services, are checked for security problems before they are added, you can see the permissions and versions of the app... 

[Aurora Store:](https://auroraoss.com/aurora-store) The most popular free and Open Source alternative for Google Play Store, it is an anonymous Play Store client.

[Google Play Store:](https://play.google.com/store/) Google´s official app store, unlike the othe app stores you need to sign in. Some apps can only be installed through this store or will have limitations if they are not installed from here, for example Google Maps, WhatsApp, or banking apps.


**De-Googling Your Apps**

To reduce reliance on big tech companies, consider using privacy-focused alternatives for your daily mobile needs:

**Email:** Use private email providers such as [Proton Mail](https://proton.me/mail) or [Tutanota](https://tutanota.com/). If you already have a Gmail account, opt for an open-source client like [Thunderbird](https://www.thunderbird.net/)  instead of the closed-source Gmail app.

**Browsers:** [Vanadium](https://grapheneos.org/features#vanadium) is a robust option available out of the box on GrapheneOS. [Brave](https://brave.com/) and [Firefox](https://www.mozilla.org/en-US/firefox/mobile/) (with privacy settings adjusted) are also strong alternatives.

**Password Managers:** Choose an open-source password manager like [Proton Pass](https://proton.me/pass) or [KeePassDX](https://www.keepassdx.com/).

**YouTube:** For ad-free, telemetry-free, background running YouTube viewing without an account, you can try [NewPipe](https://newpipe.net/) or if you want almost the same experience but with your account you can try using Youtube on brave.

**Maps:** Organic MapxThere is no open source as good as Google maps from my experience so if 

**Basic Apps:** For essential apps (gallery, calendar, file manager, etc.), check out the [Fossify](https://fossify.org/) repository. These apps are available on Aurora Store and F-Droid.

**Maps:** [Organic Maps](https://organicmaps.app/) and [OsmAnd](https://osmand.net/) are two strong open source alternatives to Google Maps, but in my opinion, they are far from offering a similar experience .

### Additional Notes and Limitations

**Mobile Payment Wallets:** I haven’t found an open-source alternative to Google Wallet that allows contactless payments on GrapheneOS. Google Wallet is not compatible with GrapheneOS. However, if you need a wallet app for storing tickets (bus, plane, concert, etc.), you can try [FossWallet](https://fossify.org/), available on F-Droid and Aurora Store. 


**Android Auto:** I haven’t tested Android Auto on GrapheneOS. According to the official documentation, compatibility may vary. For more information, check the [Android Auto section](https://grapheneos.org/usage#android-auto) on the project’s website.

**GPS:** You won’t be able to use GPS and precise location on any app out of the box. For that, I have the GPS section in this guide.


**Other Recommended Apps**

- **2FA:** [Aegis](https://getaegis.app/), [Ente Auth](https://ente.io/auth), [Proton Auth](https://proton.me/authenticator)
- **Photos:** [Ente Photos](https://ente.io/), [Immich](https://immich.app/)
- **Notes:** [Notesnook](https://notesnook.com/), [Obsidian](https://obsidian.md/), [Cryptee](https://cryptee.com/)
- **Cloud Storage:** [Proton Drive](https://proton.me/drive), [Syncthing](https://syncthing.net/), [Filen](https://filen.io/), [Nextcloud](https://nextcloud.com/)

**Where to Find More Apps**

- [PrivacyTools by Techlore](https://privacytools.techlore.tech/)
- [Privacy Guides](https://privacyguides.org/en/tools/)
- [AlternativeTo](https://alternativeto.net/platform/android/)


---


## Location and GPS

GrapheneOS isolates your location data by default. To get navigation apps working without leaking your IP address or location history to Google, you need to configure the redirection services manually.

#### **1. Enable the Global Location**

Go to **Settings > Location** and enable **Use location**, by default this is turned off. (Unlike standard Android, enabling this does not immediately start sending data to the cloud)

#### **2. Configure Privacy Proxies**

Tap on **Location services**.

- Set  **Secure User Plane Location (SUPL)** and **Predicted Satellite Data Service (PSDS)** to **GrapheneOS proxy**.
- Ensure **Network location** and **Geocoder** are also using the **GrapheneOS proxy**.

This redirects your device's requests through a proxy server. The external servers (like Google’s or Qualcomm’s) will see the proxy's IP address instead of yours, allowing you to get a GPS lock without showing your location.

#### **3. Disable Background Scanning**

In the same **Location services** menu, I recommend disabling **Wi-Fi scanning** and **Bluetooth scanning**.

On standard Android, these are on by default "to improve accuracy", but they constantly broadcast signals to nearby devices even when you aren't using them. Turning this off prevents this passive tracking and improves battery life.

#### **4. App Permissions**

When you open a map application (like Organic Maps) for the first time:

- Select **Allow only while using the app**. (Don´t select "Allow all the time" if you want to prevent background usage).

- Make sure **Use precise location** is toggled **ON** if you need turn-by-turn navigation.

### Google Maps
To use **Google Maps** normally on GrapheneOS—beyond the settings outlined in the **Location and GPS** section—you must install **Google Play Store** and **Google Play Services** from the GrapheneOS **App Store**.

1. After installing **Google Play Services**, go to **Settings > Apps > Google Play Services** and enable:
    
    - **"Allow background activity"**
    - **"Allow network access"**
2. Install **Google Maps** from the Google Play Store.
    
    - When you first open the app, grant it **location permissions** and **precise location** (select **"Allow only while using the app"**).

---
