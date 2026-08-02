<div align="center">

<br />

<img width="120" src="public/logo.png" alt="GitSearch Mobile Logo" />

# 🔭 GitSearch Mobile
### *The Ultimate GitHub App Store & Explorer for Android*

**Discover millions of open-source projects, trending repositories, and developer tools anytime, anywhere.**
*100% Client-Side · Zero Login Required · Serverless · Native Android Share*

<br />

[![Download APK](https://img.shields.io/badge/⬇%20Download%20APK-v1.0.0.2-00C853?style=for-the-badge&logo=android&logoColor=white)](../../releases/latest)

<br />

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![React 18](https://img.shields.io/badge/React_18-61DAFB?style=flat-square&logo=react&logoColor=black)
![Capacitor 6](https://img.shields.io/badge/Capacitor_6-119EFF?style=flat-square&logo=capacitor&logoColor=white)
![GitHub REST API](https://img.shields.io/badge/GitHub_REST_API_v3-181717?style=flat-square&logo=github&logoColor=white)
![Privacy First](https://img.shields.io/badge/Privacy-100%25_Client_Side-00F0FF?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)

<br />

[**⚡ Download APK (v1.0.0.2)**](../../releases/latest) • [**✨ Features**](#-key-features) • [**🎨 6 Themes**](#-6-custom-color-themes) • [**🏆 Comparison**](#-why-gitsearch-mobile) • [**🛡️ Privacy**](#%EF%B8%8F-privacy--security) • [**📥 Installation**](#-quick-installation)

</div>

---

## 🌟 What is GitSearch Mobile?

> **GitSearch Mobile** turns your Android phone into an **interactive Open-Source Discovery Hub**. 

Whether you're looking for cutting-edge AI models, trending Web frameworks, blazing-fast Rust tools, or mobile projects, GitSearch Mobile gives you a native app store experience right on your phone — **without needing a PC, complex setup, or even a GitHub account.**

---

## ✨ Key Features

### 🔭 Discover & Exploration Hub (Main Screen)
- **Interactive Discover Landing View**: Opens straight into a curated discovery dashboard with popular open-source categories.
- **1-Tap Quick Categories**: Instant exploration for **🔥 Trending**, **🤖 AI / ML**, **🌐 Web Dev**, **🦀 Rust**, **⚡ APIs**, **🐍 Python**, **📱 Mobile**, **🎮 Games**, **🔐 Security**, and **🐳 DevOps**.
- **Clickable Hero Discovery**: Tap the main header card anytime to load top trending repositories worldwide.
- **Recent Searches & 1-Tap Delete**: Smart search history with instant tap-to-search or 1-tap delete (`✕`).

### 📖 Rich In-App Documentation
- **Native Markdown README Viewer**: Read full project documentation in a sleek, glassmorphic bottom sheet without leaving the app.
- **In-App Share Button**: Tap `🔗 Share` to instantly invoke the **Native Android System Share Sheet** (WhatsApp, Telegram, Twitter, Messages) or copy the URL with 1-tap fallback.

### 🎨 6 Custom Color Themes
Switch between 6 hand-crafted color palettes in Settings ⚙️ with a compact, ultra-sleek 3-column tile selector:
1. 🌌 **Midnight Space** *(Default Ice Cyan & Deep Blue)*
2. ⚡ **Cyberpunk Neon** *(Hot Pink, Electric Cyan & Yellow Glow)*
3. 🌊 **Deep Ocean** *(Aqua Teal & Ocean Blue)*
4. 🌹 **Midnight Rose** *(Ruby Rose & Crimson)*
5. 🖤 **AMOLED Black** *(True Pure Black for OLED Display Battery Saving)*
6. 🌲 **Emerald Forest** *(Mint Green & Forest)*

### 🔖 Offline Bookmarks & Profile
- **Local Bookmarks**: Tap 🤍 on any repository to save it permanently on your device — zero account required!
- **Badge Counter**: Live animated badge indicator on the bottom nav shows saved repo counts.
- **Inline Profile Setup**: Enter your GitHub username directly inside the Profile tab to inspect public repos, followers, and bio!

---

## 🏆 Why GitSearch Mobile?

| Feature | Official GitHub App | Mobile Browser | **GitSearch Mobile** |
| :--- | :---: | :---: | :---: |
| **No Sign-In Required** | ❌ | ✅ | **✅ (100% Free Access)** |
| **Discover Landing Hub** | ❌ | ❌ | **✅ (Categories & Trends)** |
| **In-App README Viewer** | ❌ | ❌ | **✅ (Smooth Bottom Sheet)** |
| **Native Android Share Sheet** | ❌ | ❌ | **✅ (1-Tap Share)** |
| **6 Ultra-Sleek Color Themes** | ❌ | ❌ | **✅ (AMOLED, Cyberpunk, etc.)** |
| **Instant Search Suggestions** | ❌ | ❌ | **✅ (With 1-Tap Delete)** |
| **Offline Local Bookmarks** | ❌ | ❌ | **✅ (Zero Login Needed)** |
| **100% Client-Side Privacy** | ❌ | ❌ | **✅ (Direct API Calls)** |

---

## 🛡️ Privacy & Security

GitSearch Mobile is built with **100% Client-Side Architecture**:
- 🔒 **Zero Analytics or Tracking**: We do not collect, monitor, or transmit your search history or personal data.
- 💾 **Local Storage Only**: Your bookmarks, history, and theme settings live strictly on your device inside secure `LocalStorage`.
- 🌐 **Direct Connection**: All searches talk directly to `https://api.github.com` via official HTTPS endpoints.

---

## 🛠️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                   📱 GitSearch Mobile APK                   │
│                                                             │
│   ┌─────────────┐   ┌─────────────┐   ┌─────────────────┐   │
│   │ 🔭 Discover │   │ 🔖 Saved    │   │  👤 Profile     │   │
│   └──────┬──────┘   └──────┬──────┘   └────────┬────────┘   │
│          │                 │                   │            │
│          ▼                 ▼                   ▼            │
│   ┌─────────────────────────────────────────────────────┐   │
│   │          Capacitor 6 Android Native WebView         │   │
│   └────────────────────────┬────────────────────────────┘   │
└────────────────────────────┼────────────────────────────────┘
                             │ Direct HTTPS REST API v3
                             ▼
                ┌────────────────────────┐
                │  api.github.com        │
                │  GitHub REST API v3    │
                └────────────────────────┘
                             ▲
                ┌────────────┴───────────┐
                │ 💾 Phone LocalStorage  │
                │ (Bookmarks, History,   │
                │  Theme, Profile)       │
                └────────────────────────┘
```

---

## 📥 Quick Installation

### Standard Android Direct Install
1. Click [**Download APK (v1.0.0.2)**](../../releases/latest).
2. Open the downloaded `.apk` file on your Android device.
3. Tap **Install** *(if prompted, enable "Install from Unknown Sources" for your browser)*.
4. Launch **GitSearch** and start exploring!

---

## 🔧 Build From Source

> **Prerequisites**: Node.js 18+, JDK 17+, Android Studio & SDK.

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/GitSearch-Mobile.git
cd GitSearch-Mobile

# 2. Install dependencies
npm install

# 3. Development live server
npm run dev

# 4. Build web assets & sync with Android Capacitor shell
npm run build:android

# 5. Compile Android Debug APK
cd android
.\gradlew.bat assembleDebug

# Output APK path:
# android/app/build/outputs/apk/debug/app-debug.apk
```

---

## ❓ FAQ

<details>
<summary><strong>Do I need a GitHub account or API token?</strong></summary>
<br>
No! You can search, browse categories, read full README documentation, share repos, and save bookmarks without signing in or setting up any account.
</details>

<details>
<summary><strong>How does native sharing work?</strong></summary>
<br>
Tapping <code>🔗 Share</code> opens your phone's native Android share dialog, letting you send any GitHub repository link straight to WhatsApp, Telegram, Twitter, Messages, or copy the link to clipboard.
</details>

<details>
<summary><strong>Where are my saved bookmarks kept?</strong></summary>
<br>
All saved repositories are stored locally on your device in secure <code>LocalStorage</code>. They are completely private and never uploaded to any server.
</details>

---

## 👨‍💻 Developer & Support

- **Developer**: **Kizar**
- **Support Email**: [rkkizar777@gmail.com](mailto:rkkizar777@gmail.com)
- **License**: [MIT License](LICENSE)

---

<div align="center">

**Built with ❤️ by Kizar using React 18 · Capacitor 6 · GitHub REST API v3**

[⬆ **Back to Top**](#-gitsearch-mobile)

</div>
