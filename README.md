<div align="center">

<img src="icon.png" width="64" height="64" alt="Voice Helper for Claude">

# Voice Helper for Claude

**Control Claude with your voice — no keyboard, no mouse.**
Say the wake name («Клод»), dictate your request — the helper starts dictation, sends the message and turns the microphone off by itself.

[![Latest version](https://img.shields.io/github/v/release/vladkharitonov87/claude-voice-helper-releases?label=version&color=D97757)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)
[![Release date](https://img.shields.io/github/release-date/vladkharitonov87/claude-voice-helper-releases?label=released)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/vladkharitonov87/claude-voice-helper-releases/total?label=downloads)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases)
![Windows 10 | 11](https://img.shields.io/badge/Windows-10%20%7C%2011-0078D4?logo=windows)

<br>

[![Download for Windows](https://img.shields.io/badge/Download_for_Windows-D97757?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases/latest)

<sub>The <code>voice-helper-for-claude-&lt;version&gt;-setup.exe</code> file in the <b>Assets</b> section ·
<a href="https://github.com/vladkharitonov87/claude-voice-helper-releases/releases">Release history</a></sub>

</div>

---

> [!NOTE]
> The voice commands are currently **Russian only**: the wake name and the command words are Russian
> words, shown below in «quotes» with an English translation. The app's interface is available in
> **English** (the default) and **Russian** — choose it in **Settings → General → Language**; below,
> the names of its menu items and settings are given in both languages.

## What it does

- 🎙️ **Listens for the wake name.** Say «Клод» ("Claude") and Claude starts recording — your hands stay free.
- 📨 **Sends by itself.** The message goes out after a short pause, or right away on the «отправь» ("send") command.
- ↩️ **Cancels and stops.** «отмена» ("cancel") clears the input field, «стоп» ("stop") interrupts Claude's reply.
- 🔇 **Turns the microphone off** after every command, so Claude does not hear anything extra.
- 🔒 **Recognizes commands on your computer**, offline: no audio is sent anywhere.
- 🎯 **Learns not to react to look-alike words.** Words that sound like the name («холод», «код») are picked automatically as exceptions, and you can add a word to them straight from the tray menu after a false start. The «Check the word» button shows what the app hears when you say a word.
- ⏸️ **Pauses on a hotkey.** Pause and resume listening from the tray menu or with a hotkey (Ctrl + Alt + V by default; a key, a combination, or the middle/side mouse button — set in the settings).
- 🟢 **Shows its state** with the tray icon: listening, recording, no microphone, paused.
- ⚙️ **Configured in the app:** command words, delays, microphone, sounds, hotkeys, light or dark theme, interface language (English or Russian).
- 🛡️ **Explains itself** if Claude is running as administrator and offers to restart the helper with the same rights.
- 🔄 **Updates itself:** the tray menu tells you about a new version — one click and it is installed, with a progress window.

## Voice commands

| Say | What happens |
|---|---|
| **«Клод»** (and a pause) or **«Клод, записывай»** ("Claude, record") | Claude starts dictation — the text appears in the input field |
| *dictate your text and stay silent for 1.5 s* | The message is sent automatically |
| **«Клод, отправь»** ("Claude, send") | Send right away, without waiting for the pause |
| **«Клод, отмена»** ("Claude, cancel") | Discard what you dictated |
| **«Клод, стоп»** ("Claude, stop") | Stop the reply Claude is writing right now |

While recording, «отправь» and «отмена» also work without the name. Starting a recording and stopping
a reply work only when the Claude window is active, so a random phrase in a conversation will not
trigger anything in the background. All words and delays can be changed in the settings, **Voice commands**
(«Голосовые команды») section.

## Installation

1. Click **Download for Windows** above and download
   `voice-helper-for-claude-<version>-setup.exe` from the **Assets** section.
2. Run the installer and allow the changes — the app is installed for all users into
   `C:\Program Files\Voice Helper for Claude`. Shortcuts on the desktop and in the Start menu are optional checkboxes in the installer.
3. If Windows shows "Windows protected your PC", click **More info → Run anyway**. The installer is
   not digitally signed yet, so SmartScreen does not recognize it.
4. In Claude, choose the dictation language: **Settings → General → Voice → Language → Russian**.

After the installation the helper appears in the tray and starts with Windows (you can turn this off in
the settings). Click the icon to open the settings.

> [!TIP]
> You can check that the file was downloaded intact by its SHA-256 checksum, which is shown next to the
> file on the release page:
> `Get-FileHash .\voice-helper-for-claude-<version>-setup.exe`

## Requirements

| | |
|---|---|
| System | Windows 10 or 11, 64-bit |
| Claude | The Claude desktop app for Windows with voice input |
| Microphone | Any: built-in, headset or USB — chosen in the settings |
| Command language | Russian |
| Interface language | English or Russian — chosen in the settings |

There is nothing else to install: speech recognition and everything else needed are included in the installer.

## Updating

The app checks for new versions by itself — every 6 hours and on **Check for updates**
(«Проверить обновления») in the tray menu. When a new version is out, the menu shows **Update to X.Y.Z**
(«Обновить до X.Y.Z»): the helper downloads it, installs it and restarts itself. You can also update
manually by installing the new version over the old one. Your settings are kept.

What changed in each version is in the [release history](https://github.com/vladkharitonov87/claude-voice-helper-releases/releases).

## Privacy

- Commands are recognized locally ([Vosk](https://alphacephei.com/vosk/)) — audio never leaves your computer.
- The text itself is dictated by Claude's built-in voice input — the helper only presses its buttons.
- The only internet access is the update check on GitHub.
- The log is stored on your computer only and does not contain the dictated text.

## Uninstalling

**Windows Settings → Apps → Installed apps → Voice Helper for Claude → Uninstall.**
Your settings stay in `%AppData%\ClaudeVoiceHelper` — delete that folder if you no longer need them.

## Questions and bugs

Found a bug or have an idea? [Create an issue](https://github.com/vladkharitonov87/claude-voice-helper-releases/issues).
Please attach the version (tray icon menu) and the log from `%AppData%\ClaudeVoiceHelper\logs`.

---

<sub>Voice Helper for Claude is an independent project not affiliated with Anthropic. Claude is a trademark of Anthropic, PBC.</sub>
