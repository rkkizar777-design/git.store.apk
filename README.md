<div align="center">

<br />

<img width="80" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="GitSearch Mobile" />

# GitSearch Mobile

**The fastest, most beautiful way to explore GitHub on Android.**
*No PC. No backend. No login required.*

<br />

[![Download APK](https://img.shields.io/badge/⬇%20Download%20APK-v1.0.0.2-00C853?style=for-the-badge&logo=android&logoColor=white)](../../releases/latest)

<br />

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![React](https://img.shields.io/badge/React_18-61DAFB?style=flat-square&logo=react&logoColor=black)
![Capacitor](https://img.shields.io/badge/Capacitor_6-119EFF?style=flat-square&logo=capacitor&logoColor=white)
![GitHub API](https://img.shields.io/badge/GitHub_REST_API_v3-181717?style=flat-square&logo=github&logoColor=white)
![MIT License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)

<br />

[**Download APK**](../../releases/latest) • [**Features**](#-features) • [**How It Works**](#%EF%B8%8F-how-it-works) • [**Build From Source**](#-build-from-source) • [**FAQ**](#-faq)

</div>

---

## 🌟 Overview

> **GitSearch Mobile** is a lightning-fast standalone Android app that turns your phone into a powerful GitHub exploration tool — completely independent from any PC, server, or backend service.

Whether you're on the bus, in a meeting, or away from your desk, you can instantly search millions of open-source repositories, read full README documentation, bookmark projects for later, and copy Git clone links in one tap.

Built with **React 18**, **Capacitor 6**, and a direct connection to the **GitHub REST API v3**, it delivers a native-grade experience wrapped in a stunning glassmorphic dark UI.

---

## ✨ Features

### 🔍 Search Tab
| | |
|---|---|
| **Quick-Tag Discovery** | 1-tap filters for 🔥 Trending, 🤖 AI/ML, 🦀 Rust, 🐍 Python, 🌐 Web Dev, 🔐 Security, 🎮 Games, 🐳 DevOps |
| **Smart Auto-Suggest** | Past searches appear as you type — delete individual history items with a single tap |
| **Clean Search Titles** | See `🔥 Trending` in the search bar instead of raw query strings like `stars:>5000 pushed:>2024-01-01` |
| **Sort & Filter** | Sort dynamically by ⭐ Stars, 🍴 Forks, or 🕐 Recently Updated |
| **Infinite Scroll** | Results load continuously as you scroll — no pagination buttons |
| **In-App README Viewer** | Read full Markdown documentation in a smooth bottom sheet without leaving the app |
| **1-Tap Clone URL** | Tap `📋 Clone` to instantly copy the Git clone URL to your clipboard |

### 🔖 Saved Tab
| | |
|---|---|
| **Offline Bookmarks** | Save any repository locally on your phone with a single tap — zero sign-in required |
| **Live Badge Counter** | Animated counter badge on the nav bar shows how many repos you've saved |
| **Full Actions** | Open READMEs, copy clone links, and visit GitHub directly from your saved list |

### 👤 Profile Tab
| | |
|---|---|
| **Live GitHub Profile** | Enter your username to load your avatar, bio, follower & following counts |
| **Top Repositories** | Browse your highest-starred repos and tap to view their full README in-app |

### ⚙️ Settings
| | |
|---|---|
| **Token Manager** | Add a free GitHub Personal Access Token to boost your search rate from **10 → 30 req/min** |
| **Username Config** | Set your GitHub handle once and your profile loads automatically |

---

## 🏆 Why GitSearch Mobile?

| Feature | GitHub Mobile App | Mobile Browser | **GitSearch Mobile** |
| :--- | :---: | :---: | :---: |
| Standalone (no PC) | ✅ | ✅ | ✅ |
| Dark glassmorphic UI | ❌ | ❌ | ✅ |
| 1-Tap quick tag search | ❌ | ❌ | ✅ |
| In-app README viewer | ❌ | ❌ | ✅ |
| 1-Tap Git clone copy | ❌ | ❌ | ✅ |
| Search history auto-suggest | ❌ | ❌ | ✅ |
| Offline bookmarks (no login) | ❌ | ❌ | ✅ |
| Skeleton shimmer loaders | ❌ | ❌ | ✅ |
| Smart search response cache | ❌ | ❌ | ✅ |

---

## 🛠️ How It Works

```
┌─────────────────────────────────────────────────────────┐
│                📱 GitSearch Mobile APK                  │
│                                                         │
│   ┌──────────┐  ┌──────────┐  ┌──────────────────┐     │
│   │🔍 Search │  │🔖 Saved  │  │  👤 Profile       │     │
│   └────┬─────┘  └────┬─────┘  └───────┬──────────┘     │
│        │              │                │                 │
│        ▼              ▼                ▼                 │
│  ┌─────────────────────────────────────────────────┐    │
│  │          Capacitor 6 Android WebView            │    │
│  └────────────────────┬────────────────────────────┘    │
└───────────────────────┼─────────────────────────────────┘
                        │ HTTPS / REST API v3
                        ▼
           ┌────────────────────────┐
           │  api.github.com        │
           │  GitHub REST API v3    │
           └────────────────────────┘
                        ▲
           ┌────────────┴───────────┐
           │ 💾 Device LocalStorage │
           │  (Bookmarks, History,  │
           │   Token, Username)     │
           └────────────────────────┘
```

The app works in 3 layers:
1. **GitHub REST API** — All searches and data come directly from GitHub's official API over HTTPS.
2. **Smart Cache** — Queries are cached in memory so navigating back is instant without re-fetching.
3. **Local Storage** — Bookmarks, history, token, and username live permanently on your device.

---

## 🎨 Design System

```
Color Palette
─────────────────────────────────────
Background:  #07090f  (Deep Space)
Cards:       rgba(13,17,32,0.85)  (Translucent Dark)
Accent:      #90cdf4  (Ice Blue)
Gradient:    #90cdf4 → #b794f4  (Blue-Purple Logo)
Stars:       #f6ad55  (Amber)
Forks:       #68d391  (Mint)
Badge:       #fc8181 → #f6ad55  (Red-Orange Gradient)

Typography
─────────────────────────────────────
Font:        Inter (300–900 weight range)
Sizes:       10px labels → 19px logo → 24px headings

Animations
─────────────────────────────────────
Card Entry:  translateY(14px) → 0  (cubic-bezier spring)
Tap Press:   scale(0.985)
Nav Icons:   glow drop-shadow on active state
Loader:      200% shimmer sweep at 1.5s intervals
```

---

## 📥 Installation

### Easiest: Direct APK Download

```
1. Click the green "Download APK" button at the top of this page
2. Open the .apk file on your Android phone
3. Tap Install (allow "Install from unknown sources" if prompted)
4. Launch GitSearch Mobile
```

> **💡 First time?** On Android, go to **Settings → Security → Install Unknown Apps** and allow your browser or file manager.

---

## 🔧 Build From Source

> Requires: **Node.js 18+**, **Java 17+**, **Android Studio** (with Android SDK)

```bash
# Clone
git clone https://github.com/YOUR_USERNAME/GitSearch-Mobile.git
cd GitSearch-Mobile

# Install dependencies
npm install

# Development mode (browser preview with device toolbar)
npm run dev

# Build & sync to Android
npm run build:android

# Compile debug APK
cd android
.\gradlew.bat assembleDebug

# APK output:
# android/app/build/outputs/apk/debug/app-debug.apk
```

---

## ❓ FAQ

<details>
<summary><strong>Does this app need a PC or backend server?</strong></summary>
<br>
No. The APK is 100% self-contained. It talks directly to <code>api.github.com</code> from your phone with no PC, no relay server, and no backend required.
</details>

<details>
<summary><strong>Do I need a GitHub account?</strong></summary>
<br>
No. You can search, view READMEs, bookmark repos, and copy clone links without signing in. A GitHub account is only needed if you want to generate a Personal Access Token for higher rate limits.
</details>

<details>
<summary><strong>What is the search rate limit?</strong></summary>
<br>
Without a token: <strong>10 searches per minute</strong>.<br>
With a free Personal Access Token (Settings ⚙️ tab): <strong>30 searches per minute</strong>.<br>
Tokens are stored only on your device and never sent anywhere except GitHub's official API.
</details>

<details>
<summary><strong>Where are my bookmarks stored?</strong></summary>
<br>
All bookmarks are saved in your phone's native <code>LocalStorage</code>. They are never uploaded to any server. Uninstalling the app will remove them.
</details>

<details>
<summary><strong>Which Android version is required?</strong></summary>
<br>
Android 6.0 (API level 23) or higher is recommended for the best Capacitor WebView experience.
</details>

---

## 📄 License

```
MIT License — Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software.
```

---

<div align="center">

**Built with ❤️ using React 18 + Capacitor 6 + GitHub REST API v3**

[⬆ Back to top](#-gitsearch-mobile)

</div>
