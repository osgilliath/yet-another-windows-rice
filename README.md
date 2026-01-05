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

![home](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20005001.png)

## programs-used
_these are the softwares used in the rice_
> contains links to the github repos or official sites of the programs

**window manager** - [`glazeWM`](https://github.com/glzr-io/glazewm)

- **terminal** - [`wt`](https://github.com/microsoft/terminal) and [`git bash`](https://git-scm.com/install/windows)
- **shell** - [`zsh`](https://github.com/ohmyzsh/ohmyzsh/) (with oh-my-zsh)
- **launcher** - [`flow launcher`](https://github.com/Flow-Launcher/Flow.Launcher)
- **status bar** - [`zebar`](https://github.com/glzr-io/zebar)
- **spotify rice** - [`spicetify`](https://github.com/spicetify/cli)
- **browser** - [`zen`](https://zen-browser.app/)
- **video player** - [`screenbox`](https://github.com/huynhsontung/Screenbox)
- **installer** - [`scoop`](https://scoop.sh/)
- **system info** - [`fastfetch`](https://github.com/fastfetch-cli/fastfetch)
- **text editor** - [`neovim`](https://neovim.io/)
- **code editor** - [`vs code`](https://code.visualstudio.com/)

## glazeWM
![glaze](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20004222.png)

install using:</br>
```bash
winget install GlazeWM
```

- changed the [config](https://github.com/osgilliath/yet-another-windows-rice/blob/main/dots/config.yaml) a little so that the window gaps are reduced and it is compatible with flow launcher key bindings

***how to start glaze at startup?***
- make a desktop shortcut of glaze (usually created by itself)
- open run (super+r) and type `shell:startup`
- copy the shortcut and paste in the folder opened
 
## flow-launcher
![flow](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20002552.png)

install [flow launcher](https://github.com/Flow-Launcher/Flow.Launcher) by:
```bash
winget install "Flow Launcher"
```

**theme:** [macOS.flow](https://github.com/cc46808/macOS.flow) 

**plugins (optional):**
- calculator
- spotify premium
- pokedex
- dictionary

![preview](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20005920.png)

## zebar
![zebar](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20001222.png)
comes bundled by default with GlazeWM

**widget used:** overline-zebar

## spotify
> install spotify using their official site not using microsoft store

![spotify ui](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202025-12-30%20233046.png)
(check out the cat on top of the playback bar)

![lyrics](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202025-12-30%20233034.png)

install spicetify by running (in powershell):
```bash
iwr -useb https://raw.githubusercontent.com/spicetify/cli/main/install.ps1 | iex
```

**Theme:** comfy

**Snippets:**
- Dynamic Search Bar
- Rotating Cover Art
- Remove Top Gradient
- Modern Scroll Bar
- Oneko

## zen-browser
![browser ui](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202025-12-30%20234718.png)

**mods:** Transparent Zen

**layout:** only sidebar

**extensions:**
- uBlock origin
- Zen Internet

## file-explorer
![explorer](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20005238.png)

clone the [ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica) repo, to get transparent window effect

## scoop
a simple command-line installer, using which you can install programs from the terminal that are not available in winget

run in a powershell terminal:
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```
or for advanced installation options, you can see their [github](https://github.com/ScoopInstaller/Install#readme)

## neovim
multiple options are available to install neovim in windows, but I recommend using scoop, as there are multiple gui options available for nvim in scoop

to install nvim using scoop, run:
```bash
scoop bucket add main
scoop install neovim
```

you can check various gui for nvim, [here](https://scoop.sh/#/apps?q=neovim)

## fastfetch
![fstftch](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-05%20223314.png)

install using scoop: `scoop install fastfetch`

**for customisation:**
- download both the [config files](https://github.com/osgilliath/yet-another-windows-rice/tree/main/fastfetch)
- open run (super+r) and type `%USERPROFILE%`
- create or open the .config folder
- make a folder named 'fastfetch' (remove the '', duhhh)
- paste both the config files there
- replace '%USERPROFILE%' in [config.jsonc](https://github.com/osgilliath/yet-another-windows-rice/blob/main/fastfetch/config.jsonc) with your pc's user name (i.e. the name of the folder .config is in)
- run `fastfetch`

## vs-code
soon!!

