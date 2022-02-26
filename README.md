# My Itrem Customisation 

## iTerm2
https://www.iterm2.com

Install with:

```sh 
brew cask install iterm2 
```

After installation, close the terminal. You will need to provide full disk access to iTerm2. System Preferences -> Security and Privacy -> Full Disk Access, click the + icon and select iTerm2 from the Applications folder.

## Zsh
https://ohmyz.sh

Install with:

```sh 
brew install zsh 
```

Check the version of zsh: zsh --version Make zsh default shell: chsh -s /bin/zsh Check the shell you're using: echo $SHELL

## Oh My Zsh
https://ohmyz.sh

Install with:

```sh  
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"  
```

Powerlevel9k
https://github.com/bhilburn/powerlevel9k

Install with:

```sh 
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
```

Edit ~/.zshrc and set as default theme:

ZSH_THEME="powerlevel9k/powerlevel9k"

Install the font:
```sh 
https://github.com/powerline/fonts/blob/master/SourceCodePro/Source%20Code%20Pro%20for%20Powerline.otf
``` 
Open with FontBook, and click Install.

Set the font iTerm, make sure size is 14pt: iTerm → Preferences → Profiles → Text → Change Font

## Iterm theme 

Iterm theme colours 
https://iterm2colorschemes.com/

Save as: selected-theme.itermcolors
Configure the theme in iTerm: iTerm2 -> Preferences -> Profiles -> Colors -> Color Presets -> Import and select the file.
Select selected-theme from the dropdown.

## zsh Auto Suggestions
Install with:

```sh 
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

Add the plugin to ~/.zshrc:

```sh 
plugins=(
  git zsh-autosuggestions
)
```
Tweak the color solarize theme: iTerm → Preferences → Profiles → Colors tab", change the value of Black Bright to a lighter color.

## Syntax Highlighting
Install with:

https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md#oh-my-zsh

Add the plugin to ~/.zshrc:

```sh 
plugins=( [plugins...] zsh-syntax-highlighting)
```sh 

## History
Install with:

https://github.com/junegunn/fzf#using-homebrew

Run this command

```sh
$(brew --prefix)/opt/fzf/install
```
Press **Y** for the next 3 steps 

To start press `control + r`

## Change user name 

Go to file `powerlevel9k.zsh-theme`

find the line

```sh
set_default POWERLEVEL9K_CONTEXT_TEMPLATE "%n@%m"
```
to 
```sh
set_default POWERLEVEL9K_CONTEXT_TEMPLATE "%n"
```

## Word Jumps
Enable word jumps: iTerm → Preferences → Profiles → Keys → Load Preset and select Natural Text Editing

Change the username@hostname
whoam to check your username
wh
Edit ~/.zshrc

Add:

DEFAULT_USER = <username>

## Configure VS Code
Go to Settings: terminal.integrated.fontFamily: Source Code Pro for Powerline

## Git

Customize git commmands

```sh 
alias | grep git
```
