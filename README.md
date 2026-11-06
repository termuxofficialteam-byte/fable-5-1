# Fable 5.1

Fable 5.1 is a Python command-line companion designed for Termux.

## Install and run in Termux

```sh
pkg update -y
pkg install python git -y
git clone https://github.com/termuxofficialteam-byte/fable-5-1.git
cd fable-5-1
python -m pip install rich
python Fable_5.1.py
```

On first launch, the program prompts for a Gemini API key. Obtain one from Google AI Studio and enter it only into the local Termux prompt. **Do not put API keys in this repository or share them publicly.** The program saves the entered key locally at `~/.vesper/api_key`; protect access to your Termux home directory.

## Optional: Termux:API features

Some Android device features require installing the separate Termux:API Android app from the same trusted source as Termux, then installing its companion package:

```sh
pkg install termux-api
```

Grant Android permissions only for features you choose to use. Without Termux:API, the core command-line interface can still run, but device-specific features may be unavailable.

## Dependency

The required third-party Python package for the terminal interface is `rich`. The remaining top-level imports use Python's standard library. Some optional tool functions may need additional packages or command-line programs; the script reports missing optional dependencies when those functions are used.
