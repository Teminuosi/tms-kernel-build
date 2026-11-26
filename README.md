# tms-kernel-build

Build scripts for the macOS Intel (x86_64) build of [fingerprint-chromium](https://github.com/adryfish/fingerprint-chromium) 148.0.7778.215, used as the built-in browser kernel of TMS on Intel Macs.

- Based on [ungoogled-chromium-macos](https://github.com/ungoogled-software/ungoogled-chromium-macos) tag `148.0.7778.215-1.1` (BSD-3-Clause).
- The `ungoogled-chromium` submodule points to fingerprint-chromium tag `148.0.7778.215` (commit `13b89ea`).
- Cross-compiled for `x86_64` on GitHub-hosted Apple Silicon runners (`macos-15`), resumed across chained jobs.
- Changes from upstream: workflow entry (`.github/workflows/build.yml`), output file name, and ad-hoc signing instead of Developer ID signing + notarization (same as the official fingerprint-chromium arm64 dmg).
- Finished disk images are published in [Teminuosi/tms-kernel-dl](https://github.com/Teminuosi/tms-kernel-dl).

License: see `LICENSE` (BSD-3-Clause, from ungoogled-chromium-macos) and the licenses of Chromium / fingerprint-chromium.
