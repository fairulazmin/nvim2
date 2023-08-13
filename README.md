# Commands / Shortcuts

### NORMAL MODE
#### Window navigation
```
<Ctrl>+h            -   move the left
<Ctrl>+j            -   move down
<Ctrl>+k            -   move up
<Ctrl>+l            -   move to the right
```

#### Resize with arrow
```
<Ctrl>+Up           -   resize horizontally
<Ctrl>+Down         -   resize horizontally
<Ctrl>+Left         -   resize vertically
<Ctrl>+Right        -   resize vertically
```

#### Navigate buffer
```
<Shift>+l           -   navigate to the right
<Shift>+h           -   navigate to the left
```

#### Shortcut
```
<leader>+h          -   clear highlights
<leader>+c          -   close buffer
```

#### NvimTree
```
<leader>+e          -   toggle explorer
```

#### Telescope
```
<leader>+f          -   telescope find files
<leader>+F          -   telescope live grep
<leader>+P          -   telescope projects
<leader>+b          -   telescope buffers
```

#### LSP
```
gD                  -   declaration
gd                  -   definition
K                   -   hover
gI                  -   implementation
gr                  -   references
gl                  -   open float diagnostic
<leader>+lf         -   format
<leader>+li         -   LSP Info
<leader>+lI         -   installer info
<leader>+la         -   code action
<leader>+lj         -   go to next diagnostic
<leader>+lk         -   go to previous diagnostic
<leader>+lr         -   rename buffer
<leader>+ls         -   document symbols
<leader>+lq         -   quick fix
```

# How to install Neovim
## [Install wsl & Ubuntu](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#3-download-ubuntu)
Open Windows Command Prompt in administrator mode
```
wsl --install -d Ubuntu-20.04
```

Install the latest updates
```
sudo apt update && sudo apt upgrade -y
```

## Install Windows Terminal
Open Microsoft Store and install <strong>Windows Terminal</strong>

## Install Z shell
Install [Zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)
```
sudo apt-get install zsh
```

Install [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh)
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
Install [PowerLevel10k](https://github.com/romkatv/powerlevel10k)
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```
Install [Powerline](https://github.com/powerline/fonts) font
```
sudo apt-get install fonts-powerline
```
Install [FiraCode Nerd Font](https://github.com/ryanoasis/nerd-fonts/releases/download/v3.0.2/FiraCode.zip)

> Download and install for all users

Open <strong>zshrc</strong> file by typing `vim ~/.zshrc` and edit command as below
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
Install [zsh auto suggestion](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md)
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
Add the plugin to the list of plugins for Oh My Zsh
```
plugins=(git zsh-autosuggestions)
```

## Install Node.js & npm
```
sudo apt-get install -y nodejs npm
```
Check version
```
node -v && npm -v
```
## Install Neovim

```
sudo add-apt-repository ppa:neovim-ppa/unstable && sudo apt-get update && sudo apt-get install neovim
```

Clone this repository

```sh
git clone https://github.com/fairulazmin/nvim2 ~/.config/nvim
```

Install Packer
```
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
```

Install `ripgrep` for Telescope to work:

```
sudo apt install ripgrep
```

Run `nvim`

run `:PackerInstall`

run `:PackerUpdate`

run `:Mason` and install
```
autopep8
bash-language-server
css-lsp
html-lsp
json-lsp
prettier
pyright
tailwindcss-language-server
typescript-language-server
yaml-language server
```

Check health status
```
:checkhealth
```
