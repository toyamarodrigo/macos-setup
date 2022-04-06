# My macOS Setup for Development
### Install xcode
```
xcode-select --install
```

### Install Homebrew & dependencies
```
/usr/bin/ruby -e “$(curl -fsSl https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

*Create Brewfile in root*
```
touch Brewfile
```
*add all dependencies to Brewfile*
```
tap "homebrew/bundle"
tap "homebrew/cask"
tap "homebrew/core"
brew "bash"
brew "git"
brew "jenv"
brew "mysql"
brew "postgres"
brew "mongodb"
brew "vcprompt"
cask "alfred"
cask "postman"
cask "firefox"
cask "cleanmymac"
cask "bartender"
cask "dropbox"
cask "endurance"
cask "franz"
cask "hyperswitch"
cask "iterm2"
cask "libreoffice"
cask "spectacle"
cask “vlc”
cask “visual-studio-code"
```
*Install dependencies*
```
brew bundle
```
---

### iTerm2 configuration
**Font: Anonymous pro**
https://www.marksimonson.com/fonts/view/anonymous-pro

*Profiles > Edit profiles > Working Directory > Reuse previous section directory*

**Keys**
> Natural text editing

> Anonymous pro 20pt

**Window**
> Column: 70, Row: 20

---

### Bash - setting up default shell
```
sudo nano /etc/shells
```
#### Comment all of them & add /usr/local/bin/bash
```
// /bin/bash
// /bin/csh
// /bin/ksh
// /bin/sh
// /bin/tcsh
// /bin/zsh
/usr/local/bin/bash
```

#### Change shell
```
cssh -s /usr/local/bin/bash
```

#### Make .bash_profile & paste my config
https://github.com/toyamarodrigo/dotfiles/blob/master/.bash_profile
```
nano .bash_profile
```

---

### Albert3 configuration
**Turn off Spotlight**
*System Preference > Keyboard > Shortcut*

> Alfred hotkey ⌘ + Space

---

### Dock configuration
Get rid of everything, except the ones open and trash

*System Preference > Dock > Size Small*
> Position Right

> Hide Auto

---

### HyperSwitch configuration
*Preferences >*
> All Windows: ⌘ + TAB

> Current Windows: ⌥ + TAB

---

### Finder configuration
*Favorites >*

* Home folder
* Full Hard drive
* Applications
* Documents
* Pictures
* Music
* Downloads
* dev
* Airdrop

---

#### Install nvm/node

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```
```
nvm install stable
```
```
npm install -g lite-server eslint
```
---

### Visual Studio Code configuration

**Extensions and UserSettings Instalation**
https://github.com/toyamarodrigo/vscode-settings

#### Extensions

https://github.com/toyamarodrigo/vscode-settings/blob/master/Extensions.md

#### UserSettings.json

https://github.com/toyamarodrigo/vscode-settings/blob/master/UserSettings.json


**Thanks [w3cj](https://github.com/w3cj)**

**Youtube tutorial by w3cj**
https://www.youtube.com/watch?v=VC-pPFoW3zc
