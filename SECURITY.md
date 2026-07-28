# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in Yo App Switcher, please report it privately by emailing **lyle_hust@hotmail.com**. Please do not open a public issue.

You can expect:

- An acknowledgment within 48 hours
- A fix or mitigation plan within 7 days
- Credit in the release notes (unless you prefer to remain anonymous)

## Supported Versions

| Version | Supported          |
|---------|--------------------|
| 1.9+    | Active support     |
| < 1.9   | Best-effort fixes  |

## Security Model

Yo App Switcher is a native macOS menu bar application. It does not transmit data over the network. All processing happens locally on your Mac.

### Permissions Used

| Permission         | Purpose                                              | Required |
|--------------------|------------------------------------------------------|----------|
| Accessibility      | Switch focus to other running applications           | Yes      |
| Input Monitoring   | Global hotkey detection via Carbon Event HotKey API  | No*      |

*The Carbon hotkey API does not require Input Monitoring permission on macOS. Hotkey registration uses a system API that reads key events only when the registered key combination is pressed.

### Data Storage

- **Preferences** (hotkey, icon size, launch-at-login): stored in `UserDefaults`
- **Launch at Login**: managed via `SMAppService` (macOS system service)
- No analytics, no telemetry, no network requests

### Code Signing & Distribution

- Built as a universal binary (arm64 + x86_64)
- Signed with a **Developer ID Application** certificate
- Notarized by Apple for Gatekeeper compliance
- Runs with the `com.apple.security.app-sandbox` entitlement

### Third-Party Dependencies

Yo App Switcher has **zero third-party dependencies**. All functionality is built with macOS system frameworks (AppKit, SwiftUI, Carbon, CoreServices, ServiceManagement).

## Responsible Disclosure

This project follows the principle of responsible disclosure. Security issues reported privately will be addressed before any public announcement. Once a fix is shipped, the vulnerability may be disclosed in the release notes.
