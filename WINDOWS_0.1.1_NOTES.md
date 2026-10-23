<p><strong>LANTERN</strong> &nbsp; / &nbsp; WINDOWS &nbsp; / &nbsp; 0.1.1</p>

## Meet Lantern for Windows

The first public Windows release with signed automatic update assets.

**[Download for Windows ↗](https://github.com/snacbot/lantern-releases/releases/download/v0.1.1/Lantern-setup.exe)** &nbsp; · &nbsp; Windows release &nbsp; · &nbsp; Windows 10+ · x64

Run the installer, then open Lantern from the system tray.

---

### What changed

- Windows settings and display controls include the latest Mac features, with synchronized network brightness state and corrected slider rendering.
- The installer offers local network control and optional browser admin access, with firewall access limited to private networks and the local subnet.
- Automatic update checks run every 15 minutes while Lantern is running. Enable automatic installation in Settings → About & Updates to download, verify, install, and restart automatically while preserving settings.

Download **[Lantern-setup.exe](https://github.com/snacbot/lantern-releases/releases/download/v0.1.1/Lantern-setup.exe)** for installation. The raw Windows executable, windows-update.json, and windows-update.json.sig are the signed updater package; keep their names unchanged.

Update metadata is signed with the app's pinned Ed25519 key. The installer does not currently have a Windows Authenticode certificate.

### Validation

75 Rust tests, native settings checks, Windows/Mac protocol checks, slider rendering checks, and acceptance/rejection checks for signed and altered update packages.

<details>
<summary>Build reference</summary>

snacbot/lantern commit 24bd87e643da288e9e6341b5c337ba81443bd7e8.

</details>

<details>
<summary><strong>Which download should I choose?</strong></summary>

Choose the setup installer above. The versioned setup file installs the same release. The raw executable, update manifest and signature are used by the automatic updater. A web companion archive, when included, requires Python 3.9 or later.

</details>

---

[All releases](https://github.com/snacbot/lantern-releases/releases) &nbsp; · &nbsp; [Get help](https://github.com/snacbot/lantern-releases/issues) &nbsp; · &nbsp; [Buy Me a Coffee](https://buymeacoffee.com/khaosstudios)

Built by **[Khaos Studios](https://khaosstudio.com/)** · Supported by you.
