# Lantern

**Built by [Khaos Studios](https://khaosstudio.com/)**

Comfortable screen brightness across your Windows PC and Mac. Lantern lives in
the system tray or menu bar, with controls for individual displays, each computer,
and all connected computers on your local network.

[Releases and downloads](https://github.com/snacbot/lantern-releases/releases) ·
[Support Lantern](#support-lantern)

## Downloads

Lantern 0.1.4 for Windows is available as an
[installer](https://khaosstudio.com/lantern/download/Lantern-setup.exe).
Lantern 0.1.5 for Mac is available as a signed, notarized
[DMG preview](https://khaosstudio.com/lantern/download/Lantern.dmg).
See [Mac preview notes and compatibility limits](https://github.com/snacbot/lantern-releases/releases/tag/mac-v0.1.5).


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

Mac 0.1.5 checks for updates at launch and every 15 minutes while running.
Verified updates download, install and restart Lantern automatically; active
display tests restore first. There are no update opt-out settings. Older saved
opt-outs and skipped versions are cleared when 0.1.5 starts. A dedicated Mac
feed keeps Windows releases independent. The public Mac preview feed is live;
a new release is installed only when it has a higher build number.

Windows 0.1.4 requires automatic checks and installation while running. Older
releases may need their automatic update settings enabled to receive this update.
Both platforms verify signed update assets, preserve settings and restart to
apply updates. Protected installation folders may require system authorization.

## Support Lantern

Enjoy using Lantern? An optional tip is a way to thank **Khaos Studios** and support
continued development. Tips are voluntary.

[Buy Us a Coffee](https://buymeacoffee.com/khaosstudios)

Both apps include a **Buy Us a Coffee** button in Settings that opens the tip page.

## Local network and privacy

Lantern shares computer names, display details and brightness state with peers on
your local network. The current native network protocol is unauthenticated and
intended for trusted networks. Do not expose it directly to the internet.
On Mac, incoming LAN brightness control is off by default, including after an
upgrade. Opt in explicitly in Settings → Network only on a trusted network.
Discovery and local controls still work while it is off; phone control requires
its separate opt-in and pairing key. Windows currently retains its existing LAN
behavior.

Automatic Mac update checks contact the public GitHub release feed and download
servers. Sparkle system profiling is disabled. Tip payments take place on
Buy Me a Coffee's website; Lantern does not handle card details.

## Reporting a problem

Use [the issue tracker](https://github.com/snacbot/lantern-releases/issues) for
release and compatibility reports. Include your OS version, Lantern version,
monitor model, and cable/dock or DisplayLink setup. Review screenshots and logs
for private computer names and addresses before sharing them publicly.

Please do not post payment details, passwords, or signing credentials in an issue.

## Upcoming installation reports

Future Mac and Windows releases will automatically send a one-time installation
report to Khaos Studios’ Discord channel, separately from anonymous usage analytics. It includes the
computer name, approximate state/country, platform, app version and random
installation ID (the PostHog distinct ID when available). No city, coordinates,
IP address or LAN node identifier is sent to Discord. No first-launch prompt is shown.
Existing installations upgrading to this feature may also be reported once.
Current published installers do not contain this feature.
