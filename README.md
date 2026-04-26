A simple extension for [Marinara Engine](https://github.com/Pasta-Devs/Marinara-Engine) that allows changing the accent colours of built-in and compatible themes.

## Features:
- Two independent absolute-hue sliders (Accent + Highlight) calibrated to graphics-software convention (0° = red).
- Per-theme defaults computed dynamically from the active theme's base colors via `getComputedStyle`, with live re-anchoring on theme switches.
- Theme-extensible via `--accent-changer-src-*` source variables; SillyTavern integration ships in-box and the same pattern extends to any future visual theme.
- Auto-contrast on `--primary`-using buttons (covers both `--primary-foreground` consumers and the engine's `text-white` hardcodes), tunable via `--accent-changer-fg-threshold`.
- Storage holds absolute hue (theme-stable across switches); CSS holds the relative shift (theme-relative for clean rotation math).
- Settings injected as a toggle button into the extension's own card on Settings → Extensions.