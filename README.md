# Plugin Expert Studio — Official Releases

Official standalone installers and disk images for **Plugin Expert Studio**.

---

## Downloads (Version 2.1.1)

| Platform | Architecture | Installer | Direct Download | SHA256 Checksum |
| :--- | :--- | :--- | :--- | :--- |
| **Windows** | 64-bit (x64) | Setup EXE | [Download Windows Setup (89.1 MB)](https://github.com/futuremintai10-sketch/pluginxpert-studio-releases/releases/download/v2.1.1/PluginXpert-Studio-Setup-2.1.1.exe) | `0ac2e5c25d3f6db5de04081730aa22ba79c30e5693ff0c551626afabdac394d7` |
| **macOS** | Apple Silicon (M1/M2/M3/M4) | DMG | [Download Apple Silicon DMG (125.6 MB)](https://github.com/futuremintai10-sketch/pluginxpert-studio-releases/releases/download/v2.1.1/PluginXpert-Studio-2.1.1-apple-silicon.dmg) | `c1d2af1090d6c6fdfd637bc2e4ca08b64f8fe39e5e2440a2577443df1e6968e1` |
| **macOS** | Intel | DMG | [Download Intel DMG (129.4 MB)](https://github.com/futuremintai10-sketch/pluginxpert-studio-releases/releases/download/v2.1.1/PluginXpert-Studio-2.1.1-intel.dmg) | `0f002b33cb1eabc6964c22a69ef3606a578987d46938cb4af934d93e5196ecfc` |

Checksums file: [`SHA256SUMS.txt`](https://github.com/futuremintai10-sketch/pluginxpert-studio-releases/releases/download/v2.1.1/SHA256SUMS.txt)

---

## Verification

To verify checksums:

```bash
# On macOS / Linux:
shasum -a 256 -c SHA256SUMS.txt

# On Windows (PowerShell):
Get-FileHash .\PluginXpert-Studio-Setup-2.1.1.exe -Algorithm SHA256
```

---

## Installation & Security Notes

- **Source Code Privacy**: This repository is dedicated strictly to compiled production release binaries and verification signatures. Source code is stored exclusively in our private organization repository.
- **macOS Ad-hoc Signing**: This release is ad-hoc signed (`-c.mac.identity="-"`). If macOS Gatekeeper alerts on first launch, either right-click the app in `/Applications` and choose **Open**, or run:
  ```bash
  xattr -cr /Applications/PluginXpert\ Studio.app
  ```
- **Windows Firewall**: On first run or connection test, allow `px-lt-engine.exe` through Windows Defender Firewall using the in-app "Fix Connection" button.
