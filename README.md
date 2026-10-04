# Gym

A gym app for Android: build a training plan, log workouts one-handed, and earn badges and ranks along the way.

Made for the **Samsung Galaxy Z Fold8 Ultra** (Android 17, One UI 9). It needs Android 14 or newer. It may work on
other phones, but it has only been tested on the Fold.

This repository holds the release builds only. The source is private.

## Install

1. On the phone, open the [latest release](https://github.com/MazenJ200/gym-app-releases/releases/latest).
2. Under Assets, download `gym-<version>-<commit>.apk`.
3. Open the downloaded file. The first time, Android asks you to allow your browser (or My Files) to install unknown
   apps: allow it, go back, and tap Install. Google Play Protect may warn that it does not recognise Gym (it has never
   been on the Play Store): choose Install anyway.
4. Open Gym, pick a plan (see First start), and follow "Before your first workout" (notifications, battery, and the
   backup folder).

If **Auto Blocker** stops the install (Settings, Security and privacy, Auto Blocker), Samsung is refusing apps from
outside the Galaxy Store and Play Store. Turning it off is your call: it is a security setting.

## Update

From 1.1.0, Gym updates itself: open About (Home, the three dots, About) and tap **Check for updates**. When a newer
version is out, tap Download and install, then:

- The first time only, Android asks you to allow Gym to install updates: turn the switch on, then press Back.
- Tap Update.
- Play Protect warns that it does not recognise Gym: choose **Install anyway**. ("Scan app" would send the app to
  Google; you may, but there is no need.)

Gym saves a backup first, then updates in a couple of seconds with your data as it was. If your phone shows its home
screen afterwards, open Gym again. It never checks by itself: only when you tap.

You can still download the newer APK from Releases and open it: Android updates the app in place and keeps your data.
Or let [Obtainium](https://github.com/ImranR98/Obtainium) watch this repository
(`https://github.com/MazenJ200/gym-app-releases`): it tells you when a new release is out and installs it with one
tap.

**Never uninstall Gym to update it.** Uninstalling deletes everything you logged.

## Your data

Your plans and logs stay on your phone: no account, no server. Gym goes online only when you tap Check for updates,
to read the newest version from this page and download it if you ask. After every workout it writes a backup to
`Download/GymApp/backups/`. Copy that folder off the phone now and then: it is the
only way back if the phone is lost or reset.

## First start

Gym opens on **Pick a plan**: choose one of the templates (Push Pull Legs, Upper/Lower, Full Body, strength programs,
and "Hamzeh Split", the author's own) or start a blank plan of your own. Pick pounds or kilograms at the top of the
same page. The plan you create first becomes your active plan; Plans is where you change it later.

Moving from another phone? "Restore a backup" on the same page brings in a backup from your old phone's
`Download/GymApp/backups/` folder.

(Gym 1.0.0 and earlier started with "Hamzeh Split" already active instead.)

## Check a download (optional)

Each release has a `release.json` beside the APK with the APK's SHA-256. Every build is signed with the same key,
whose certificate SHA-256 is:

```
01:40:24:25:86:60:78:21:F5:D2:E8:7E:6F:F7:F2:F6:45:E5:E3:12:6F:22:E7:04:8D:E9:D0:54:A6:2F:47:45
```

Android refuses an update signed by any other key, so an update can only come from the same author.

## Credits

- Exercise data by RepDB ([repdb.co](https://repdb.co)).
- Illustrations for four exercises: [Everkinetic](https://github.com/everkinetic/data), created by Greg Priday,
  [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), unmodified.
- Muscle map shapes: [body-muscles](https://github.com/vulovix/body-muscles) by Ivan Vulović, Apache License 2.0.
- Number font: [Archivo](https://github.com/Omnibus-Type/Archivo) by Omnibus-Type, SIL Open Font License 1.1.
- Strength ranks: data from the [OpenPowerlifting](https://www.openpowerlifting.org) project (public domain). The DOTS
  formula by Tim Konertz, coefficients from OpenPowerlifting (MIT).
- Templates inspired by GZCLP (Cody LeFever), Starting Strength (Mark Rippetoe), StrongLifts 5x5 (Mehdi Hadim), the
  r/Fitness Basic Beginner Routine, the Reddit PPL (Metallicadpa), 5/3/1 and 5/3/1 Boring But Big (Jim Wendler), and
  PHUL (Brandon Campbell). Their authors are not affiliated with this app.

The full credits and license texts are in the app: Settings, About.

## Terms

Provided as is, with no warranty. The exercise data and images belong to RepDB and are licensed for use inside this app
only: do not extract or redistribute them. Exercise content is informational, not medical advice.
