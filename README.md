# SimPHY — Downloads

**SimPHY** is a physics simulation app for education: build and explore 2D & 3D physics — rigid bodies, joints, circuits, optics and more — with built-in JavaScript scripting to create interactive simulations and games.

🌐 Website: [simphy.com](https://simphy.com) · 📦 **[Download the latest release »](https://github.com/maheshkurmi/SimPHY-releases/releases/latest)**

---

## Which file should I download?

| Your system | Download | How to install |
|---|---|---|
| **macOS** (Apple Silicon) | `SimPHY-x.y.dmg` | Open the DMG and drag SimPHY to Applications. Signed & notarized — no security warnings. |
| **Windows 10/11** (64-bit) | `SimPHY-x.y.z.msi` | Run the installer. If SmartScreen appears, click **More info → Run anyway**. |
| **Windows** (32-bit, older PCs) | `SimPHY-x.y.z-x86.msi` | Same as above. For legacy 32-bit machines — also runs on 64-bit Windows. |
| **Ubuntu / Debian / Mint** | `simphy_x.y_amd64.deb` | Double-click to install, or `sudo dpkg -i simphy_*.deb` |
| **Fedora / RHEL / openSUSE** | `simphy-x.y.x86_64.rpm` | Double-click to install, or `sudo rpm -i simphy-*.rpm` |
| **Any Linux** (no install) | `SimPHY-x86_64.AppImage` | `chmod +x SimPHY-x86_64.AppImage`, then double-click to run. |

No Java installation is required — every package bundles its own runtime.

### Notes

- **Windows SmartScreen**: the Windows installers are not yet code-signed, so SmartScreen may warn on first run. The **More info → Run anyway** flow is expected; you can verify your download against `SHA256SUMS.txt` (below).
- **32-bit edition**: uses the Rhino JavaScript engine instead of GraalJS. Scripts run identically with two limits: no ES6 `class` syntax, and use `for (let x of …)` rather than `for (const x of …)`.
- **Linux**: after installing the deb/rpm, SimPHY appears in your application menu. The AppImage is fully portable — nothing is installed.

## Verifying your download

Each release includes `SHA256SUMS.txt`. To verify:

```bash
# macOS / Linux
shasum -a 256 -c SHA256SUMS.txt --ignore-missing

# Windows (PowerShell)
Get-FileHash .\SimPHY-4.0.msi -Algorithm SHA256   # compare with SHA256SUMS.txt
```

## Support

- Website & documentation: [simphy.com](https://simphy.com)
- Bug reports and questions: [open an issue](https://github.com/maheshkurmi/SimPHY-releases/issues)

---

*This repository hosts release binaries only. SimPHY is © SIMPHY SOFTWARES (OPC) PVT LTD.*
