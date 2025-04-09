# Nvim-Setup
Setup Nvim in Linux local

## Install
### Download Neovim source code
```
git clone https://github.com/neovim/neovim.git <br>
cd neovim
```
### Build Neovim
```
make CMAKE_BUILD_TYPE=Release
```
### Install Newovim locally
```
make install
```
### Add Neovim to Path in shell
With .bashrc or .zshrc <br>
```
export PATH=$HOME/neovim/bin:$PATH >> ~/.bashrc <br>
source ~/.bashrc <br>
```
With .cshrc 
```
set path = ($path $HOME/nvim/bin)
```
### Check installation
```
nvim --version
```
## Setup
### Reference github to add config file
https://github.com/Dark-GreenCat/Neovim-Configuration.git

### Plugin 
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim <br>
:PlugInstall <br>

Run nvim

## Issue 
If run have fail usr/local/
=> /u/lethanh/.local/nvim/share/
