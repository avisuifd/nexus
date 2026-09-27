# NEXUS Privacy Policy

**Effective September 26, 2026**

NEXUS is a free desktop dashboard made by avisuifd ("the developer"). This policy explains what NEXUS does with your information.

## The short version

- **Your data stays on your PC.** Tasks, notes, settings, chats and files are stored on your computer, not on any NEXUS server — there isn't one.
- **No accounts, no ads, no tracking, no analytics.** NEXUS doesn't collect usage statistics or crash reports, and the developer receives no information about you.
- **Nothing is sold or shared** by the developer, because the developer never has it.
- Some features need to talk to outside services (like a weather service). The table below lists exactly what each one sends.

## What stays on your computer

Stored in `%APPDATA%\NEXUS` (and your Downloads folder for received files):

- your name, settings and dashboard layout
- tasks, notes, links, countdowns, calendar events, timers and focus history
- Rocket League match history for your session
- Chat messages, invite codes and received files (`Downloads\NEXUS Chat`)
- Phone Drop history and received files (`Downloads\NEXUS Drop`)
- clipboard history (if you add that widget)
- Spotify/Gmail sign-in tokens (if you connect them), encrypted with Windows' built-in data protection
- a local error log used only for troubleshooting (it's never sent anywhere)

## What leaves your computer, and why

| Feature | Sent to | What's sent |
|---|---|---|
| Weather, forecast, air quality | Open-Meteo | The latitude/longitude of the city you picked |
| City search (Settings › Weather) | Open-Meteo | The text you type |
| Severe weather alerts (US) | US National Weather Service | Your weather city's latitude/longitude |
| Stocks | Yahoo Finance | The symbols on your watchlist |
| Sports | ESPN | The leagues and teams you follow |
| Now Playing album covers | Apple iTunes Search | The artist and song title — only when the playing app doesn't provide a cover |
| Quick Links icons | Google favicon service | The website addresses of your links |
| Update checks | GitHub | A request for the latest NEXUS version |
| Chat | ntfy.sh relay | **Encrypted** messages and files (see below) |
| Phone Drop — Internet mode | ntfy.sh relay, and GitHub Pages for the phone page | **Encrypted** text and files (see below) |
| Spotify widget (optional) | Spotify | Requests to your own Spotify account |
| Gmail widget (optional) | Google | Read-only requests to your own Gmail |

Like any website, these services can see your **IP address** and the time of each request, and handle it under their own privacy policies. NEXUS doesn't send them your name or any identifier of its own.

## Chat and Phone Drop

- **End-to-end encrypted.** Chat messages and files are encrypted on your PC with AES-256-GCM using a key made from the chat's invite code. Phone Drop's Internet mode works the same way, using a secret key in the QR link (the part after `#`, which browsers never send to any server).
- **The relay can't read them.** ntfy.sh only passes along scrambled data. It can see your IP address, when messages are sent, their size, and a random channel name. It keeps messages for about **12 hours** and files for about **3 hours**, then deletes them.
- **Anyone with an invite code or QR link can read that chat or drop.** Keep them private. **New link** in Phone Drop and **Leave chat** in Chat stop old codes from working for you.
- **Home-network Phone Drop** doesn't use the internet at all: your phone talks directly to your PC over your Wi-Fi, protected by a random password in the QR code.

## Features that read information on your PC

These run **only on your computer** and never send anything anywhere:

- **Text shortcuts** use a keyboard helper that keeps only the last few characters you typed in memory, to spot your shortcuts. Nothing is saved or sent, and it ignores keys while Ctrl, Alt or Win is held.
- **Camera & mic dots** read Windows' list of which apps are using your camera or microphone.
- **Clipboard history** keeps your recent text copies on your PC and skips items that password managers mark as private.
- **Now Playing** reads what Windows' media controls show; **System** reads CPU, memory and disk usage; **Rocket League** reads match data from the game on your PC.
- **Screensaver** checks how long your PC has been idle.

## Children

NEXUS is not meant for children under 13, and it doesn't knowingly collect information from anyone — it doesn't collect personal information at all.

## Your choices

- Turn off any feature: remove its widget, or switch it off in Settings (alerts, text shortcuts, camera & mic dots, updates, screensaver).
- Disconnect Spotify or Gmail in **Settings › Accounts**; this deletes the saved sign-in tokens.
- Export everything: **Settings › Data & backup › Export**.
- Delete everything: **Settings › Data & backup › Erase all data**, or uninstall NEXUS and delete `%APPDATA%\NEXUS` and the `Downloads\NEXUS Chat` and `Downloads\NEXUS Drop` folders.

## Security

NEXUS limits which websites it can contact, encrypts Chat and Phone Drop content, stores sign-in tokens with Windows' data protection, and verifies every update's checksum before installing it. No software is perfectly secure, so keep Windows up to date and only share invite codes with people you trust.

## Changes

If this policy changes, the new version will be included in NEXUS (**Settings › About & legal**) and on the NEXUS GitHub page, with a new date at the top.

## Contact

Questions about privacy: **github.com/avisuifd/nexus/issues**
