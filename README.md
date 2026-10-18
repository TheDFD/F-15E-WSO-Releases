# F-15E WSO downloads

Public installers and update feeds for F-15E WSO. Development source remains private.

## Installation and updates

Close DCS and Goose, then download and run the [1.1.186-beta.1 installer](https://github.com/TheDFD/F-15E-WSO-Releases/releases/tag/beta-v1.1.186-beta.1). Older clients without the update feature need this one manual installation. No GitHub account or token is required.

This Beta adds the requested snowplow → UFC coordinate point → TPOD PB17 flow for A/G Nearest and Waypoint. Nearest uses a verified empty `.C` target point; Waypoint uses the existing point. Both LANTIRN and LITENING stop after cueing, without zoom, manual slew or automatic designation. Occupied points are preserved.

A/A Next verifies 4TWS and uses Coolie UP on a visible front radar page. A/A Previous, PACS Link and A/G Picture are removed from the menu. CTAF is R1 305 / R2 251 AM. Purple becomes Black / MPD Green, Settings controls are clearer, and repeated volume-slider saves are coalesced. Short spike/launch alerts precede optional descriptions; confirmed splash reports survive new cockpit orders. The existing explicit STOP quiet policy remains.

Under **Settings > Updates**, choose **Beta** for numbered test releases or **Stable** for approved releases. Stable has no published installer yet. Selecting an unpublished channel leaves your installed version in place.

Goose checks shortly after startup and every 30 minutes while running. Automatic installation waits until DCS is closed; Windows may request administrator approval. You can turn automatic installation off. Downloads are checked for version, channel, size and SHA-256. A published Stable release can replace an installed Beta when Stable is selected.

## Monitor placement

**Settings > Overlay display** remembers your monitor and menu position. Choose the DCS window, primary monitor or a connected display, then one of nine positions. Disconnected displays fall back to primary while retaining your saved choice. Use **Refresh monitors** after changing your layout. The optional status card opens on the same monitor and can be dragged separately.

## VR setup: SteamVR and OpenXR

VR requires the separately installed [OpenKneeboard companion](https://openkneeboard.com/). Goose supplies a persistent capture source; OpenKneeboard supplies headset rendering and placement.

1. Start Goose, DCS and OpenKneeboard with normal Windows user privileges.
2. Enable **Settings > Overlay display > VR capture window** in Goose.
3. In OpenKneeboard, add a **Window Capture** tab for **F-15E WSO VR Menu**. Enable **Capture client area** to exclude its title bar.
4. Enable the appropriate SteamVR or OpenXR support in OpenKneeboard for the runtime used by DCS. Set headset position, size and recenter there.
5. Keep the capture source open and unminimized. Desktop monitor placement and headset placement are separate.

Use your existing WSO open/select, slew and Back bindings. Menus, target choices, confirmations and radio entry share the source window. Its handle survives menu closing; **Show VR capture window** reopens the source if you close its title bar. The optional **F-15E WSO VR Status** card needs a separate capture tab.

Follow the companion's [window-capture guide](https://openkneeboard.com/features/window-capture/), [capture compatibility notes](https://openkneeboard.com/troubleshooting/window-capture-compatibility/) and [SteamVR/OpenXR instructions](https://github.com/OpenKneeboard/OpenKneeboard/blob/master/docs/troubleshooting/steamvr-or-openxr.md).

This Beta has automated Windows capture-window, input and placement checks. Live headset rendering, motion-controller pointing, multiplayer-server compatibility and the real installer/UAC upgrade cycle still need testing. Goose does not install a VR companion or change your runtime. This feature preserves the existing flight logic, DCS scripts and audio and does not modify F-15E module files.

[All releases](https://github.com/TheDFD/F-15E-WSO-Releases/releases)
