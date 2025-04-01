# Nvim-Setup
Setup Nvim in Linux local

## Install
### Download Neovim source code
git clone https://github.com/neovim/neovim.git
cd neovim

### Build Neovim
make CMAKE_BUILD_TYPE=Release

### Install Newovim locally
make install

### Add Neovim to Path in shell
With .bashrc or .zshrc
export PATH=$HOME/neovim/bin:$PATH >> ~/.bashrc 
source ~/.bashrc

With .cshrc 
set path = ($path $HOME/nvim/bin)

### Check installation
nvim --version

## Setup
### Reference to github 
https://github.com/Dark-GreenCat/Neovim-Configuration.git

### Plugin 
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
:PlugInstall

Run nvim
