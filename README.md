# StreamGoblin

**Feed the Stream. Tame the Chaos.**

StreamGoblin is a friendly Windows installer and compatibility checker for streaming software. It uses native Windows APIs, `HttpClient`/Windows Package Manager, and ordinary Windows processes. **It does not use PowerShell.**

## Included apps
OBS Studio, VoiceMeeter, NVIDIA Broadcast, Voicemod, SteelSeries Sonar, Streamlabs Desktop, PRISM Live Studio, and Meld Studio.

## New-computer friendly
- Self-contained x64 and x86 builds; users do not need to install .NET.
- Automatic first-run Goblin Gear Check.
- Architecture, RAM, storage, GPU, microphone, camera, pending-restart, admin and winget checks.
- Official vendor pages as a safe fallback.
- Detects already-installed applications.
- Clear blocking and recommendation messages.

## Important x86 note
StreamGoblin itself can be built for both x86 and x64. Many modern streaming applications are x64-only. On a 32-bit PC, incompatible cards are disabled rather than forced.

## Build on Windows
1. Install the .NET 8 SDK.
2. Optional: install Inno Setup 6 to produce installer EXEs.
3. Double-click `build\build-all.cmd`.
4. Outputs appear under `releases`.

No PowerShell script is used by the project or build process.

## Expand the catalogue
Edit `catalog/apps.json`. Add the app name, official website, winget package ID, supported architectures, requirements, and detection names.

## Security
StreamGoblin never asks for stream keys or account passwords. It does not disable Windows security and does not use third-party download mirrors.

## Experience presets and category selection
StreamGoblin includes beginner-friendly experience presets:
- Beginner Streamer
- Simple OBS Setup
- Gaming Streamer
- Professional Broadcaster
- Podcast & Talk Show
- Creative / Multiplatform
- Low-Spec PC
- Everything Compatible

Every software category includes its own **Select All** and **Clear** buttons. Users can apply a preset and then customize individual applications or entire categories before installing.

## Responsive interface in v1.2.0

StreamGoblin now automatically adapts to different monitor sizes, window sizes, and Windows DPI scaling. Wide windows show full horizontal application cards. Narrow windows switch to taller stacked cards so descriptions, compatibility results, and action buttons do not overlap. The sidebar also changes width automatically, and nonessential header details hide on compact screens.

Recommended supported display range starts at 760×600, with the best experience at 1280×720 or higher. Windows scaling at 100%, 125%, 150%, and 200% is handled through DPI-aware WinForms scaling.

