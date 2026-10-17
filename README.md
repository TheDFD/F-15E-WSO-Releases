# F-15E WSO downloads

Official public downloads for F-15E WSO. This repository hosts installers and update feeds. The development source remains private.

## First installation

1. Close DCS and Goose.
2. Download [F-15E WSO 1.1.185-beta.2](https://github.com/TheDFD/F-15E-WSO-Releases/releases/tag/beta-v1.1.185-beta.2) and run the installer.
3. Open **Settings > Updates** and choose **Beta** or **Stable**.

Existing 1.1.184 clients need this one manual installation to enable automatic updates. No GitHub account or access token is required.

## Update channels

| Channel | Releases |
| --- | --- |
| Beta | Numbered test builds, beginning with `1.1.185-beta.2`. |
| Stable | Approved releases. |

Goose checks for updates shortly after startup and every 30 minutes while running. With automatic installation enabled, updates wait until DCS is closed. Windows may request administrator approval. The selected channel is remembered, and automatic installation can be turned off in Settings.

If a channel has no published installer, selecting it leaves the installed version in place. A published Stable release can replace an installed Beta when Stable is selected.

Downloads use HTTPS and are checked for version, channel, file size and SHA-256 before installation. The update system retains the stock F-15E module files. This Beta preserves the flight code, overlay renderer, DCS scripts and audio from 1.1.184.

[All releases](https://github.com/TheDFD/F-15E-WSO-Releases/releases)

