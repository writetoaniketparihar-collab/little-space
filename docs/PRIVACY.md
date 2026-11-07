# Privacy and permissions

## Notes on your Mac

Little Space stores its local notes vault using AES-256-GCM encryption. The encryption key is generated on the Mac and stored in macOS Keychain, rather than alongside the vault. Encryption does not replace a Mac backup or protect an unlocked note from someone who can already use your Mac.

The app does not require a Little Space account and does not include app analytics. Website analytics and payment processing are separate, as described in the [privacy policy](https://littlespace.pro/privacy).

## Optional Apple sync

Sync is optional. When enabled, writing is also copied into Apple Notes and tasks into Apple Reminders. Apple handles iCloud delivery between your devices. Those copies are governed by your Apple account settings and Apple's protections, not just the local Little Space vault.

The app requests automation access to Notes and access to Reminders for this feature. macOS grants broader Reminders access than a single list; Little Space uses its own lists. You can revoke permissions in System Settings under Privacy & Security. Turning off sync stops future syncing; it does not by itself erase existing copies in Apple apps.

## Voice

Voice requires microphone and speech-recognition permissions. Little Space requests on-device recognition and requires a supported language. macOS may need to download language resources from Apple.

## Update checks

Automatic checks are optional and off until enabled. A manual check, or an enabled automatic check, requests the version file at `https://littlespace.pro/version.json` over HTTPS. The request does not include your note text or a Little Space account identifier. The website infrastructure necessarily receives normal connection information such as your IP address. Installing an update remains a manual download through the customer portal.

## Public support

GitHub issues and attachments are public. Use fictional note content when reproducing a bug. Never post your notes vault, Keychain data, account credentials, payment details, receipts or private download links. Review diagnostic logs before sharing them, since errors or file paths can reveal personal details.

For confidential support or security concerns, follow [SUPPORT.md](../SUPPORT.md) or [SECURITY.md](../SECURITY.md).
