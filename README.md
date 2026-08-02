<div align="center">

<br/>

<img src="https://img.shields.io/badge/%F0%9F%94%AD_GitSearch-Mobile-63b3ed?style=for-the-badge&labelColor=07090f&color=63b3ed&logo=github&logoColor=white" height="44" alt="GitSearch Mobile" />

<h1>GitSearch Mobile</h1>

<p><strong>The most beautiful, fast, and private way to explore GitHub on Android.</strong><br/>
<em>Discover · Read · Bookmark · Share — No login. No server. No compromise.</em></p>

<br/>

[![Download APK](https://img.shields.io/badge/⬇%20Download%20APK-v1.0.0.2-00C853?style=for-the-badge&logo=android&logoColor=white)](../../releases/latest)

<br/>

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![React 18](https://img.shields.io/badge/React_18-61DAFB?style=flat-square&logo=react&logoColor=black)
![Capacitor 6](https://img.shields.io/badge/Capacitor_6-119EFF?style=flat-square&logo=capacitor&logoColor=white)
![GitHub API](https://img.shields.io/badge/GitHub_REST_API_v3-181717?style=flat-square&logo=github&logoColor=white)
![Privacy](https://img.shields.io/badge/Privacy-100%25_Client--Side-00F0FF?style=flat-square)
![MIT](https://img.shields.io/badge/License-MIT-b794f4?style=flat-square)

<br/>

[**⚡ Download**](../../releases/latest) · [**✨ Features**](#-features) · [**🎨 Themes**](#-6-color-themes) · [**🏆 Why Us**](#-why-gitsearch-mobile) · [**🛡️ Privacy**](#-privacy--security) · [**🔧 Build**](#-build-from-source)

</div>

---

<br/>

## 📸 Screenshots

> **Dark glassmorphic UI · 6 themes · Discover hub · README viewer · Native share**

<div align="center">

| Discover | Search Results | README Viewer | Settings |
|:---:|:---:|:---:|:---:|
| 🔭 Category Cards | 📦 Repo Cards | 📖 Markdown Docs | 🎨 Theme Picker |

</div>

---

## ✨ Features

### 🔭 Discover Hub *(Main Screen)*
Open the app and you're instantly greeted by a rich exploration landing — no blank search box.

- **Hero Card** — tap it to instantly load the world's top trending repos
- **10 Quick Categories** — one tap to explore: 🔥 Trending, 🤖 AI/ML, 🌐 Web Dev, 🦀 Rust, ⚡ APIs, 🐍 Python, 📱 Mobile, 🎮 Games, 🔐 Security, 🐳 DevOps
- **Recent Searches** — tap any past search to re-run it instantly, or swipe to clear

---

### 🔍 Search & Browse
- **Smart search** with inline history suggestions and 1-tap delete
- **Sort by** ⭐ Stars · 🍴 Forks · 🕐 Recently Updated
- **Infinite scroll** — results load automatically as you scroll
- **Language dots**, topic tags, license badges — all visible at a glance

---

### 📖 In-App README Viewer
- Full **Markdown rendering** inside a smooth bottom sheet
- Code blocks, tables, images, blockquotes — all beautifully styled
- **Share** any repo directly from the README viewer

---

### 🔗 Native Android Share
- Tap **🔗 Share** on any card → Android native share sheet opens
- Share to WhatsApp, Telegram, Twitter, Gmail, copy link — whatever you have installed
- Works as expected on every Android device

---

### 🔖 Offline Bookmarks
- Tap 🤍 to save any repo **permanently** on your device
- **No sign-in required** — all local, all private
- Animated badge counter on the nav bar shows your saved count

---

### 👤 GitHub Profile
- Enter your GitHub username once → see your avatar, bio, repo list, followers & following
- Tap any of your repos to read its README in-app
- 1-tap **Edit** to switch profiles anytime

---

## 🎨 6 Color Themes

Switch in **Settings ⚙️** with a sleek compact tile picker:

| | Theme | Vibe |
|---|---|---|
| 🌌 | **Midnight Space** *(default)* | Ice Cyan + Deep Space Blue |
| ⚡ | **Cyberpunk Neon** | Hot Pink + Electric Cyan + Yellow |
| 🌊 | **Deep Ocean** | Aqua Teal + Cool Blue |
| 🌹 | **Midnight Rose** | Ruby Red + Crimson Glow |
| 🖤 | **AMOLED Black** | Pure Black — save battery on OLED displays |
| 🌲 | **Emerald Forest** | Mint Green + Forest Dark |

---

## 🏆 Why GitSearch Mobile?

| | Official GitHub App | Mobile Browser | **GitSearch Mobile** |
|:---|:---:|:---:|:---:|
| No sign-in needed | ❌ | ✅ | **✅** |
| Discover landing hub | ❌ | ❌ | **✅** |
| In-app README viewer | ❌ | ❌ | **✅** |
| Native Android share | ❌ | ❌ | **✅** |
| 6 custom dark themes | ❌ | ❌ | **✅** |
| Search history suggestions | ❌ | ❌ | **✅** |
| Offline local bookmarks | ❌ | ❌ | **✅** |
| 100% client-side privacy | ❌ | ❌ | **✅** |
| AMOLED battery saver theme | ❌ | ❌ | **✅** |

---

## 🛡️ Privacy & Security

GitSearch Mobile is **100% serverless and client-side**:

- 🔒 **Zero tracking** — no analytics, no telemetry, no data collection whatsoever
- 💾 **Local only** — bookmarks, search history, profile, and theme live strictly on your device
- 🌐 **Direct API** — every request goes straight from your phone to `https://api.github.com` over HTTPS
- 🚫 **No backend** — there is no relay server, no proxy, no middleman

---

## 📥 Install the APK

```
1. Tap "Download APK" above
2. Open the .apk file on your Android phone
3. Tap Install (allow "Install from unknown sources" if prompted)
4. Launch GitSearch — enjoy!
```

> 💡 **First time?** Go to **Settings → Security → Install Unknown Apps** and allow your browser or file manager.

---

## 🔧 Build From Source

> **Prerequisites:** Node.js 18+, JDK 17+, Android Studio + Android SDK

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/GitSearch-Mobile.git
cd GitSearch-Mobile

# Install dependencies
npm install

# Run in browser (dev preview)
npm run dev

# Build & sync to Android
npm run build:android

# Compile APK
cd android
.\gradlew.bat assembleDebug

# Output:
# android/app/build/outputs/apk/debug/app-debug.apk
```

---

## ❓ FAQ

<details>
<summary><strong>Do I need a GitHub account?</strong></summary>
<br>
No. Search, browse, read READMEs, share repos, and save bookmarks — all without any account.
</details>

<details>
<summary><strong>How does the Share button work?</strong></summary>
<br>
Tapping <code>🔗 Share</code> calls the native Android share system, so you can send any repository link to WhatsApp, Telegram, Email, or copy it — exactly how sharing works in any other Android app.
</details>

<details>
<summary><strong>Are my bookmarks private?</strong></summary>
<br>
Yes. Everything is stored in your device's <code>LocalStorage</code>. Nothing leaves your phone. Uninstalling the app will remove saved data.
</details>

<details>
<summary><strong>What Android version is required?</strong></summary>
<br>
Android 6.0 (API 23) or higher is recommended for the best Capacitor WebView experience.
</details>

---

## 👨‍💻 Developer

<div align="center">

| | |
|---|---|
| **Developer** | Kizar |
| **Support** | [rkkizar777@gmail.com](mailto:rkkizar777@gmail.com) |
| **License** | [MIT](LICENSE) |
| **Built with** | React 18 · Capacitor 6 · GitHub REST API v3 |

</div>

---

<div align="center">

Built with ❤️ by **Kizar**

[⬆ Back to top](#gitsearch-mobile)

</div>
