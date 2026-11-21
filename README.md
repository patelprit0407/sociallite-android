# 📱 SocialLite – Block Reels & Shorts (Personal Clone)

> **"Keep the social connection. Remove the infinite scrolling."**  
> 100% on-device, private, zero-subscription personal clone for Android.

---

## 🚀 1-Click Direct Download

<div align="center">

### [⬇️ **CLICK HERE TO DOWNLOAD THE LATEST APK (DIRECT LINK)** ⬇️](../../releases/latest/download/SocialLite-latest.apk)

[![Download APK](https://img.shields.io/badge/Download-SocialLite_APK-2ea44f?style=for-the-badge&logo=android&logoColor=white)](../../releases/latest/download/SocialLite-latest.apk)
[![GitHub Release](https://img.shields.io/github/v/release/patelprit0407/sociallite-android?style=for-the-badge&color=blue)](../../releases/latest)

*(Once this repository is on GitHub, the button above will always download the freshest build directly to your phone without browsing files).*

</div>

---

## ⚡ Super Simple Setup (3 Steps)

1. **Download**: Tap the green button above on your Android phone to download `SocialLite-latest.apk`.
2. **Install**: Tap the notification or open your phone's **Downloads** folder, then tap **Install**.
3. **Turn On Protection**:
   * Open **SocialLite**.
   * Tap **"Enable in Accessibility Settings"**.
   * Toggle **SocialLite Anti-Doomscroller** to **ON**.

*(If your phone says "Restricted setting" on Android 13+: Go to Settings -> Apps -> SocialLite -> tap the 3 dots in the top right -> tap "Allow restricted settings").*

---

## 🎯 What SocialLite Does

* **Instagram**:
  * ❌ Blocks the **Reels** tab & full-screen Reels feed.
  * ❌ Blocks the **Explore** grid to stop aimless scrolling.
  * ✅ Keeps **Direct Messages (DMs)** and friend profile chats completely open.
  * 🎯 **Single Reel Support**: Lets you watch one friend-sent Reel from DMs, but automatically blocks swiping down to the next reel.
* **YouTube**:
  * ❌ Blocks the **Shorts** bottom navigation tab.
  * ❌ Auto-exits full-screen Shorts player.
  * ✅ Keeps regular long-form videos, subscriptions, and intentional search intact.
* **Zero Subscriptions & Private**:
  * Runs 100% on-device. No accounts, no data tracking, and no subscriptions.

---

## 🛠️ Project Structure

```
sociallite-android/
├── .github/workflows/build-apk.yml  # Automated cloud APK builder & release generator
├── app/src/main/
│   ├── AndroidManifest.xml
│   ├── res/xml/accessibility_service_config.xml
│   └── java/com/sociallite/blocker/
│       ├── MainActivity.kt               # Jetpack Compose dashboard
│       ├── data/BlockerPreferences.kt     # On-device settings & stat counters
│       └── service/
│           ├── SocialLiteAccessibilityService.kt # Core interception engine
│           ├── InstagramInterceptor.kt   # Reels & Explore blocker
│           └── YouTubeInterceptor.kt     # YouTube Shorts blocker
```
