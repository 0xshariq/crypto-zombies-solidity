# cryptozombies-lesson-code

![CryptoZombies](https://user-images.githubusercontent.com/13703497/69648502-c8f3db80-10ae-11ea-9d52-ce4d4bbc426a.jpeg)


## Overview
This repository contains source codes for [Cryptozombies](https://cryptozombies.io/en/) lessons.

The source codes are divided into `courses` and `chapters` as folders and chapters contain Solidity sample codes for each `lesson`.

> _NOTE: Lesson 7, 8, 9 has been removed and currently no source code is available for those lessons._

## How To Use
You can simply clone the project to your local storage with following command:

```
git clone https://github.com/0xshariq/crypto-zombies-solidity.git
```

Or fork it to modify the sample codes for your own study.

If you found any error in the codes while you study, Feel free to submit pull requests or issues.

>_WARNING: Please note that these codes are just sample codes, so DO NOT use them on production._

## License
[![License shields](https://img.shields.io/badge/License-GPL%20v3-blue)](https://www.gnu.org/licenses/gpl-3.0)

This project is licensed under the GNU General Public License v3.0. See the [LICENSE](https://github.com/loomnetwork/cryptozombies-lesson-code/blob/master/LICENSE) file for details.

## Files (Solidity & Frontend)

Below is a quick reference to the main Solidity files and the simple frontend included in this repository. The purpose notes are brief — check the source for full implementation details.

- `zombiefactory.sol` — Core contract for creating new zombies and storing the main zombie data structures (names, DNA, owner mapping, creation logic).
- `zombiefeeding.sol` — Extends the factory with feeding mechanics to interact with other contracts/creatures and to change zombie DNA.
- `zombieattack.sol` — Implements attack/battle mechanics between zombies (win/lose logic, cooldowns, rewards, etc.).
- `zombieownership.sol` — Handles ownership specifics and safe transfer patterns for zombie tokens between players.
- `zombiehelper.sol` — Utility functions for reading/formatting zombie data (e.g., get zombies by owner, helper getters).
- `ownable.sol` — A small access control contract providing an `owner` address and `onlyOwner` modifier commonly used to restrict privileged actions.
- `safemath.sol` — Arithmetic safety helpers (overflow/underflow protection) used by the contracts where needed.
- `erc721.sol` — A simplified ERC-721 interface/implementation used to make zombies ERC-721 compatible (token standards for NFTs).

Folder: `web3-integration-with-frontend/`

- `cryptozombies_abi.js` — ABI export used by the static frontend to interact with deployed contracts.
- `index.html` — Minimal frontend demonstrating how to connect a dApp to the contracts via web3 and display interaction examples.

If you add or remove files, consider updating this list so the README stays accurate.