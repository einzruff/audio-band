# Fork of audio-band from dsafa

Install:
1. copy release\connectors folder into \debug
2. create batch file, install.cmd in \debug with contents:
@echo off
%SystemRoot%\Microsoft.NET\Framework64\v4.0.30319\regasm.exe /nologo /codebase %~dp0AudioBand.dll
pause

Uninstall:
For uninstall, create batch file uninstall.cmd in \debug with contents:
@echo off
%SystemRoot%\Microsoft.NET\Framework64\v4.0.30319\regasm.exe /nologo /unregister %~dp0AudioBand.dll
pause

---

[![Build status](https://ci.appveyor.com/api/projects/status/v32xl29r8uucuwj3?svg=true)](https://ci.appveyor.com/project/dsafa/audio-band)

# Audio Band
*This is still a work in progress!*

Audio Band allows you to display song information in the taskbar.

![Demo](./screenshots/demo.gif)

## Features
- Displays song information - album art, artist, title, progress
- Control your music - play/pause, previous/next
- Add support for your music player of choice through plugins

## Installation
There is currently no installer available, however there are prereleases in the [Release](https://github.com/dsafa/audio-band/releases) page.

## Usage
1. Right click on the taskbar and select `Audio Band` from the toolbars submenu.
2. Right click on the Audio Band toolbar and select an audio source
_images here_

### Current Supported Audio Sources
- Spotify

## Building
This project uses C# 7 features so a compatible compiler is required.

## Contributing
Help is appreciated
- Ask questions, report bugs, suggest features in issues
- Send pull requests

## Screenshots
![Screenshot](./screenshots/screenshot.png)

## License
[LICENSE](https://github.com/dsafa/audio-band/blob/master/LICENSE)
[THIRD PARTY](https://github.com/dsafa/audio-band/blob/master/LICENSE-3RD-PARTY)
