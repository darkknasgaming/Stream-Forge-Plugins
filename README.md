# Stream Forge Plugins

Official plugin and expansion repository for Stream Forge.

Plugins are optional additions to Stream Forge and are installed separately from the core application.

## Official Plugins

### Forge Avatar

Audio-reactive animated character system for Stream Forge.

Features include:

- Idle animation frames
- Talking animation frames
- Automatic blinking
- Mic-reactive scale/bounce
- Expression images
- Per-scene visibility
- Stream Forge Broadcaster integration

Current release: v0.5.1

## Installation

Plugins may be installed manually or, in future Stream Forge versions, through the built-in activation-code installer.

## Plugin Architecture

Stream Forge Core remains responsible for:

- Program compositor
- Broadcast lifecycle
- Program audio
- Recording
- Native capture
- YouTube / Twitch output

Plugins extend Stream Forge through supported plugin hooks and must not create competing core owners.
