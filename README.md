# Lantern

**Built by Khaos Studios**

Comfortable screen brightness across your Windows PC and Mac. Lantern lives in
the system tray or menu bar, with controls for individual displays, each computer,
and all connected computers on your local network.

[Releases and downloads](https://github.com/snacbot/lantern-releases/releases) ·
[Support Lantern](#support-lantern)

## Downloads

Public installers are being prepared. No public app binaries have been released yet.
When available, official downloads will appear on the
[Releases page](https://github.com/snacbot/lantern-releases/releases).

| App | Platform | Release format |
| --- | --- | --- |
| Lantern for Windows | Windows 10 or later, x64 | Windows installer |
| Lantern for Mac | macOS 13 or later, Apple Silicon and Intel | Signed, notarized DMG |

These are the build targets. Compatibility testing across the supported systems
is still in progress. This repository contains public release information and
download assets; source development is maintained separately.

## What Lantern does

- Adjust a single display, every display on one computer, or your connected computers together.
- Combine monitor brightness controls with software dimming where supported.
- Dim DisplayLink displays even when the dock does not expose a hardware brightness control.
- Rename, reorder or hide displays, and optionally start Lantern when you sign in.
- Restore local screen brightness with the recovery shortcut or the restore button.

Hardware brightness support depends on the monitor, cable and dock. Mac hardware
DDC control requires Apple Silicon; Intel external displays can use software dimming.
Software dimming changes the screen image and requires Lantern to stay running.
It does not switch off the physical backlight. DisplayLink backlight-off has not
been verified, and it is not promised as a supported feature.

## Recovery shortcuts

| Platform | Restore local displays to 100% |
| --- | --- |
| Windows | **Ctrl + Alt + Home** |
| Mac | **Control + Option + Command + R** |

Experimental display power tests are separate from normal brightness controls.
Monitor power behavior varies by hardware.

## Updates

The Mac app includes Sparkle update support with automatic checks, optional
automatic installation, and a manual **Check for Updates…** button. Public
updates will become available after the first signed release and update feed are
published. The Windows app links to this official release page for downloads.

## Support Lantern

Enjoy using Lantern? An optional tip is a way to thank **Khaos Studios** and support
continued development. Tips are voluntary.

**The tip link is being set up.** It will appear here when the studio's payment
page is ready. Both apps link to this section, so the support destination can be
updated without changing the apps.

## Local network and privacy

Lantern shares computer names, display details and brightness state with peers on
your local network. The current native network protocol is unauthenticated and
intended for trusted networks. Do not expose it directly to the internet.

Automatic Mac update checks contact the public GitHub release feed and download
servers. Sparkle system profiling is disabled. Tip payments will take place on
the chosen provider's website; Lantern does not handle card details.

## Reporting a problem

Use [the issue tracker](https://github.com/snacbot/lantern-releases/issues) for
release and compatibility reports. Include your OS version, Lantern version,
monitor model, and cable/dock or DisplayLink setup. Review screenshots and logs
for private computer names and addresses before sharing them publicly.

Please do not post payment details, passwords, or signing credentials in an issue.
