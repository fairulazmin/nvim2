# Personnal Neovim preferences based on chrisatmachine config 

## Install Neovim

```sh
sudo apt install neovim
```
or
```sh
sudo add-apt-repository ppa:neovim-ppa/unstable
sudo apt-get update
sudo apt-get install neovim
```

## Install the config

Clone this repository

```sh
git clone https://github.com/fairulazmin/nvim2 ~/.config/nvim
```

Run `nvim`

Check health status

```sh
:checkhealth
```
Install `ripgrep` for Telescope to work:

```sh
sudo apt install ripgrep
```

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
