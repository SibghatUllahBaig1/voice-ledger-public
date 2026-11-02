<div align="center">

# 🎙️ Voice Ledger

**Speak a transaction, watch it land in your Google Sheet — instantly. No typing, no forms.**

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=flat-square&logo=googlesheets&logoColor=white)
![RevenueCat](https://img.shields.io/badge/RevenueCat-F2545B?style=flat-square)
![iOS](https://img.shields.io/badge/iOS-000000?style=flat-square&logo=apple&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)

</div>

> 🔒 **Source code is private** (commercial product). This page is a case study of what I designed and built end to end.

---

## 🎯 The problem

People already track expenses, sales and tasks in Google Sheets — but updating a spreadsheet from a phone is slow and fiddly. Entries get delayed, forgotten or skipped, and the data goes stale.

## 💡 The solution

**Voice Ledger** lets you simply *say* what happened — *"Paid 40 for fuel yesterday"* — and the app understands it, maps it to the right columns, and writes a clean row straight into **your own Google Sheet**. Your sheet stays the single source of truth; the app just makes it effortless to keep up to date.

---

## ✨ Key features

| Feature | What it does |
|---|---|
| 🎤 **Voice entry** | Record a sentence; the app parses amounts, dates (including relative ones like "yesterday"), categories and notes. |
| 📊 **Direct Google Sheets sync** | Writes rows to the sheet and tab you choose — no export/import step. |
| 🧩 **Custom rules** | Define how spoken phrases map to your sheet's columns, dropdowns and defaults. |
| 📴 **Offline-first** | Entries are queued locally when there's no connection and synced automatically when it returns. |
| 🕘 **History** | Review, verify and correct what was recorded. |
| 🌍 **Multi-language** | Localized interface and voice input. |
| 💎 **Pro subscription** | Premium features via in-app subscriptions, plus a rewarded-ad option to unlock Pro for a session. |
| 🔔 **Notifications** | Push notifications and subscription status updates kept in sync via webhooks. |
| 🔐 **Google sign-in** | Secure authentication with Google OAuth (verified privacy policy and "Limited Use" compliance). |

---

## 🏗️ Architecture & engineering highlights

- **Feature-first structure** — `auth · voice · ledger · sheets · rules · offline · history · subscription · notifications · locale · settings`.
- **Firebase backend** — Auth, Cloud Firestore, Cloud Functions and Cloud Messaging; hardened Firestore security rules.
- **Smart parsing pipeline** — turns free-form speech into structured rows, with rule-based defaults and fixes for tricky cases like relative dates and free-text dropdown fields.
- **Reliable offline sync** — local persistence (Hive) with a retry queue so no entry is ever lost.
- **Google OAuth & Sheets API** — passed OAuth verification requirements, including Limited Use data-handling wording.
- **Monetization** — RevenueCat subscriptions with webhook-driven entitlement updates; AdMob rewarded ads for Pro-session unlocks.
- **Testable by design** — mocks for Firestore and Auth, plus a test harness for the sheet and offline flows.

## 🧰 Tech stack

**Flutter · Dart · GetX · Firebase Auth · Cloud Firestore · Cloud Functions · FCM · Google Sign-In · Google Sheets API · Hive · RevenueCat · AdMob · App Links · WebView**

---

## 📸 Screenshots & links

<!-- Add screenshots: <img src="screenshots/home.png" width="220"/> -->
<!-- Add store badges once published -->
*Screenshots and demo available on request.*

---

## 🤝 Want an app like this?

I build production-ready mobile apps — voice, automation, Google Workspace integrations, subscriptions and store release — from idea to App Store.

📫 **sibghat.developlogix@gmail.com** · 🌐 **[developlogix.com](https://www.developlogix.com)** · 💼 **[LinkedIn](https://www.linkedin.com/in/sibghat-ullah-baig-4a2812a1)**

<sub>Built by [Develop Logix](https://www.developlogix.com)</sub>
