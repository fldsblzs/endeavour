# Endeavour OS Configurations
Configurations and utilities for Endeavour OS

## Terminal

Default terminal is [Tabby](https://tabby.sh/) using the [altair](https://github.com/yxuko/terminus-altair) theme. The default shell is `zsh` with [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh).

## Editors

Terminal based text editor [Helix](https://helix-editor.com/), [documentation](https://docs.helix-editor.com/), [GitHub repo](https://github.com/helix-editor/helix).

GUI text editor [Visual Studio Code](https://code.visualstudio.com/).

## App Launcher

[rofi](https://github.com/davatorium/rofi) window switcher, application launcher and dmenu replacement. Also using this curated [rofi collection](https://github.com/adi1090x/rofi) for themes and nice stuff.

### Shortcut for rofi

Set up global shortcut on `Ctrl + Return` to run `~/.config/rofi/launchers/type-1/launcher.sh`.

## OneDrive

Using [onedrive](https://github.com/abraunegg/onedrive/blob/master/README.md) client in Docker, see [details](./onedrive/README.md)

## Misc

### Disable PC Speaker

```sh
# /etc/modprobe.d/nobeep.conf

blacklist pcspkr
blacklist snd_pcsp
```