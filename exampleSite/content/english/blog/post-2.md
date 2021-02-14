---
title: Get Started
date: 2021-02-13T16:22:16-08:00
image: images/showcase/showcase-2.png
description: get started with your new phone how to first step
draft: true

---
# Getting Started

After purchasing your Anon Phone, you'll want to properly set up your new device with the recommended apps and services that will protect your privacy and secure your data. Let's get to work:

Immediately: **_Fit a case and screen protector_**

Sooner or later your new phone will hit the ground or take an inevitable tumble. Protect it with a case and screen protector. It's cheap insurance and you'll thank us later. You can purchase a screen protector and case in our [Product Store](https://app.forestry.io/sites/hwdlor1bbi6ijw/#/sections/all-page-en/examplesite/content/english/products/ "Product Store").

For the Pixel 3a XL I recommend the [Otterbox Symmetry ](https://distracted-ptolemy-1fd198.netlify.app/products/product-5/ "Otterbox Symmetry")case and the [Super Shieldz Screen Protector](https://distracted-ptolemy-1fd198.netlify.app/products/product-5/ "Super Shieldz Screen Protector"). They’re not cheap, but the’re good quality. I fitted mine more than six months ago and they continue to impress me.

## Step 1: Install GrapheneOS

I’m not going to go into any detail about how to install GrapheneOS. The [GrapheneOS installation guide](https://grapheneos.org/install) explains the process well, so follow it and come back here when you’re done.

Once you’ve finished installing GrapheneOS, keep your phone connected to your computer because we’ll be using `adb` at different times throughout the setup process. This will require you to have **USB debugging** toggled to on in **Settings** > **System** > **Advanced** > **Developer options**.

## Step 2: Configure Vanadium

[Vanadium](https://grapheneos.org/usage#web-browsing) is the browser bundled with GrapheneOS.

We want to make sure it can install apps, and set its default search engine.

1. Open the App Drawer by swiping up from the bottom of the screen.
2. Tap the **Settings** icon.
3. Go to **Settings** > **Apps and notifications** > **Advanced** > **Special app access** > **Install unknown apps** > **Vanadium**.
4. Toggle **Allow from this source** to on.
5. Open Vanadium by tapping on the greyscale **Chromium** icon.
6. Inside Vanadium go to **Settings** > **Search engine**, then select **DuckDuckGo**.

## Step 3: Connect to wi-fi

1. Open the Quick Settings menu by swiping down once from the top of the screen.
2. Long-press on the **wi-fi** icon, toggle **Use Wi-Fi** to on, and connect to a wi-fi network.

## Step 4: Install F-Droid

[F-Droid](https://f-droid.org/) is a catalogue of free open-source (FOSS) Android apps. It’s like the [Google Play Store](https://play.google.com/store), but all the apps it contains are FOSS. There are a lot of excellent apps in there – more than I realised before I started using it.

You’ll need F-Droid to install apps later in this guide, and you’ll also need it over time to find and install apps as the need for them arises.

1. In Vanadium, browse to [https://f-droid.org](https://f-droid.org "https://f-droid.org").
2. Tap the **DOWNLOAD F-DROID** button.
3. Tap **Download** in the **Download file** dialog.
4. Tap **OK** in the **This type of file can harm your device** notification.
5. Once the **FDroid.apk** file has downloaded, tap **Open** in the notification.
6. Tap **INSTALL** in the **F-Droid** **Do you want to install this application?** dialog.
7. Tap **DONE** in the **F-Droid** **App installed** dialog.

## Decision 1: Will you use a VPN?

As you set up your phone, there are a few important decisions to make. When we reach each one I’ll flag it and explain what you might want to consider. Whether to use a [VPN](https://en.wikipedia.org/wiki/Virtual_private_network) is your first decision.

If you don’t use a VPN, your mobile/cell carrier will log your use of mobile/cell data, and the ISP of every wi-fi you connect to will log your use of wi-fi data. Increasingly, governments around the world are requiring these logs to be kept, and kept for years, which is a troubling practice.

GrapheneOS will work just fine without a VPN, but in light of this I can’t imagine not using one.

I recommend in the strongest possible terms that you use a VPN and set it to be always-on so that 100% of your internet traffic runs through it.

## Decision 2: Which VPN will you use?

The well-regarded [PrivacyTools](https://www.privacytools.io/) recommends [three VPN services](https://www.privacytools.io/providers/vpn/) and provides a useful summary of what each one offers. All three have no-logging policies, meaning that they undertake not to record your traffic as it goes into and out of their servers.

I use [Mullvad](https://mullvad.net/), partly because it’s one of PrivacyTools recommendations and partly because Mozilla chose them to power [Mozilla VPN](https://vpn.mozilla.org/), which seems like a meaningful stamp of approval.

I find the Mullvad service to be stable and fast. I can recommend it.

A VPN alternative you may come across is the [Orbot](https://guardianproject.info/apps/orbot/) app. It sends traffic through the Tor network, so it doesn’t require you to trust that your VPN truly isn’t keeping logs. I really love the concept of Orbot, but because it uses Tor it slows down browsing to such a frustrating degree that I don’t use it and I don’t recommend it for users who don’t have specific and uncommon privacy needs.

## Step 5: Install the VPN app

Install the app of your VPN service – for me that’s [Mullvad VPN](https://f-droid.org/en/packages/net.mullvad.mullvadvpn/) – via F-Droid, and set it to be always-on.

Alternatively you can install the [WireGuard](https://f-droid.org/en/packages/com.wireguard.android/) app or [OpenVPN for Android](https://f-droid.org/en/packages/de.blinkt.openvpn/) app and load your VPN configurations into them. To me though, that approach is clunkier than it needs to be. Considering that you’re trusting your VPN service with all of your internet traffic, I think it’s reasonable and much more convenient to trust their FOSS app to seamlessly manage your VPN connection.

 1. In F-Droid, find and install **Mullvad VPN**.
 2. In the **F-Droid** **For your security, your phone is not allowed to install unknown apps from the source** dialog, tap **SETTINGS**.
 3. Toggle **Allow from this source** to on, then tap the **back arrow** in the top left corner of the screen.
 4. In the **Mullvad VPN** **Do you want to install this application?** dialog, tap **INSTALL**.
 5. Open Mullvad VPN.
 6. If you already have a Mullvad account, login with your account number. If you don’t have a Mullvad account, tap **Create account** at the bottom of the screen, record your new account number somewhere secure, then tap **Buy credit** at the bottom of the screen and buy credit.
 7. Select the country of the VPN connection you want to use.
 8. Tap **OK** in the **Connection request** dialog.
 9. After a few seconds you should see **SECURE CONNECTION** in green text above the country you chose in the middle of the screen.
10. Tap the **gear** icon in the top right corner of the screen
11. Select **Preferences** and toggle **Auto-connect** to on.
12. Open the App Drawer and tap the **Settings** icon.
13. Go to **Settings** > **Network and Internet** > **Advanced** > **VPN**.
14. Tap the **gear** icon at the right of **Mullvad VPN**
15. Toggle **Always-on VPN** to on.
16. Toggle **Block connections without VPN** to on.
17. Tap **TURN ON** in the **Require VPN connection?** dialog.
18. Open the App Drawer, long-press on **Mullvad VPN**, then tap the **App info** popover which appears.
19. Tap **Notifications** and toggle **Show notifications** to off.

    When notifications are on, you’ll always see a Mullvad icon reminding you that the app is running. The icon appears both on the lock screen and in the notification bar of the home screen. I find this icon distracting, so I prefer not to see it. Don’t feel bad about switching off this app’s notifications because GrapheneOS itself will take care of making sure that the VPN is always on, and will warn you if and when it isn’t.

## Decision 3: How will you block ads?

You can block ads by either:

* setting up system-wide ad-blocking using Private DNS, or
* using a browser with built-in ad-blocking.

Neither option is perfect, and each has different drawbacks.

### Private DNS

You can set **Private DNS** to something like `dns.adguard.com` as described in the [system-wide ad-blocking section of the GrapheneOS FAQ](https://grapheneos.org/faq#ad-blocking).

This will stop ads appearing in your browser(s) and apps. It’s easy and very effective.

The problem with this approach is that the DNS resolver, for example AdGuard, will see every URL your browser and apps try to connect to. This means one more organisation having visibility into your internet use.

To be worth using, I think an ad-blocking DNS resolver would need to be run on a commercial scale, have a robust no-logging policy and be located outside the [Five Eyes](https://en.wikipedia.org/wiki/Five_Eyes). None of the [DNS resolvers listed by PrivacyTools](https://www.privacytools.io/providers/dns/#dns) ticks all these boxes.

Even if you use a VPN, setting a Private DNS will cause all DNS resolution to happen outside the VPN, leaking that information.

The advice from the [custom DNS resolvers section of the GrapehenOS FAQ](https://grapheneos.org/faq#custom-dns) is “If you’re using a VPN, you should consider using the standard DNS service provided by the VPN service to avoid standing out from other users.”

I use a VPN, and I recommend you do, so to me all of this adds up to a convincing argument not to use an ad-blocking DNS resolver.

### Ad-blocking browser

My preferred option is to use an ad-blocking browser.

This has the advantage of allowing your DNS resolution to happen through your VPN (if you use one, and you should), so you’re not leaking your DNS queries.

The problem with it, however, is that it doesn’t block ads in your apps. I find that this isn’t a problem in practice though, because I don’t use any apps which have ads.

## Step 6: Install Bromite

_You can skip this step if you’ve decided to use a DNS resolver for ad-blocking._

[Bromite](https://www.bromite.org/) is a Chromium browser modified with ad-blocking and extra privacy features.

We’ll use it as our default browser.

1. In F-Droid, tap **Settings** > **Repositories**, then tap the **+** button in the top right corner of the screen. You’ll see the **Add new repository** dialog.
2. In Vanadium, browse to [https://bromite.org/fdroid](https://bromite.org/fdroid "https://bromite.org/fdroid").
3. On that page, just below the QR code, you’ll find the address and fingerprint of the Bromite F-Droid repository. Copy and paste them into F-Droid’s **Add new repository** form.
4. Tap **ADD** in the form.
5. Go to the F-Droid **Latest** screen, search for **Bromite**, then install it.
6. Open the App Drawer and tap the **Settings** icon.
7. Go to **Settings** > **Apps & notifications** > **Advanced** > **Special app access** > **Install unknown apps** > **Bromite**.
8. Toggle **Allow from this source** to on.
9. Open Bromite and inside it go to **Settings** > **Search engine**, then select **DuckDuckGo**.

## Step 7: Install Signal

[Signal](https://signal.org/) is a secure messaging app which can seamlessly manage all your messaging, both encrypted messages and conventional texts. It can also make encrypted voice calls.

We’ll use it as a drop-in replacement for the default Messaging app.

 1. In Bromite, browse to [https://signal.org/android/apk/](https://signal.org/android/apk/ "https://signal.org/android/apk/").
 2. Scroll down past the **Danger zone** heading and then tap the **Download** button.
 3. Tap **Download** in the **Download file** dialog.
 4. Tap **OK** in the **This type of file can harm your device** notification.
 5. Once the **Signal-website-univeral-release…apk** file has downloaded, tap **Open** in the notification.
 6. Tap **INSTALL** in the **Signal** **Do you want to install this application?** dialog.
 7. Tap **DONE** in the **Signal** **App installed** dialog.
 8. Go to **Settings** > **Apps and notifications** > **Advanced** > **Special app access** > **Install unknown apps** > **Signal**.
 9. Toggle **Allow from this source** to on.

    Signal needs this permission to be able to update itself.
10. Open the App Drawer by swiping up from the bottom of the screen, long-press on **Signal**, then tap the **App info** popover which appears.
11. Tap **Permissions** and move **Camera**, **Contacts**, **Microphone**, **Phone**, **SMS** and **Storage** from the **DENIED** list to the **ALLOWED** list.
12. Tap the **back arrow** at the top left of the screen.
13. Tap **Notifications** and toggle **Other** to off.

    When this setting is on you’ll see an icon reminding you that Signal is running in the background. The icon appears both on the lock screen and in the notification bar of the home screen. I find this icon distracting, so I prefer not to see it.

## Step 8: Transfer Signal messages from your old phone

_You can skip this step if you don’t have Signal messages that you want to transfer from your old phone._

If you’re already a Signal user and want to transfer your existing Signal messages to this phone, you first need to make a Signal backup following [their instructions](https://support.signal.org/hc/en-us/articles/360007059752-Backup-and-Restore-Messages), then continue on.

_On your computer_

Here’s how I copied the Signal backup directory from my old phone to my computer:

    $ adb pull /sdcard/Signal

Then, from the same directory as the previous command, this copied it onto the Pixel 3a:

    $ adb push Signal /sdcard/

## Step 9: Register and configure Signal

1. Put your SIM card into the phone. Signal needs this to register the new device.
2. Open the Signal app and follow its setup/registration process. If you have a backup to restore, make sure you select the **RESTORE BACKUP** button when it’s presented on the **Restore from backup?** screen.
3. After the registration step in which you enter your name, Signal shows some action confirmations towards the top of the screen in white text on a blue background.
4. Tap the **Use as default SMS app** action confirmation, then select **Signal** in the dialog which appears, then tap **SET AS DEFAULT**.
5. Tap the **Import system SMS** action confirmation.
6. Tap the **x** in the top right corner of the **Invite your friends!** action confirmation.
7. Tap the **Optimize for missing Play Services** action confirmation then tap **ALLOW** in the **Let app always run the background?** dialog.

## Step 10: Install Tor Browser

[Tor Browser](https://www.torproject.org/) is a browser which uses [onion routing](https://en.wikipedia.org/wiki/Onion_routing).

This is the gold standard for private web browsing.

1. In F-Droid, go to **Settings** > **Repositories**.
2. Toggle **Guardian Project** to on.
3. Go to the F-Droid **Latest** screen, search for **Tor Browser** and install it.
4. Open the App Drawer and tap the **Settings** icon.
5. Go to **Settings** > **Apps and notifications** > **Default apps** > **Browser app** then tap **Bromite**.

   Installing Tor Browser unsets the default browser, so this sets it.

## Step 11: Install OsmAnd\~

[OsmAnd\~](https://osmand.net/) is an offline maps and navigation app.

1. In F-Droid, find and install **Maps & GPS Navigation OsmAnd+** (known as OsmAnd\~).
2. Open the App Drawer, long-press on **OsmAnd\~**, then tap the **App info** popover which appears.
3. Tap **Permissions** and move **Location** and **Storage** from the **DENIED** list to the **ALLOWED** list. For **Location**, choose **Only while app is in use**.
4. Open OsmAnd\~.
5. Tap the **GET STARTED** button.
6. Tap **SKIP** on the **Download map** screen, then tap **SELECT** in the **Skip downloading maps** dialog.
7. On the **Map** screens that follow keep selecting your location as the options become more specific.
8. When you see a **Standard map** option, tap it.

   This will download a map for your area. OsmAnd\~ is an offline tool, so it needs to download maps of areas in which it will be used.
9. In the **World overview map** notification which appears next, tap **DOWNLOAD**.

## Step 12: Install Aurora Store

[Aurora Store](https://auroraoss.com/) is a FOSS client for the Google Play Store.

You can use it to install apps which are available for free in the Google Play Store.

1. In F-Droid, find and install **Aurora Store**.
2. Open the App Drawer, long-press on **Aurora Store**, then tap the **App info** popover which appears.
3. Tap **Permissions** and move **Storage** from the **DENIED** list to the **ALLOWED** list.
4. Open the App Drawer and tap the **Settings** icon.
5. Go to **Settings** > **Apps and notifications** > **Advanced** > **Special app access** > **Install unknown apps** > **Aurora Store**.
6. Toggle **Allow from this source** to on.
7. Open Aurora Store.
8. On the **Welcome** screen tap **NEXT**.
9. On the **Accounts** screen tap **ANONYMOUS**.

   This will allow you to install apps without having to authenticate to the Play Store with a Google account of your own.

## Step 13: Add a weather shortcut

As a rule, weather apps just repackage data from national weather services.

Rather than installing a weather app, we’ll go straight to the source and keep it simple by adding a shortcut to the relevant weather service to the home screen.

1. In Bromite, browse to your national weather service, then navigate to the forecast page for your city or region.
2. Tap the **3 vertical dots** icon in the top right corner of the screen and select **Add to Home screen**.
3. In the **Add to Home Screen** dialog, enter `Weather` and then tap **Add**.
4. In the **Add to Home Screen** confirmation dialog, tap **ADD AUTOMATICALLY**.

## Step 14: Remove unused apps from the App Drawer

Some apps which are bundled with GrapeheneOS are unlikely to be used often, so we’ll remove them from the App Drawer to keep it as uncluttered as possible.

One is [Auditor](https://attestation.app/) which verifies the integrity of the operating system.

Others are **Calendar**, **Gallery** and **PDF Viewer**, because in the next step we’ll install alternatives to each of them which have more functionality.

1. Open the App Drawer.
2. Long-press on **Auditor**, then tap the **App info** popover which appears.
3. Tap **FORCE STOP**, then tap **OK** in the confirmation dialog.
4. Tap **DISABLE**, then tap **DISABLE APP** in the confirmation dialog.
5. Repeat this process for **Calendar**, **Gallery** and **PDF Viewer**.

## Step 15: Install other apps from F-Droid

We’ll also install some other apps using F-Droid to provide various functionality.

Search for each one by name in F-Droid, then install it.

After you install each app, open it and approve the permissions it requests.

 1. [AntennaPod](https://f-droid.org/packages/de.danoeh.antennapod/) - Podcast manager and player.
 2. [Feeder](https://f-droid.org/en/packages/com.nononsenseapps.feeder/) - Feed reader.
 3. [Jitsi Meet](https://f-droid.org/en/packages/org.jitsi.meet/) - Video calling.
 4. [KeePassDX](https://f-droid.org/en/packages/com.kunzisoft.keepass.libre/) - Password manager.
 5. [Markor](https://f-droid.org/en/packages/net.gsantner.markor/) - Note taker.
 6. [MuPDF viewer](https://f-droid.org/en/packages/com.artifex.mupdf.viewer.app/) - Document viewer.
 7. [NewPipe](https://f-droid.org/en/packages/org.schabi.newpipe/) - YouTube frontend.
 8. [Simple Calendar Pro](https://f-droid.org/en/packages/com.simplemobiletools.calendar.pro/) - Calendar.
 9. [Simple Gallery Pro](https://f-droid.org/en/packages/com.simplemobiletools.gallery.pro/) - Photo and video gallery.
10. [Syncthing](https://f-droid.org/en/packages/com.nutomic.syncthingandroid/) - Decentralised file synchronisation.
11. [Termux](https://f-droid.org/en/packages/com.termux/) - Terminal emulator.
12. [Voice Recorder](https://f-droid.org/en/packages/com.simplemobiletools.voicerecorder/) - Audio recorder.
13. [VLC](https://f-droid.org/en/packages/org.videolan.vlc/) - Media player.

## Step 16: App settings improvements

### Clock

1. Open the App Drawer and tap the **Clock** icon.
2. Tap the **3 vertical dots** icon in the top right corner of the screen and select **Settings**.
3. Tap **Gradually increase volume** and select **30 seconds**.

   This provides a less jarring experience when waking up to an alarm.
4. Tap **Start week on** and select **Monday**.

   Because the week starts on Monday, not Sunday.

### Jitsi Meet

1. Open the App Drawer and tap the **Jitsi Meet** icon.
2. Tap the **3 horizonal lines** icon in the top left corner of the screen and select **Settings**.
3. Type your first name, nickname or _nom de guerre_ into the **Display name** field.

   This identifies you in a call.
4. Toggle **Start with audio muted** to on.

   If you leave this set to off, sooner or later you’ll find yourself in an awkward situation.
5. Toggle **Start with video muted** to on.

   If you leave this set to off, sooner or later you’ll find yourself in an awkward situation.

## Step 17: Device-wide settings improvements

I find that these modifications to the default settings make the phone feel more natural and more pleasant to use.

 1. **Settings** > **Battery** - Toggle **Battery percentage** to on.

    This displays the battery percentage next to the battery icon in the notification bar at the top of the screen.
 2. **Settings** > **Display** > **Adaptive brightness** - Toggle **Adaptive brightness** to on.

    This makes the screen brightness adapt to the environment, increasing in brighter conditions and decreasing in darker conditions.
 3. **Settings** > **Display** > **Advanced** - Toggle **Auto-rotate screen** to on.

    This rotates the screen when the phone is rotated.
 4. **Settings** > **Display** > **Advanced** > **Lock screen display** - Toggle **Always on** to on.

    This displays basic information and alerts on the screen when the phone is not in use. Switching it on reduces time between charges slightly, but it’s worth it. If you don’t turn this setting on, your phone’s screen will be entirely black when not in use, and the only way to check for alerts will be to wake it up, which gets annoying fast.
 5. **Settings** > **Display** > **Advanced** > **Lock screen display** - Toggle **New notifications** to off.

    This option wakes the screen on new notifications. It’s unnecessary and distracting when **Always on** is enabled, so switch it off.
 6. **Settings** > **Display** > **Advanced** > **Lock screen display** - Toggle **Show lockdown option** to on.

    This adds a **Lockdown** button to the power button menu. This button locks the phone immediately and deactivates fingerprint unlocking. To unlock the phone from this state, the PIN is required. Once unlocked with the PIN, fingerprint unlocking is re-enabled.
 7. **Settings** > **Display** > **Advanced** > **Lock screen display** > **Lift to check phone** - Toggle **Lift to check phone** to off.

    This option wakes the screen when the phone is picked up. I find it unnecessary when **Always on** is enabled, so switch it off.
 8. **Settings** > **Display** > **Night light** - Tap **Schedule** and select **Turns on from sunset to sunrise**.

    The makes the screen colour less blue at night.
 9. **Settings** > **Security** > **Fingerprint** - Tap **Fingerprint + PIN** and follow the prompts.

    This allows the phone to be unlocked with a fingerprint or PIN, which is much more convenient than a PIN alone.

    Enrol the index finger of both hands so you can unlock the phone one-handed with either hand. Now you can touch the fingerprint sensor to wake your phone and unlock it in the one operation.
10. **Settings** > **Sound** > **Advanced** - Toggle all sliders under **OTHER SOUNDS AND VIBRATIONS** to off.

    This makes your phone quieter to use.
11. **Settings** > **System** > **Date & time** - Toggle **Use locale default** to off.

    This needs to be switched off to allow the 24 hour time format to be used.
12. **Settings** > **System** > **Date & time** - Toggle **Use 24 hour format** to on.

    This will show a time as 21:28 rather than 9:28pm throughout the device.
13. **Settings** > **System** > **Gestures** > **System navigation** - Select **Gesture navigation**.

    This provides more expressive gesture navigation.
14. **Settings** > **System** > **Languages & input** > **Languages** - Add **English (Australia)**, then remove **English (United States)**.

    This is what I do, and you should modify this setting for your language.
15. **Settings** > **System** > **Languages & input** > **Virtual keyboard** > **Android Keyboard (AOSP)** > **Appearance & Layouts** > **Theme** - Select **Material Dark**.

    This sets the keyboard to a dark theme which is easier on the eyes than a light theme.
16. **Settings** > **System** > **Languages & input** > **Virtual keyboard** > **Android Keyboard (AOSP)** > **Preferences** - Toggle **Vibrate on keypress** to off.

    This turns off haptic feedback for keypresses on the keyboard.
17. **Settings** > **System** > **Languages & input** > **Virtual keyboard** > **Android Keyboard (AOSP)** > **Text correction** - Toggle **Personalised suggestions** to on.

    This will build up a dictionary of autocomplete suggestions over time based on your personal language use.

## Step 18: Set a wallpaper

I like to set a plain black wallpaper.

The file I use is a 1 pixel by 1 pixel black image called [black.png](https://redandblack.io/blog/2020/how-to-set-up-grapheneos/files/black.png).

_On your computer_

Download the black image file from the link above, then `cd` into the directory you saved it to.

Copy it to the phone with:

    $ adb push black.png /sdcard/Wallpaper/black.png

_On your phone_

1. Go to **Settings** > **Display** > **Wallpaper**, then tap **Wallpapers**.
2. Tap **My photos**.
3. Tap the **3 vertical dots** icon in the top right corner of the screen and select **Show internal storage**.
4. Tap the **3 horizontal lines** icon in the top left corner of the screen then tap **Pixel 3a**, then **Wallpaper**, then **black.png**.
5. Tap **Set wallpaper** at the top of the screen.
6. Select **Home screen and lock screen** in the **Set wallpaper** confirmation dialog.

## Step 19: Configure the Quick Settings menu

1. Swipe down from the top of the phone twice to open the Quick Settings menu.
2. Tap the **pencil** icon in its lower left corner.
3. In the top row, put **Wi-Fi**, **Hotspot**, **Bluetooth**.
4. In the second row, put **Dark theme**, **Location**, **Do Not Disturb**.
5. In the third row, put **Mobile data**, **Battery Saver**, **Aeroplane mode**.
6. In the fourth row, put **Torch**, **Night Light**, **Auto-rotate**.
7. All other icons go in the **DRAG HERE TO REMOVE** section at the bottom of the screen.
8. Tap the **back arrow** at the top left of the screen.

## Step 20: Set up your home screen

 1. For each icon on your home screen, long-press on it, drag it to the far right side of the screen, wait for the next screen with the other app icons on it to appear, then place it on that screen. This will move all the icons to the one screen, and the screen which was to the right of the home screen now becomes the home screen.
 2. Remove **Messages** from the home screen by long-pressing it, dragging it to the **REMOVE** text at the top of the screen and dropping it there. Then do the same for **MuPDF** and **Vanadium**.
 3. Open the App Drawer.
 4. Long-press on **Clock**, drag it upwards and then place it on the home screen. Then do the same with **Files** and **Gallery**.
 5. In the Favourites Bar at the bottom of the screen, beside **Phone** , put **Signal**, **Jitsi**, **Bromite**, and **Camera**.
 6. In the top row of the home screen put the general utility apps: **Calendar**, **Clock**, **OsmAnd\~**, **Voice Recorder** and **Weather**.
 7. In the second row of the home screen put the media apps: **AntennaPod**, **Feeder**, **Gallery**, **NewPipe**, and **VLC**.
 8. In the third row of the home screen put the system utility apps: **Files**, **Markor**, **Syncthing** and **Termux**.
 9. In the fourth row of the home screen put the privacy and security apps: **KeePassDX**, **Mullvad VPN** and **Tor Browser**.
10. In the fifth row of the home screen put the catalogue apps: **Aurora Store** and **F-Droid**.

## Step 21: Set up Seedvault backups

[Seedvault](https://calyxinstitute.org/projects/seedvault-encrypted-backup-for-android) is an encrypted backup app which is bundled with GrapheneOS.

For this step, you’ll need a USB flash drive (with a USB-C adapter) which will be the target for the backup. Ideally it will be at least the same size as your phone’s storage, which for a Pixel 3a is 64GB.

The data which Seedvault backs up doesn’t include your phone’s shared storage, and backups for that will be handled in the next step.

1. Go to **Settings** > **System** > **Backup**
2. A 12-word recovery code is displayed. Record it somewhere secure.
3. Tap the **CONFIRM CODE** button.
4. Enter the recovery code and tap the **DONE** button.
5. Plug the flash drive into the phone.
6. Tap **CANCEL** in the **F-Droid** **Open F-Droid to handle…** dialog.
7. Tap your flash drive’s name on the **Choose where to store backups** screen.
8. Toggle **Backup my data** to **on** on the **Backup** screen.
9. Tap the **3 vertical dots** icon in the top right corner of the screen and select **Backup now** to run your first backup.

## Step 22: Set up shared storage backups

Because Seedvault doesn’t back up the phone’s shared storage, we need to back up shared storage in a separate step.

I recommend backing it up to a second flash drive which is fully encrypted.

1. Plug the flash drive into your computer, then mount and unlock it.
2. Connect the phone to the computer.
3. Copy the phone’s shared storage to the flash drive.

It may not be necessary to do this right now, as you’ve just set your phone up and the amount of data in shared storage is probably minimal. This is a procedure you should carry out regularly from now on though.

I had wanted to be able to recommend a way to back up shared storage directly from the phone into an encrypted container on the same flash drive we used for the Seedvault backup in the step above. I experimented with using the [EDS Lite](https://f-droid.org/en/packages/com.sovworks.edslite/) app to do that, but couldn’t find a way that was simple and robust, so I think the method I’ve recommended is the best for most people.

## Step 23: Deactivate USB debugging

You don’t need to have USB debugging switched on any more, so it makes sense to turn it off now.

1. Go to **Settings** > **System** > **Advanced** > **Developer options** and toggle **USB debugging** to off.

## Do you really need an email app?

This guide doesn’t mention installing an email app because I don’t think it’s something that should be done without careful thought.

Many peoples' email contains a lot of information about them. It can also be used to reset important passwords.

If you lose possession of your phone while it’s unlocked, which is entirely possible given that it’s a device you use in one hand in public places, your email app will be available to the person who finds or takes it.

I’m not saying you shouldn’t install an email app, but I am saying that unless there is a compelling reason for you to have access to email on your phone, consider not installing one.

## Try out other apps too

Many non-FOSS apps with Play Services dependencies can be installed from Aurora Store and will often work with more functionality than you might expect.

If you’re not sure about an app, just try it. You might be pleasantly surprised.

## GrapheneOS is fantastic

I’m thoroughly enjoying the de-Googlified GrapheneOS experience. I’ve been using it for the best part of six months now, and I can’t fault it in any way at all.

I really do feel like at long last I’ve found the holy grail of mobile.