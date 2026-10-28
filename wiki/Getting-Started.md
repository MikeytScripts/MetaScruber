# Getting Started

## 1. Download

Go to the **[latest release](https://github.com/MikeytScripts/MetaScruber/releases/latest)** and download one file:

| File | For |
|---|---|
| **MetaScrub.exe** | Most Windows 10 and 11 PCs |
| **MetaScrub-arm64.exe** | Windows on ARM laptops (for example Snapdragon) |
| SHA256SUMS.txt | Checksums, if you want to verify the download |

Not sure which one? Open **Settings → System → About** in Windows and look at **System type**. "ARM-based processor" means the arm64 file; anything else means `MetaScrub.exe`.

**Optional, to verify the download:** in PowerShell, run `Get-FileHash .\MetaScrub.exe` and check the hash matches the line in `SHA256SUMS.txt`.

## 2. Run it

Double-click the `.exe`. There's nothing to install.

Windows SmartScreen may warn you the first time because the app isn't code-signed yet. Click **More info → Run anyway**.

On first use, MetaScrub may download the open-source tools **ffmpeg** and **yt-dlp** from their official GitHub releases. That's normal, and no personal data is sent.

## 3. Enter your license key

The download is free, but you need a **license key** to use it. **[Get one on Discord](https://discord.gg/HnqkyDkFUA)**, then enter it when MetaScrub asks. Each key works on one PC.

## 4. Optional setup

| To use... | You need |
|---|---|
| **Schedule** | Connect your YouTube channels (Schedule → **Connect a channel**) |
| **AI titles** | An AI API key. See [OpenRouter: API Key and Choosing a Model](OpenRouter-Setup). |
| **Tracker** | Your own YouTube API key |
| **Discord alerts** | A Discord webhook URL. See [Features → Discord alerts](Features#discord-alerts). |

## Where your data lives

Settings, the upload queue, upload history and tracked stats are saved in **Documents\MetaScrub**. Google sign-in tokens and API keys are encrypted with Windows' built-in data protection. There is no MetaScrub server.
