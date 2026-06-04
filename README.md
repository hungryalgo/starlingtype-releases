# StarlingType (听打)

> **Dictate in English and 中文 without switching languages.**
> Your voice never leaves your device.

**English** · [简体中文](README.zh-Hans.md)

[![macOS](https://img.shields.io/badge/macOS-Download%200.1.1-blue?style=for-the-badge&logo=apple)](https://github.com/hungryalgo/starlingtype-releases/releases/tag/v0.1.1)
[![Android](https://img.shields.io/badge/Android-Download%200.1.0-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/hungryalgo/starlingtype-releases/releases/tag/android-v0.1.0)

---

## What is this?

StarlingType is a voice-to-text dictation app for **bilingual Chinese–English speakers**. Speak a sentence — mixing English and 中文 freely — and the words appear as text. Everything runs **on your device**; audio is never uploaded.

It's named after the starling, a bird famous for vocal mimicry. **听打** (Tīng Dǎ) literally means "listen-type."

- 🗣️ **Bilingual in one sentence** — say "我们 schedule 一个 meeting" and it just works.
- 🔒 **100% on-device** — no cloud, no account, no telemetry that sends audio.
- 🆓 **Free.**

---

## Choose your platform

### 🍎 macOS

Dictate into any text field on your Mac with a wake phrase or a click.

**Quick version:** Say a wake phrase ("Hey Type" / 嘿小听), speak, and the text lands at your cursor. Or click **Dictate now** in the menu bar to skip the wake phrase.

➡️ **[Download for macOS 0.1.1](https://github.com/hungryalgo/starlingtype-releases/releases/tag/v0.1.1)** · **[Full setup guide →](docs/guide-macos.md)**

Requires macOS 13+ on Apple Silicon (M1 or newer).

### 🤖 Android

Three ways to dictate, so you can pick what fits the moment:

1. **Tap to dictate** — open the app, tap the big button, speak → text is copied to your clipboard to paste anywhere. *(Zero setup.)*
2. **The StarlingType keyboard** — switch to it in any app and tap 🎤 → text is typed straight into the field.
3. **The Quick Settings tile** — for **hands-free wake-word** dictation from anywhere → text goes to your clipboard.

> **Wake words** ("Hey Type" / 嘿小听 …) work hands-free only when the **Quick Settings tile** is on, or while the StarlingType keyboard is open with the optional setting enabled. Otherwise, just tap.

➡️ **[Download for Android 0.1.0](https://github.com/hungryalgo/starlingtype-releases/releases/tag/android-v0.1.0)** · **[Full setup guide →](docs/guide-android.md)**

Requires Android 8.0+. A one-time ~280 MB speech-model download on first run. UI available in English and 简体中文.

---

## Privacy

Everything happens on your device. There is no cloud transcription, no telemetry that sends audio, and no account to create. You can verify it by turning off the network and dictating anyway — it still works.

## Feedback

Found a bug, have an idea, or a wake phrase that doesn't detect well in your accent? Email **starlingtype+feedback@gmail.com**. If you use StarlingType regularly, even a one-line "still using it" helps decide what to build next.

## What's next

Planned sequence: Android (now), then Windows + Linux, then iOS. What gets built depends on whether StarlingType finds users — if you'd use it on a platform it's not on yet, **email and say so**.

## License

StarlingType is closed-source for v1.0. The full EULA is in [LICENSE](LICENSE) and bundled inside each app. Third-party components (Sherpa-ONNX, FunASR/SenseVoice, PyAudio, PortAudio, NumPy, Python) are permissively licensed (Apache 2.0 / MIT / BSD-3 / PSF); their full texts are bundled inside the apps.

---

<sub>Copyright © 2026 Spec Envoy. All rights reserved.</sub>
