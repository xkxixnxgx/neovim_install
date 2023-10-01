# neovim_install
Configuration file and installation guide

## Go to `https://github.com/neovim/neovim/releases/tag/stable` and load `nvim-linux64.tar.gz`
```bash
wget -O ~/nvim-linux64.tar.gz https://github.com/neovim/neovim/releases/download/stable/nvim-linux64.tar.gz
sha256sum ~/nvim-linux64.tar.gz
tar xzvf ~/nvim-linux64.tar.gz
sudo ln -s  ~/nvim-linux64/bin/nvim /usr/bin/nvim
nvim

mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
mv ~/.local/state/nvim ~/.local/state/nvim.bak
mv ~/.cache/nvim ~/.cache/nvim.bak
git clone --depth 1 https://github.com/AstroNvim/AstroNvim ~/.config/nvim
git clone https://github.com/xkxixnxgx/nvim_config ~/.config/nvim/lua/xkxixnxgx
nvim

```


