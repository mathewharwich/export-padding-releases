# Export Padding

Add time before and after Ableton Live exports with a compact Max for Live device.

## Free beta

**[Download Export Padding 0.4.0 beta 1](https://github.com/mathewharwich/export-padding-releases/releases/tag/v0.4.0-beta.1)**

Choose the **Export-Padding-0.4.0-beta.1-macOS.zip** release asset and unzip it. Copy **Export Padding.amxd** to your Ableton User Library and place one enabled instance on Main. This repository contains public downloads and documentation. The implementation is maintained in a private repository. The beta is free for personal or professional use under the included license.

## Use

Set Before and After in 0.25-second steps over 0–60 seconds. Leave **Padding ON**, select an Arrangement range and open **Export Audio/Video**. The device measures Live’s timing across tempo and meter changes where it can verify the range. Wait for the adjusted render bounds, review them and export.

**Protect tail** is optional. Turn it on before opening Export. It checks the completed render for a tail, then keeps the full After interval beyond that tail. Main WAV and AIFF at 16, 24 and 32 bits, FLAC at 16 and 24 bits, and native Live MP3 are supported. Turn off Normalize, Render as Loop, Create Analysis File and Video. MP3 protection keeps complete encoded frames and verifies the decoded result without re-encoding.

The scan covers up to 60 extra seconds at a −80 dBFS threshold. Later audio, continuing tails and unverified bounds can leave the full render for review. Keep the hidden recovery files until you have checked the output.

## Compatibility and support

Requires macOS, Ableton Live 12 with Max for Live, and the English Live interface. Intel qualification uses Live 12 Suite 12.4.16. The universal bundle includes Apple silicon code, with runtime qualification pending.

For a reproducible issue, include the device version, Live version, macOS version, architecture, export settings and steps. Review any screenshots or diagnostics before sharing them.

[Product information](https://dev.mathewharwich.com/projects/export-padding) · [Issue tracker](https://github.com/mathewharwich/export-padding-releases/issues)

Export Padding is an independent project by Mathew Harwich. Ableton Live and Max for Live are products of their respective owners.
