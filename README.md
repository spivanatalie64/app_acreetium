# app_acreetium

**Maintainer:** Natalie (AcreetionOS)  
**Part of:** [AcreetionOS](https://acreetionos.org)

Build scripts, patches, and CI for Acreetium — the Chromium engine for AcreetionOS (WebView provider + browser).

## Structure

```
├── build.sh          Build script (uses chromiumbb)
├── patches/          Patches from Vanadium, LineageOS, Cromite, and custom
│   ├── 0001-Vanadium/
│   ├── 0002-LineageOS/
│   ├── 0003-Cromite/
│   └── 9000-Acreetium/
├── .gitea/           CI/CD workflows
├── trigger-build.txt
└── trigger-release.txt
```

## Prerequisites

- [chromiumbb](https://github.com/spivanatalie64/chromiumbb) — Guile build tool
- [codeberg-tool](https://github.com/spivanatalie64/codeberg-tool) — for Codeberg ops
- Chromium source tree (use `setup-acreetium.sh` in the acreetium project)

## Building

```bash
# From within the Chromium source tree:
./path/to/app_acreetium/build.sh
```

## Patches

Patches are organized by origin and applied in numeric sort order.

## Credits

- Vanadium patches from GrapheneOS (GPL-2.0)
- LineageOS patches (Apache-2.0)
- Cromite patches (GPL-2.0-or-later)
