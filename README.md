# Money Manager V4 — Android beta

**Closed-source APK distribution only.** This repository provides the official compiled APK and user documentation, not application source code or an open-source license.

## Download

[Beta releases](https://github.com/nafiz51/money-manager-v4/releases) · [0.1.6 Beta1](https://github.com/nafiz51/money-manager-v4/releases/tag/v0.1.6-beta.1)

Version0.1.6 / Android versionCode26. Requires Android6(API23)+ and a current WebView. Accepted on Vivo Y20/Android12; other devices are not fully qualified.

## Features

- Offline accounts, opening balances, income, expenses and transfers.
- Lending/borrowing, partial/full settlements, linked reversals and history.
- Monthly reports, light/dark themes and display-currency preference.
- Local V2 backup/restore and optional Google Drive backup features.

## Install and update

Download the APK and checksum from Releases and verify SHA-256 before installing. Existing users: privately retain a current V2 backup, then install over the existing app. **Do not uninstall or clear app data.** Stop if Android rejects a signature/update; do not bypass it. The beta uses the existing Money Manager test-build certificate and was accepted as an in-place update on the maintainer's Vivo Y20.

```text
9fe782766ef0c88694cd994981644c5fb6151708d95615014ce01f3cabb5c528  money-manager-v4-0.1.6-v26-beta.apk
```

## Important beta limitations

- Currency selection changes **display formatting only**, without conversion; numerical amounts remain unchanged. The ledger/backups remain **BDT-denominated**, with two decimal places.
- V2 backup files are **plaintext**. Store them privately; checksums detect accidental corruption, not malicious reading/modification.
- **Restore replaces the entire ledger, not merges it.** Keep a recovery copy, verify the intended file and type CONFIRM only when ready. Later changes are lost; automatic backup is disabled pending review after restore.
- Backup limits remain100,000 total rows,16MiB plaintext and24MiB file. Very old encrypted exports require the original-passphrase offline conversion workflow.
- **Backup V3 is not available.** No unlimited-capacity, universal financial-correctness or complete-device-compatibility guarantee.
- Google Drive features have historical device evidence but were **not freshly retested in final beta acceptance**. Google/network access is optional for Drive, not local finances; Android background scheduling is not exact.

## Report a bug

[Open an issue](https://github.com/nafiz51/money-manager-v4/issues) with app version, Android/device version, steps, expected/actual behaviour and visible error text. Use fictional examples and redact screenshots. **Never attach financial backups/databases, private account information, OAuth tokens, signing keys or passwords.** If data integrity seems wrong, stop further writes and retain a private recovery copy.
