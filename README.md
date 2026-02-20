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

![home](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/demo.gif)

## programs-used
_these are the softwares used in the rice_
> contains links to the github repos or official sites of the programs

**window manager** - [`glazeWM`](https://github.com/glzr-io/glazewm)

- **terminal** - [`wt`](https://github.com/microsoft/terminal) and [`git bash`](https://git-scm.com/install/windows)
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
_widget-config:_ [here](https://github.com/osgilliath/yet-another-windows-rice/blob/main/zebar/overline-zebar-config.json)
(you may change the colours as per your theme)

## terminal
![terminal](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-02-05%20213807.png)

_pre-requisite:_ install jet-brains mono font from [nerd-fonts](https://www.nerdfonts.com/font-downloads)

- open the terminal
- go to settings (drop down menu near the plus icon)
- go to 'open json file' (bottom of the left side bar)
- replace the contents of the file with [this](https://github.com/osgilliath/yet-another-windows-rice/blob/main/terminal/settings.json)
- save the file

**to install some other theme:**
- go to [windows terminal themes](https://windowsterminalthemes.dev/)
- select a theme and click on get theme
- paste the copied text in the 'schemes' section of the json file
- change theme from the appearance section of the settings

## scoop
a simple command-line installer, using which you can install programs from the terminal that are not available in winget

run in a powershell terminal:
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```
or for advanced installation options, you can see their [github](https://github.com/ScoopInstaller/Install#readme)

## fastfetch
![fstftch](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-02-05%20213820.png)

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
![vscode](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-05%20235928.png)

**Theme:** Catppucin for VSCode

**Icons:** Catppucin icons

**Extensions:**
- Power Mode, by Cody Hoover
- vscode-pets, by Anthony Shaw
- Prettier, by Prettier
- readme-preview, by Manish Sencha

**how to make it minimal:**
1. go to view -> appearance -> menu bar (untick it)
2. right click on any empty space in the side bar
3. go to activity bar position -> top
4. right click again -> move primary side bar right (optional)
5. right click on the search bar
6. untick command centre (you can access it with ctrl+shift+p)

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

**Extensions:**
- Immersive view
- NPV Ambience
- Reeeewiiiind

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
- Zen Internet (mandatory for the transparent effect)

## file-explorer
![explorer](https://github.com/osgilliath/yet-another-windows-rice/blob/main/Screenshots/Screenshot%202026-01-04%20005238.png)

**for the transparent effect:**
- clone the [ExplorerBlurMica](https://github.com/Maplespe/ExplorerBlurMica) repo, or the download the raw files
- extract the files
- open the Release folder, and run 'register.cmd' as administrator
- reopen file explorer to see the effect
- change the value of 'a' in config.ini to adjust transparency (i use a=0)

**for uninstallation:**
- run 'uninstall.cmd' as administrator

## neovim
multiple options are available to install neovim in windows, but I recommend using scoop, as there are multiple gui options available for nvim in scoop

to install nvim using scoop, run:
```bash
scoop bucket add main
scoop install neovim
```

you can check various gui for nvim, [here](https://scoop.sh/#/apps?q=neovim)

> Now you can say I use windows btw 
