# Export Padding

Extra time around Ableton Live exports, from a compact Max for Live device.

Place Export Padding on Main, choose Before and After in seconds, and leave **Padding ON**. Select an Arrangement range and open Live's normal Export Audio/Video dialog. The device extends the render bounds to include the surrounding timeline audio. Before and After move in **0.25-second steps** over 0–60 seconds. No companion application is required.

## Free beta

**[Download Export Padding 0.2.0 beta 1](https://github.com/mathewharwich/export-padding-releases/releases/tag/v0.2.0-beta.1)**

Choose the **Export-Padding-0.2.0-beta.1-macOS.zip** release asset. GitHub's automatically generated “Source code” archives contain this repository's public documentation and artwork; they do not contain the device or its proprietary implementation.

This repository distributes official beta downloads and documentation. The source repository remains private. Official beta use is free for personal or professional work under the included Export Padding Beta License. Future releases may be paid. Max for Live devices can be inspected; freezing packages dependencies and is not copy protection.

## Install and use

1. Unzip the download and copy **Export Padding.amxd** into your Ableton User Library.
2. Place one enabled instance on Main.
3. Set Before and After, leave **Padding ON**, and select an Arrangement range.
4. Open **Export Audio/Video**, wait for the adjusted bounds, inspect Render Start and Render Length, and export normally.

Padding OFF or device bypass leaves exports unchanged. Use Ableton's Info View for control guidance.

## Protect tail

Optional **Protect tail** preserves reverb and delay decay, then adds the full After padding beyond the detected tail. A three-second correction plus two seconds of After keeps five seconds past the selected end.

Protection is OFF by default. It requires **Main / Encode PCM ON / WAV / 32-bit / No Dither**, with **MP3, video, Normalize, Render as Loop and Create Analysis File OFF**. Allow the check after rendering to finish before using the WAV. Ordinary fixed padding remains available with protection OFF.

The check captures up to 60 extra seconds and uses a −80 dBFS peak threshold. If the full tail and After interval cannot be confirmed in that range, the longer render is kept. Neighboring clips count as Main audio; noise or infinite feedback can prevent a resolved result. This beta retains hidden raw recovery WAVs beside protected exports, which can occupy substantial disk space. Keep them until the final export has been reviewed; Finder's Command-Shift-period shows hidden files.

## Compatibility

- macOS and Ableton Live 12 with Max for Live; Suite includes Max for Live.
- Tested on Intel with Live 12 Suite 12.4.16. The native component is universal; Apple-silicon runtime testing remains outstanding.
- English UI, constant tempo, 4/4, and one enabled instance per Set. Windows, tempo automation, meter changes and multiple enabled instances are not qualified.
- Bounds use Live's displayed sixteenth-note fields. Hidden off-grid fractions and arbitrary sample precision are not preserved reliably.
- Added handles include neighboring timeline audio. Before is clamped at the beginning of the Arrangement.

The embedded native component is Developer ID signed, Apple-notarized and stapled. The ZIP and `.amxd` are not separately claimed to be notarized containers. Read each release's README and license before installing.

## Support and privacy

- [Product information](https://dev.mathewharwich.com/projects/export-padding)
- [Report a reproducible bug](https://github.com/mathewharwich/export-padding-releases/issues)

Include the device version, Live version, macOS version, computer architecture, padding values and steps to reproduce the problem. Do not post private Sets, copyrighted audio, credentials, or unreviewed screenshots and diagnostics.

Export Padding runs inside Live. It does not require a companion app or account.

Export Padding is an independent project by Mathew Harwich, not affiliated with or endorsed by Ableton or Cycling '74. Ableton Live and Max for Live are products of their respective owners.
