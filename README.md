# UnifiedInbox

Open-source Android app aiming to bring email, SMS and phone-call activity into one interface.

## Project status

**Early prototype (0.1.0).** The current app contains the initial Compose interface and demo rows. It does not yet connect to real email accounts, read/send SMS, or access call history.

## Planned features

- Unified timeline for email, SMS and call activity
- IMAP email account support
- Android SMS integration with explicit user consent and required default-app role
- Call history and dialer integration using Android-supported roles and permissions
- Unified contacts and search
- Local-first storage and privacy-conscious design

## Build

Requirements: JDK 17 and Gradle 8.9.

\`\`\`sh
gradle assembleDebug
\`\`\`

The debug APK is generated at \`app/build/outputs/apk/debug/app-debug.apk\`.

GitHub Actions builds the debug APK on pushes and pull requests to \`main\`, and uploads it as a workflow artifact.

## Security and privacy

Do not commit passwords, app passwords, OAuth tokens, private keys, or personal message data. Email authentication should use secure OAuth where supported, or credentials stored only in Android's protected local storage.

## License

This project is licensed under Apache-2.0. See [LICENSE](LICENSE).
