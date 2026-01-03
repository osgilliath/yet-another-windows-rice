# yet-another-windows-rice

The repo contains:
- the softwares used in the rice
- the config files (modified ones) of the programs
- the settings changed / extensions installed in the programs
- installation scripts
- github repos or official sites
- wallpapers and colour schemes used
- screenshots of the rice

---

## programs-used
_these are the softwares used in the rice_
> contains links to the github repos or official sites of the programs

**window manager** - [`glazeWM`](https://github.com/glzr-io/glazewm)

- **terminal** - [`wt`](https://github.com/microsoft/terminal) and [`git bash`](https://git-scm.com/install/windows)
- **shell** - [`zsh`](https://github.com/ohmyzsh/ohmyzsh/) (with oh-my-zsh)
- **launcher** - [`flow launcher`](https://github.com/Flow-Launcher/Flow.Launcher)
- **lockscreen** - _tba_
- **status bar** - [`zebar`](https://github.com/glzr-io/zebar)
- **spotify rice** - [`spicetify`](https://github.com/spicetify/cli)
- **browser** - [`zen`](https://zen-browser.app/)
- **video player** - [`screenbox`](https://github.com/huynhsontung/Screenbox)
- **system info** - [`fastfetch`](https://github.com/fastfetch-cli/fastfetch)
- **text editor** - [`neovim`](https://neovim.io/)

## glazeWM
![glaze](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20004222.png)
install using:</br>
```bash
winget install GlazeWM
```
- changed the [config](https://github.com/osgilliath/yet-another-windows-rice/blob/main/dots/config.yaml) a little so that it the window gaps are reduced and it is compatible with flow launcher key bindings


## flow-launcher
![flow](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20002552.png)
install [flow launcher](https://github.com/Flow-Launcher/Flow.Launcher) </br>
theme: [macOS.flow](https://github.com/cc46808/macOS.flow) </br>
plugins(optional):
- spotify premium
- pokedex
- dictionary

![preview](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20002732.png)

## zebar
![zebar](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20001222.png)
comes bundled by default with GlazeWM

widget used: overline-zebar

## spotify
> install spotify using their official site not using microsoft store

![spotify ui](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202025-12-30%20233046.png)

![lyrics](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202025-12-30%20233034.png)

install spicetify by running (in powershell):
```bash
iwr -useb https://raw.githubusercontent.com/spicetify/cli/main/install.ps1 | iex
```
Theme: comfy <br/>
Snippets: 
- Dynamic Search Bar
- Rotating Cover Art
- Remove Top Gradient
- Modern Scroll Bar
- Oneko

## zen-browser
![browser ui](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202025-12-30%20234718.png)

mods: Transparent Zen
layout: only sidebar
extensions:
- uBlock origin
- Zen Internet

## file-explorer
clone the [ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica) repo, to get transparent window effect

