# Stream Forge Plugins

Official plugin and expansion catalog for **Stream Forge**.

Stream Forge Core stays focused on the stable broadcasting platform. Optional features live here as independently versioned plugins that users can install only when they want them.

## Official plugins

### Forge Avatar

Audio-reactive animated character plugin for Stream Forge.

Current release: **v0.5.1 — Animation-Only Reliability Cleanup**

Features include:

- Microphone-reactive talking frames
- Scale-to-sound reaction
- Multiple Idle, Talking and Blink frames
- Random automatic blinking
- IndexedDB artwork storage
- Optional manual expression images
- Per-scene Broadcaster source visibility and Move / Resize
- Activation-code unlock with normal Enable / Disable afterwards

Forge Avatar is visual-only. Stream Forge Broadcaster remains the sole microphone/audio owner.

## Repository layout

```text
Stream-Forge-Plugins/
├── catalog/
│   └── plugin-catalog.json
├── plugins/
│   └── forge-avatar/
│       ├── manifest.json
│       └── README.md
├── .gitignore
├── README.md
└── RELEASE-CHECKLIST.md
```

Source documentation, manifests and the plugin catalog live in Git.

Packaged plugin ZIP files belong in **GitHub Releases**, not normal Git history.

## Distribution model

The long-term Stream Forge plugin flow is:

```text
Activation code / Install in Stream Forge
                ↓
Official plugin catalog
                ↓
Compatible GitHub Release asset
                ↓
Hash / signature verification
                ↓
Atomic install with rollback
                ↓
Persistent unlock
                ↓
Normal Enable / Disable
```

Activation codes are discovery/unlock gates, not DRM or security boundaries.

## Community plugins

Stream Forge is intended to support third-party plugins through a documented, versioned Plugin API/SDK. Community plugins should use supported hooks and declared capabilities instead of modifying protected core ownership directly.
