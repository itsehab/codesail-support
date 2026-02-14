# Privacy Policy

**Effective Date**: February 14, 2026
**App**: CodeSail
**Developer**: Ehab Fayez

## Overview

CodeSail is a mobile companion app for Claude Code. Your privacy is important — the app is designed to collect the minimum data necessary to function and keeps your information secure with end-to-end encryption.

## Data We Collect

### Authentication Credentials
When you pair your device, CodeSail generates a cryptographic key pair and stores an authentication token. These are used solely to authenticate with the relay server and encrypt your messages.

- **Stored locally** in the iOS Keychain (hardware-encrypted)
- **Not shared** with any third party
- **Deleted** when you log out of the app

### Session Data
CodeSail receives session metadata (session name, status, working directory) and encrypted messages from the relay server. Messages are end-to-end encrypted — they are encrypted on the sending device and can only be decrypted by your paired devices.

- **The relay server cannot read your message content**
- Session metadata is used only to display your sessions in the app

### Integration Tokens
If you connect third-party services (Vercel, GitHub, OpenAI, Sentry, Neon, Resend, AWS, Google AI), their API tokens are stored locally in the iOS Keychain. These tokens are used only to fetch data from the respective services and are never sent anywhere else.

### In-App Purchase
CodeSail offers a one-time lifetime purchase. Purchase transactions are handled entirely by Apple through StoreKit. We do not collect or store payment information.

## Data We Do NOT Collect

- No personal information (name, email, phone number)
- No location data
- No contacts or address book data
- No browsing history
- No advertising identifiers
- No analytics or usage tracking sent to external services
- No crash reports sent to third parties

## Third-Party Services

- **Relay Server** (`api.cluster-fluster.com`): Receives encrypted session data for real-time sync between your devices. Cannot decrypt message content.
- **Apple StoreKit**: Handles in-app purchases. Subject to [Apple's Privacy Policy](https://www.apple.com/legal/privacy/).
- **Third-Party Integrations** (optional): When you connect services like GitHub or Vercel, API requests are made directly to those services using your provided tokens. Each service has its own privacy policy.

## Data Storage & Security

- All sensitive credentials are stored in the **iOS Keychain**, which is hardware-encrypted and protected by your device passcode/biometrics.
- Messages use **NaCl (libsodium) secretbox** and **AES-256-GCM** encryption.
- All network communication uses **HTTPS/TLS**.
- Widget data shared via App Groups contains only session status summaries (no message content).

## Data Retention

- All app data is stored locally on your device.
- Logging out deletes all credentials, tokens, and cached data from the device.
- Uninstalling the app removes all locally stored data.
- Session data on the relay server is subject to the relay server's retention policy.

## Children's Privacy

CodeSail is not directed at children under 13. We do not knowingly collect data from children.

## Changes to This Policy

We may update this policy from time to time. Changes will be posted on this page with an updated effective date.

## Contact

If you have questions about this privacy policy, contact us at:
**howdy@codesail.app**
