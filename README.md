# StarlingType (听打)

> **Dictate in English and 中文 without switching languages.**
> Your voice stays on your Mac.

[![Download](https://img.shields.io/badge/Download-StarlingType%200.1.0-blue?style=for-the-badge&logo=apple)](https://github.com/hungryalgo/starlingtype-releases/releases/latest)
[![macOS](https://img.shields.io/badge/macOS-13.0%2B-lightgrey?style=for-the-badge)](#system-requirements)

**English** · [简体中文](README.zh-Hans.md)

---

## What is this?

StarlingType is a Mac dictation app for bilingual Chinese-English speakers. Say a wake phrase, speak a sentence, and the text appears where your cursor is — even if you mix English and 中文 in the same sentence. Audio never leaves your Mac.

It's named after a starling — a bird famous for vocal mimicry. **听打** (Tīng Dǎ) literally means "listen-type."

## How is it different from Apple Dictation?

|   | StarlingType | Apple Dictation |
|---|:---:|:---:|
| Bilingual English + 中文 in one sentence | ✅ | ❌ |
| Wake-word activated (hands-free) | ✅ | ❌ |
| Works in any text field | ✅ | ✅ |
| 100% local — audio stays on your Mac | ✅ | ✅* |
| Free | ✅ | ✅ |

<sub>*Apple processes some dictation off-device on older models or specific languages.</sub>

## Install (≈1 minute)

1. **Download** `StarlingType-0.1.0.dmg` from the [latest release](https://github.com/hungryalgo/starlingtype-releases/releases/latest).
2. **Open** the `.dmg`, drag **StarlingType** to **Applications**.
3. **First launch only:** right-click the app → **Open** → confirm.
   *(This is a one-time Gatekeeper step because StarlingType is not yet signed with an Apple Developer ID. See [Why the warning?](#why-the-gatekeeper-warning) below.)*
4. Follow the in-app setup wizard. It walks you through microphone access and (optional) cursor-injection permissions.

## How to use it

Once StarlingType is running (you'll see a microphone icon in your menu bar):

**English wake phrases:**
- "Hey Type"
- "Hey Starling"

**Chinese wake phrases (中文):**
- 嘿小听
- 小听小听
- 嘿听打
- 听打听打

Say a wake phrase, hear the **pop** chirp, then dictate. When you stop talking, a **tink** chirp plays and the text appears at your cursor (or on your clipboard — your choice in settings).

Don't feel like talking? Click the **Dictate now** button in the menu bar to skip the wake phrase entirely.

## System requirements

- **macOS Ventura (13.0) or later**
- **Apple Silicon (M1 or newer)** — Intel Macs are not supported (the on-device speech engine ships Apple Silicon binaries only)
- ~450 MB disk (most of which is the on-device speech-recognition model)
- A working microphone

## Privacy

Everything happens on your Mac. There is no cloud transcription, no telemetry that sends audio, and no account to create.

You can verify this yourself by blocking the app from network access (Settings → Network → Firewall, or Little Snitch / LuLu). Dictation still works.

## Known issues in v0.1.0

- **Permissions after an update.** macOS ties permission grants (Microphone, Accessibility) to the app's code signature. StarlingType signs every release with the same identity so your grants normally **carry over across updates** — you shouldn't have to re-grant anything. If a permission does drop after an update, StarlingType detects it on launch and offers a one-click **"Re-run Setup"** to restore it. Manual recovery if you ever need it (~20 seconds, order matters):
  1. Open the gear panel → click **Open Accessibility** (or System Settings → Privacy & Security → Accessibility)
  2. **Select StarlingType** in the list (the row becomes highlighted), then **click the − button at the bottom-left of the list** to remove the entry
  3. **Quit StarlingType** from the popover
  4. Relaunch StarlingType from your Applications folder
  5. Grant the permission when the system prompts you

  **Don't skip the quit + relaunch** — re-adding the entry while the broken version is still running leaves the running process with a cached "denied" state. Best practice if you ever hit this: remove the entry **before** installing the new version.
- **Gatekeeper warns on first launch.** Right-click → Open once; macOS remembers your choice. (See below for the why.)
- **Wake phrase may bleed into your first sentence** if you don't pause briefly. Saying "Hey Type hello world" can transcribe as "Type hello world." Pause ~300ms (the chirp is your cue) and you'll be clean.

## Why the Gatekeeper warning?

StarlingType is not signed with an Apple Developer ID. Apple's Developer Program costs $99/year, and for a free, open-distribution v1.0 we chose to skip it rather than pass the cost on. macOS therefore shows "StarlingType can't be opened because it is from an unidentified developer" on first launch.

Right-click the app → **Open** bypasses this once. macOS remembers your choice afterward.

If StarlingType gets enough use to justify the Developer Program, we'll sign + notarize future builds and this warning goes away.

## Feedback

Have a bug, an idea, or a wake phrase that doesn't detect well in your accent? Email **starlingtype+feedback@gmail.com**.

If you're using StarlingType regularly, a one-line "still using it" message helps decide whether to keep building Mac-first or pivot to Android / iOS / Windows.

## What's next

We have a planned platform sequence — Android (free), then Windows + Linux (free), then iOS (paid, because Apple requires it). None of those are guaranteed; they depend on whether v0.1.0 finds users. If you'd use StarlingType on a platform that isn't Mac, **email us and say so** — that's the strongest signal.

## License

StarlingType is closed-source for v1.0. The full End User License Agreement is included inside the app (menu bar → **Licenses**) and in the [LICENSE](https://github.com/hungryalgo/starlingtype-releases/blob/main/LICENSE) file of this repo.

Third-party components used by StarlingType (Sherpa-ONNX, FunASR/SenseVoice, PyAudio, PortAudio, NumPy, Python) are all permissively licensed (Apache 2.0 / MIT / BSD-3 / PSF). Their full license texts are bundled inside the app and viewable via the **Licenses** menu.

---

<sub>Copyright © 2026 Spec Envoy. All rights reserved.</sub>
