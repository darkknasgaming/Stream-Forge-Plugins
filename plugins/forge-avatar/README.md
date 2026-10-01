# Forge Avatar v0.5.1 — Animation-Only Reliability Cleanup

Optional activation-gated Stream Forge plugin supporting:

- **v1.5.1 Alpha 9.4.248 — YouTube Quota Guard Hardening**
- **v1.5.1 Alpha 9.4.249 — Now Playing & Assist Stability**
- **v1.5.1 Alpha 9.4.250 — Twitch Simulcast & Quota Recovery**

v0.5.1 removes the experimental speech systems and keeps the parts that are reliable in real use.

## What remains

- Existing Stream Forge microphone level drives talking frames and scale-to-sound.
- Multiple Idle, Talking and Blink frames.
- Random Auto Blink with configurable interval/duration.
- Program-overlay blink scheduling fix.
- IndexedDB artwork storage and legacy art migration.
- Optional expression image slots with manual **Test** buttons.
- Per-scene Forge Avatar Program source with normal Move / Resize.
- Activation-code unlock and normal Enable / Disable.

## Removed completely

- Chromium SpeechRecognition.
- Language-pack controls.
- Speech-to-text phrase triggers.
- Trainable voice-command matching.
- Voice templates / recognition strictness controls.
- Compatibility microphone fallback.

Forge Avatar does **not** open another microphone. It only observes the existing Broadcaster microphone level.

## Upgrade

You can install v0.5.1 directly over v0.2.x, v0.3.0, v0.4.x or v0.5.0 when the previous plugin's recorded patched hashes still match. The installer restores the previous patch from its safety backup before applying v0.5.1.

Opening Forge Avatar after the upgrade strips old speech/voice-command settings and saved voice templates from the Forge Avatar profile. Your artwork, animation frames and normal reaction settings are retained.

## Activation code

`FAV-7K9M-Q4VX-2RDA`

The activation code remains a discovery/unlock gate, not security.

## Ownership / safety

- Stream Forge Broadcaster remains the microphone/audio owner.
- Forge Avatar is visual-only.
- No second microphone capture, AudioContext, Program compositor, MediaRecorder or Program audio owner.
- `server.js`, `electron-main.js`, `electron-preload.js`, native DXGI/shared-texture transport and YouTube/Twitch lifecycle are not patched.
- Forge Avatar remains disabled per scene by default.

## Runtime proof

Build verification can prove install/uninstall safety, source wiring, animation logic and absence of speech-recognition code. Real blink/talking/Program rendering remains Windows-runtime proof.
