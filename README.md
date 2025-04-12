# Nvim-Setup
Setup Nvim in Linux local

## I. Install
### Download Neovim source code
```
git clone https://github.com/neovim/neovim.git <br>
mv neovim nvim
cd nvim
```
### Build Neovim
```
make CMAKE_BUILD_TYPE=Release
```
### Install Newovim locally
```
make install
```
If have error, open file
```
vim build/cmake_install.cmake 
```
Change to true directory 

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
## II. Setup
### Reference github to add config file
https://github.com/Dark-GreenCat/Neovim-Configuration.git

### Plugin 
curl -fLo ~/.local/share/nvim/site/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim <br>
:PlugInstall <br>

Run nvim


