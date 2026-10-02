# Aural Field

Aural Field is a tiny generative ambient instrument designed to live at the edge of your browser while you work.

It is intentionally small: no account, no samples, no feed, no content to manage. Click the extension icon, press play, and shape a procedural sound world with a handful of controls.

## Why it exists

Most focus-audio products ask you to choose content. Aural Field treats background sound as an object instead: something you can nudge, disturb, and then mostly forget about.

The visual form and the sound share the same parameters, so what you see is not decoration. Density, space, motion, harmonic function, and material all affect both the generative geometry and the synthesis system.

## Interaction

- **Play / pause** starts or stops the generative field.
- **Density** changes event rate, harmonic extensions, overtone count, and visual frequency.
- **Space** changes stereo width, register spread, reverb, delay, and visual amplitude.
- **Motion** changes modulation, detune, harmonic pace, and visual phase.
- **Material** is a 2D timbre surface from soft → bright and pure → grain.
- **Click the field** to drop a note into the current harmonic world.
- **Hover play** to switch harmonic parent functions.
- **New world** generates a new seed, root, and progression.
- **Spacebar** toggles playback.
- **R** generates a new world.

Settings persist between sessions.

## Chrome extension

The repo root is directly loadable as an unpacked Manifest V3 extension.

1. Open `chrome://extensions`
2. Enable **Developer mode**
3. Choose **Load unpacked**
4. Select this repository folder
5. Pin Aural Field

Clicking the toolbar icon opens Aural Field directly in Chrome's Side Panel. It stays available while you move between tabs.

### Permissions

Aural Field requests only:

- `sidePanel` to live in Chrome's side panel
- `storage` for extension-local preferences

It does not read webpages, browsing history, accounts, or personal data. The synthesis runs locally with the Web Audio API.

## Web demo

The same instrument remains the repository's `index.html`, so GitHub Pages can host a full-screen demo without a separate frontend.

## Design principle

**One object, a few forces.**

The goal is for Aural Field to feel closer to a desk object than a media player.
