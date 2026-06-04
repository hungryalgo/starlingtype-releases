# StarlingType for macOS — Setup & User Guide

> Dictate in English and 中文 without switching languages. Your voice stays on your Mac.

**English** · [简体中文](guide-macos.zh-Hans.md) · [← Back to README](../README.md)

---

## Contents
1. [Install](#1-install)
2. [First-run setup](#2-first-run-setup)
3. [How to use it](#3-how-to-use-it)
4. [Wake phrases](#4-wake-phrases)
5. [Settings](#5-settings)
6. [System requirements](#6-system-requirements)
7. [The Gatekeeper warning](#7-the-gatekeeper-warning)
8. [Permissions after an update](#8-permissions-after-an-update)
9. [Known issues](#9-known-issues)

---

## 1. Install (≈1 minute)

1. **Download** `StarlingType-0.1.1.dmg` from the [macOS release](https://github.com/hungryalgo/starlingtype-releases/releases/tag/v0.1.1).
2. **Open** the `.dmg` and drag **StarlingType** into **Applications**.
3. **First launch only:** right-click (or Control-click) the app → **Open** → confirm. This is a one-time step — see [section 7](#7-the-gatekeeper-warning).

---

## 2. First-run setup

A setup wizard runs on first launch and walks you through:

1. **Welcome & privacy** — a quick intro; audio stays on your Mac.
2. **Microphone** — allow it so StarlingType can hear you.
3. **Mode** — *Cursor mode* (recommended) types text at your cursor in any app; *Clipboard mode* copies it for you to paste.
4. **Accessibility / Automation** (cursor mode only) — grant these so StarlingType can insert text where your cursor is. The wizard explains each prompt before it appears.
5. **Live wake test** — try a wake phrase and see "We heard you."
6. **Done** — optionally enable **Launch at login** (recommended, since it's a menu-bar app with no Dock icon).

---

## 3. How to use it

Once running, StarlingType lives in your **menu bar** (a microphone icon).

1. Say a **wake phrase** (see below).
2. Hear the **pop** chirp — that's your cue to talk.
3. Speak your sentence, mixing English and 中文 freely.
4. When you stop, a **tink** chirp plays and the text appears **at your cursor** (or on your **clipboard**, depending on your mode).

Don't feel like talking to it? Click **Dictate now** in the menu-bar panel to dictate without a wake phrase.

---

## 4. Wake phrases

**English:**
- "Hey Type"
- "Hey Starling"

**中文:**
- 嘿小听
- 小听小听
- 嘿听打
- 听打听打

> Tip: pause briefly after the wake phrase (the chirp is your cue). Saying "Hey Type hello world" with no pause can transcribe as "Type hello world."

---

## 5. Settings

Open the gear panel from the menu-bar icon:

- **Mode** — Cursor (type at cursor) or Clipboard (copy to paste).
- **Microphone device** — pick your input by name (survives AirPods connect/disconnect).
- **Wake sensitivity** and **VAD** tuning.
- **Audio chirps** — toggle the pop/tink sounds.
- **Language** — System / English / 中文 for the app's own UI.
- **Launch at login** — keep StarlingType available without opening it each time.
- **Recovery shortcuts** — quick links to the Accessibility/Automation panes if you ever need to re-grant.

---

## 6. System requirements

- **macOS Ventura (13.0) or later.**
- **Apple Silicon (M1 or newer).** Intel Macs are not supported — the on-device speech engine ships Apple-Silicon binaries only.
- ~450 MB disk (mostly the speech-recognition model).
- A working microphone.

---

## 7. The Gatekeeper warning

StarlingType isn't signed with an Apple Developer ID (that program costs $99/year; for a free v1.0 we skipped it rather than pass on the cost). So macOS shows "StarlingType can't be opened because it is from an unidentified developer" on first launch.

**Right-click the app → Open** bypasses this once; macOS remembers your choice afterward. If usage justifies it, future builds will be signed + notarized and the warning disappears.

---

## 8. Permissions after an update

macOS ties permission grants (Microphone, Accessibility) to the app's code signature. StarlingType signs every release with the **same identity**, so your grants **carry over across updates** — you shouldn't have to re-grant anything.

If a permission ever does drop, StarlingType detects it on launch and offers a one-click **Re-run Setup**. Manual recovery (rarely needed, ~20 seconds — order matters):

1. System Settings → Privacy & Security → **Accessibility** (or the gear panel's **Open Accessibility**).
2. **Select StarlingType**, then click the **−** button to remove the entry.
3. **Quit StarlingType.**
4. Relaunch it from Applications.
5. Grant the permission when prompted.

Don't skip the quit + relaunch — re-adding the entry while the old process runs leaves a cached "denied" state.

---

## 9. Known issues

- **Gatekeeper warns on first launch** — right-click → Open once (see [section 7](#7-the-gatekeeper-warning)).
- **Wake phrase can bleed into your first sentence** if you don't pause — pause ~300 ms (the chirp is your cue).

---

Questions or bugs? Email **starlingtype+feedback@gmail.com**.
