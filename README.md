<p align="center">
  <img src="docs/images/banner.png" alt="StreamGoblin banner" width="100%">
</p>

<h1 align="center">StreamGoblin</h1>

<p align="center">
  <strong>Feed the Stream. Tame the Chaos.</strong><br>
  A user-friendly Windows installer and compatibility checker for live-streaming software.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D4?logo=windows&logoColor=white" alt="Windows 10 and 11">
  <img src="https://img.shields.io/badge/Builds-x64%20%7C%20x86-7C3AED" alt="x64 and x86">
  <img src="https://img.shields.io/badge/PowerShell-Not%20Used-22C55E" alt="No PowerShell">
  <img src="https://img.shields.io/badge/Focus-Live%20Streaming-EC4899" alt="Live Streaming">
</p>

---

## What is StreamGoblin?

**StreamGoblin** helps streamers prepare a Windows PC with the tools needed for live broadcasting, audio routing, voice effects, and camera enhancement.

Instead of searching multiple websites and guessing which applications will work, StreamGoblin checks the computer, organizes compatible choices, and helps install selected software from official sources.

## Highlights

- **Goblin Gear Check** scans the PC before installation
- Detects Windows architecture, RAM, storage, CPU, GPU, microphone, camera, and restart status
- Checks whether selected software is compatible with the computer
- Detects supported applications that are already installed
- Groups applications into clear live-streaming categories
- Includes presets for different experience levels and streaming styles
- Provides **Select All** and **Clear** controls for each category
- Supports separate **x64** and **x86** StreamGoblin installers
- Uses official package sources or official developer pages
- Uses no PowerShell scripts or PowerShell commands
- Responsive layout for different monitor sizes and Windows scaling settings

## Supported Live-Streaming Software

| Category | Applications |
|---|---|
| **Streaming & Recording** | OBS Studio, Streamlabs Desktop, PRISM Live Studio, Meld Studio |
| **Audio Routing & Mixing** | VoiceMeeter, SteelSeries Sonar |
| **Voice Effects** | Voicemod |
| **Camera & AI Enhancement** | NVIDIA Broadcast |

> Some modern streaming applications only support 64-bit Windows. StreamGoblin can run on x86 Windows, but incompatible applications will be blocked instead of being installed incorrectly.

## Experience Presets

StreamGoblin can automatically select recommended software for different users:

| Preset | Best for |
|---|---|
| **Beginner Streamer** | A simple first streaming setup |
| **Simple OBS Setup** | Users who want a clean OBS-based workflow |
| **Gaming Streamer** | Game streaming with audio and voice tools |
| **Professional Broadcaster** | A more complete production setup |
| **Podcast & Talk Show** | Microphone-focused live broadcasts |
| **Creative / Multiplatform** | Creative and multi-platform streaming |
| **Low-Spec PC** | Lighter software choices |
| **Everything Compatible** | Every supported app that passes the Gear Check |

Presets are only a starting point. Every application can still be selected or cleared manually.

## Download and Install

Open the repository's **Releases** page and download the installer that matches your computer:

| File | Choose this version when |
|---|---|
| `StreamGoblin-Setup-x64.exe` | You use 64-bit Windows. This is correct for most modern computers. |
| `StreamGoblin-Setup-x86.exe` | You use 32-bit Windows. |

### Check your Windows system type

1. Open **Windows Settings**.
2. Select **System**.
3. Select **About**.
4. Look for **System type**.

### Install StreamGoblin

1. Download the correct installer.
2. Double-click the downloaded `.exe` file.
3. Approve the Windows security prompt.
4. Follow the setup wizard.
5. Launch StreamGoblin from the Start menu or desktop shortcut.

## Using StreamGoblin

1. Select **Run Gear Check**.
2. Review the compatibility score and detected computer information.
3. Choose an experience preset or select applications manually.
4. Use **Select All** or **Clear** inside each category.
5. Review any compatibility warnings.
6. Select **Unleash Installer**.
7. Follow any official installer windows that appear.

Applications marked as incompatible are not selected automatically.

## Goblin Gear Check

Goblin Gear Check can review:

- Windows version and system architecture
- Installed memory
- Available storage
- Processor information
- Graphics hardware
- NVIDIA RTX availability
- Microphone and camera availability
- Pending Windows restart
- Administrator access
- Windows Package Manager availability
- Supported applications already installed

The score is guidance rather than a guarantee. Live-streaming performance also depends on internet upload speed, stream resolution, bitrate, encoder choice, and other programs running on the PC.

## Responsive Interface

StreamGoblin adjusts to:

- Different monitor resolutions
- Resized application windows
- Windows display scaling
- Compact and wide layouts

On smaller windows, application cards reflow vertically to keep descriptions and controls readable. A resolution of **1280 × 720 or higher** is recommended.

## Safety and Privacy

StreamGoblin is designed to be transparent:

- Does not request stream keys or account passwords
- Does not disable Windows security
- Does not install unrelated software
- Does not use unofficial download mirrors
- Does not use PowerShell
- Uses official package sources and developer pages
- Shows which applications are selected before installation

## Troubleshooting

### StreamGoblin does not start

Open this diagnostic file:

```text
%LOCALAPPDATA%\StreamGoblin\startup-error.log
```

Include its contents when reporting a startup problem.

### An application cannot be selected

The application may not support your Windows architecture or detected hardware. Read the compatibility message displayed on its card.

### NVIDIA Broadcast is unavailable

NVIDIA Broadcast requires supported NVIDIA RTX hardware and compatible drivers.

### StreamGoblin opens an official website

An automatic package may not be available. StreamGoblin opens the official developer page so the application can be downloaded safely.

### A restart is recommended

Virtual audio devices and audio drivers may require a Windows restart before they work correctly.

## Uninstalling StreamGoblin

1. Open **Windows Settings**.
2. Select **Apps**.
3. Open **Installed apps**.
4. Find **StreamGoblin**.
5. Select **Uninstall**.

Removing StreamGoblin does not automatically uninstall the streaming applications installed through it.

## Important Notice

StreamGoblin is an independent setup utility. OBS Studio, VoiceMeeter, NVIDIA Broadcast, Voicemod, SteelSeries Sonar, Streamlabs Desktop, PRISM Live Studio, and Meld Studio belong to their respective developers and are subject to their own licences and terms.

---

<p align="center">
  <strong>StreamGoblin</strong><br>
  Feed the Stream. Tame the Chaos.
</p>
