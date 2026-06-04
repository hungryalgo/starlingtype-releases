# StarlingType for Android — Setup & User Guide

> Dictate in English and 中文 without switching languages. Everything runs on your phone.

**English** · [简体中文](guide-android.zh-Hans.md) · [← Back to README](../README.md)

---

## Contents
1. [Install](#1-install)
2. [First-run setup](#2-first-run-setup)
3. [The three ways to dictate](#3-the-three-ways-to-dictate)
4. [Wake words](#4-wake-words)
5. [Settings](#5-settings)
6. [Switching to the StarlingType keyboard](#6-switching-to-the-starlingtype-keyboard)
7. [Language (English / 中文)](#7-language-english--中文)
8. [Troubleshooting](#8-troubleshooting)

---

## 1. Install

StarlingType for Android is distributed as a direct `.apk` download (it's not on the Play Store yet).

1. On your phone, open the [latest Android release](https://github.com/hungryalgo/starlingtype-releases/releases/tag/android-v0.1.0) and download **`StarlingType-Android-0.1.0.apk`**.
2. Tap the downloaded file. Android will ask permission to **install unknown apps** for your browser (or Files app) — allow it once, then continue.
3. Tap **Install**, then **Open**.

> This "install unknown apps" step is normal for apps distributed outside the Play Store. You only do it once.

**Requirements:** Android 8.0 or newer. About **280 MB** is downloaded on first run for the on-device speech models (best on Wi-Fi). Works on phones and foldables.

---

## 2. First-run setup

When you open StarlingType the first time, a short wizard walks you through everything:

1. **Welcome** — a quick intro.
2. **Download speech models (~280 MB)** — tap **Download**. This is one-time; best on Wi-Fi. Wait for "✓ Models installed."
3. **Microphone** — tap **Allow microphone**. StarlingType only listens while you're dictating, and audio never leaves the phone.
4. **Enable the keyboard** — tap **Enable keyboard**, turn **StarlingType** on in the system list, then come back. *(This is needed only for the "type into any app" method — see [section 6](#6-switching-to-the-starlingtype-keyboard).)*
5. **You're all set** — tap **Finish**. You'll land on the home screen.

You can re-run this any time from **Settings → Re-run setup**.

---

## 3. The three ways to dictate

StarlingType gives you three ways to dictate. Use whichever fits the moment.

### A. Tap to dictate (zero setup) — copies to clipboard
Best for quickly capturing a thought to paste somewhere.

1. Open the **StarlingType** app.
2. Tap **🎤 Tap to dictate**.
3. Speak after the chirp.
4. Your text is **copied to the clipboard** — switch to any app and paste.

### B. The StarlingType keyboard — types straight into the field
Best for writing directly inside another app (messages, email, notes).

1. In any app, tap a text field so a keyboard appears.
2. **Switch to the StarlingType keyboard** (see [section 6](#6-switching-to-the-starlingtype-keyboard)).
3. Tap **🎤 Dictate** and speak → the words are **typed into the field**.
4. There's also a **⌨ Switch keyboard** button to go back to your normal keyboard.

> The StarlingType keyboard is **voice-only** (no letter keys). Keep your usual keyboard as your default and switch to StarlingType just for dictation.

### C. The Quick Settings tile — hands-free, from anywhere
Best for hands-free dictation. This is the **only way to use wake words without opening the keyboard.**

1. Add the **StarlingType** tile to Quick Settings (the panel you swipe down from the top). The easiest way: in the app, **How to use → Add Quick Settings tile** → confirm.
2. Tap the tile to turn it **on** — StarlingType now listens in the background.
3. Say a **wake word** (see below), then speak.
4. Your text is **copied to the clipboard** to paste.
5. Tap the tile again to turn it off.

---

## 4. Wake words

A wake word tells StarlingType "start listening." Say one, then talk.

| English | 中文 |
|---|---|
| "Hey Type" | 嘿小听 |
| "Hey Starling" | 小听小听 |
| | 嘿听打 |
| | 听打听打 |

**Where wake words work:**
- ✅ With the **Quick Settings tile** on (hands-free, from any app).
- ✅ In the **StarlingType keyboard** *if* you enable **Settings → "Listen for wake word while keyboard is open"** (uses more battery).
- For everything else, just **tap** 🎤 — no wake word needed.

> Tip: pause briefly after the wake word (you'll hear a chirp) so the first words of your sentence aren't cut off.

---

## 5. Settings

Open **Settings** from the home screen.

- **Language** — System default / English / 中文 (see [section 7](#7-language-english--中文)).
- **Keyboard copies to clipboard (instead of typing in place)** — *off by default.* Leave it off and the keyboard types straight into the field. Turn it on only if a particular app rejects direct typing; then a **📋 Paste** button appears on the keyboard to insert the text.
- **Audio chirps** — the sounds when recording starts/stops.
- **Haptics** — vibration feedback.
- **Listen for wake word while keyboard is open** — *off by default.* Lets you say a wake word instead of tapping 🎤 while the keyboard is up. ⚠️ Uses more battery (the mic stays on the whole time the keyboard is open).
- **Wake-word sensitivity** — higher = fewer false triggers; lower = easier to trigger. Applies the next time listening starts.
- **Battery optimization** — opens the system screen if you want to keep always-on dictation reliable.

---

## 6. Switching to the StarlingType keyboard

Android only lets **you** (not an app) switch the active keyboard. Two easy ways:

**Easiest:** In the StarlingType app, tap **⌨ Switch to StarlingType keyboard** on the home screen — a system picker pops up; choose **StarlingType**.

**While typing:** Tap the **keyboard icon** that appears in the navigation bar (usually bottom-right) when a keyboard is showing, and choose StarlingType.

> **Samsung phones:** the navigation-bar keyboard icon is often off by default. Turn it on under **Settings → General management → Keyboard list and default → Keyboard button on navigation bar.** Then switching is one tap from any app.

When you're done dictating, use the keyboard's **⌨ Switch keyboard** button (or the same nav-bar icon) to go back to your normal keyboard.

---

## 7. Language (English / 中文)

The whole app — buttons, onboarding, the keyboard, notifications — is available in **English** and **简体中文**.

Change it in **Settings → Language**:
- **System default** — follows your phone's language.
- **English**
- **中文**

The change applies across the app immediately; no restart needed.

---

## 8. Troubleshooting

**The keyboard's mic types nothing.** Make sure **Settings → "Keyboard copies to clipboard"** is **off** (the default) so it types in place. If it's on, dictation goes to the clipboard — tap **📋 Paste** to insert it.

**A wake word does nothing.** Wake words only work with the **Quick Settings tile on**, or with the keyboard open *and* "Listen for wake word while keyboard is open" enabled. Otherwise tap 🎤.

**The "Switch keyboard" button seems unresponsive.** Tap it once and wait a moment for the system picker. If your phone hides the navigation-bar keyboard icon, use the in-app **⌨ Switch to StarlingType keyboard** button instead.

**Models won't download.** You need a network connection for the one-time ~280 MB download. Try Wi-Fi, then **Settings → Re-run setup** to retry.

**Always-on (the tile) has no notification.** If you declined the notification permission, the background service still runs and still copies your dictation to the clipboard — there's just no visible notification. You can grant notifications later in the system app settings.

---

Questions or bugs? Email **starlingtype+feedback@gmail.com**.
