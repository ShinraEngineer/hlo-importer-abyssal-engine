<div align="center">

  # HeroLab to Foundry, Powered by Abyssal Engine

  *A Foundry VTT module that imports Hero Lab Online characters directly into Pathfinder 2e and Starfinder 2e games, using HLO's official Public API.*

  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
  [![Foundry V14](https://img.shields.io/badge/Foundry-V14.361-purple)](https://foundryvtt.com)
  [![PF2e](https://img.shields.io/badge/system-pf2e-blue)](https://github.com/foundryvtt/pf2e)
  [![SF2e](https://img.shields.io/badge/system-sf2e-blue)](https://foundryvtt.com)
  [![Ko-Fi](https://img.shields.io/badge/Ko--Fi-Support-ff5e5b)](https://ko-fi.com/adamantiteadventurer)

</div>

---

## About this repository

This repository is the public home for bug reports and feature requests for the **HeroLab to Foundry (Powered by Abyssal Engine)** Foundry VTT module. The module itself is distributed through [shinra.cc](https://shinra.cc/hlo-importer-abyssal-engine/) and the Foundry package registry. Source files are not hosted here.

If you found a problem or have an idea, please open a GitHub issue using the templates provided. That is the fastest way for me to see it and act on it.

## What the module does

The module imports Hero Lab Online characters into Foundry VTT for Pathfinder 2e and Starfinder 2e. Three input modes feed the same parser:

- **HLO Public API**, using an element token plus your user token, so the character pulls down live
- **Pasted JSON**, for when you already have a portfolio export on the clipboard
- **Uploaded JSON file**, for batched imports from a saved export

The conversion logic runs entirely inside the module. There is no third-party hosted service in the critical path, which is the key reliability lesson from the previous generation of HLO importers.

## Install

| | |
|---|---|
| **Module manifest URL** | `https://shinra.cc/hlo-importer-abyssal-engine/module.json` |
| **Foundry listing** | submitted and pending review, username `shokotsu` |
| **Foundry compat** | V14 verified (14.361), V13 supported as a fallback |
| **Target systems** | `pf2e`, `sf2e` |

Paste the manifest URL into Foundry's *Install Module* dialog, or wait for the official Foundry package listing to go live and install from there.

## Reporting bugs and requesting features

Use the GitHub Issues tab on this repository:

- **Bug report:** [open a bug report](https://github.com/ShinraEngineer/hlo-importer-abyssal-engine/issues/new?template=bug_report.yml)
- **Feature request:** [open a feature request](https://github.com/ShinraEngineer/hlo-importer-abyssal-engine/issues/new?template=feature_request.yml)

For a bug report, the most helpful thing you can include is the in-Foundry conversion log (the module writes one for every import) and the HLO export JSON or the element token you used. If you cannot share those publicly, say so in the issue and I will follow up privately.

## Acknowledgements

This project stands on the shoulders of `zarmstrong/hlo-importer` and its companion conversion service, which served the PF2e Foundry community from 2020 to 2022. The original is dormant. This is a from-scratch reimplementation rather than a fork, but the architecture borrows lessons from 134 versions of the original published changelog.

Hero Lab and the Hero Lab logo are registered trademarks of LWD Technology, Inc. Pathfinder, Starfinder, and associated trademarks are property of Paizo Inc. Foundry Virtual Tabletop is a trademark of Foundry Gaming, LLC. This project is not affiliated with, endorsed by, or sponsored by any of these companies.

## Support and contact

- **Brand home:** [shinra.cc](https://shinra.cc)
- **Ko-Fi:** https://ko-fi.com/adamantiteadventurer (supporting future development is appreciated, not required)
- **Discord:** [shinra.engineer](https://discordapp.com/users/310193940106313729) (direct message)
- **GitHub Issues:** https://github.com/ShinraEngineer/hlo-importer-abyssal-engine/issues

## License

MIT. See [LICENSE](LICENSE).
