# Nvim-Setup
Setup Nvim in Linux local

## I. Install
### Download Neovim source code
```
git clone https://github.com/neovim/neovim.git 
mv neovim nvim
cd nvim
```
### Build Neovim
```
make CMAKE_BUILD_TYPE=Release
```
### Install Newovim locally
Need to choose path to install (bin) , using make + Tab to see option setup path
```
make install 
```
If have error, open file
```
vim build/cmake_install.cmake 
```
Change to true directory 

### Add Neovim to Path in shell
With .bashrc or .cshrc <br>
```
export PATH=$HOME/.local/nvim/build/bin:$PATH >> ~/.bashrc
source ~/.bashrc
```
With .cshrc 
```
set path = ($path $HOME/.local/nvim/build/bin) >> ~/.cshrc
source ~/.cshrc
```
### Check installation
```
nvim --version
```
## II. Setup
### Reference github to add config file
```
https://github.com/Dark-GreenCat/Neovim-Configuration.git
```
And add folder to .config with folder name is nvim

### Plugin 
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim 
:PlugInstall <br>

Run nvim


