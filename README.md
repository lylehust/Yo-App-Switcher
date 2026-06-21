# Yo App Switcher

![App Screenshot](YoAppSwitcher.png)

A keyboard-driven app switcher for macOS. Press a hotkey to bring up a floating frosted-glass panel showing all running Dock apps with Vimium-style hint labels — then press the hint key to switch instantly.

## How It Works

1. Press **Option+a** (customizable) to open the switcher panel
2. Each running app gets a hint key label (A, S, D, F, G, H, J, K, L, etc.)
3. Press the hint key to switch to that app
4. Press **Escape** or hotkey again to dismiss

## Features

- **Floating frosted-glass panel** — compact, centered, stays out of your way
- **Vimium-style hints** — home row keys first for fastest reach
- **Customizable hotkey** — change the shortcut in Preferences
- **Adjustable icon size** — 32pt to 128pt slider in Preferences
- **Launch at Login** — toggle in the menu bar
- **Conflict detection** — warns if shortcut conflicts with system shortcuts
- **Menu bar only** — no Dock icon, always running, lightweight
- **Universal binary** — works on Apple Silicon and Intel Macs

## Requirements

- macOS 14 (Sonoma) or later
- **Accessibility permission** (prompted on first launch) — required for reliable app switching

## Installation

1. Launch from Applications
2. Grant Accessibility permission when prompted (System Settings → Privacy & Security → Accessibility)

## Usage

| Action | Default Shortcut |
|--------|-----------------|
| Open switcher panel | Option+a |
| Switch to app | Press the hint key |
| Dismiss panel | Escape/hotkey |
| Preferences | Menu bar → Preferences... (Cmd+,) |

## Version History
**1.05** — App icon update  
**0.2** — Initial release

## Download Link  

https://apps.apple.com/us/app/yoappswitcher/id6778926070?mt=12
