# Linux

## Instalación Archlinux

### Script de instalación

### Paquetes a instalar
Principales:

alacritty arandr bat exa ffmpeg fish fzf git gst-plugins-ugly kitty luarocks ncdu neofetch nitrogen nvim pass pulseaudio ranger ripgrep ristretto rofi scrot thunar wget rust base-devel

Instalar gestor de paquetes AUR

```bash
git clone https://aur.archlinux.org/paru.git
cd paru
makepkg -si
```
Paquetes AUR:

slack zoom teams marktext-bin

[Marktext](https://github.com/marktext/marktext)

### Post instalación
Cambiar el shel principal por fish

```bash
chsh -s /usr/bin/fish
```

Paquete necesario para ~Ya no me acuerdo~

```bash
luarocks install luautf8
```

Bajar repositorio de contraseñasa. Setear variable de entorno PASSWORD_STORE_DIR e importar clave privada

```bash
gpg --decrypt file.gpg | gpg --import
export PASSWORD_STORE_DIR=~/dieworte/
```
o

```fish
gpg --decrypt file.gpg | gpg --import
set -Ux PASSWORD_STORE_DIR ~/repos/eb/dieworte
```

Aliases:

```bash
alias ll="exa --icons -l"
funcsave ll
alias ls="exa --icons"
funcsave ls
alias notas="nvim ~/repos/per/notas/index.md"
funcsave notas
```

Descargar repositorio de configuraciones y linkear dotfiles

```bash
git clone http://github.com/estebanber/archlinux ~/repo/per/archlinux --recursive
cd ~/.config
ln -s ~/repos/per/archlinux/dotfiles/kitty kitty
ln -s ~/repos/per/archlinux/dotfiles/alacritty alacritty
ln -s ~/repos/per/archlinux/dotfiles/awesome/ ~/.config/
```
nvim config

### Configuración Neovim
- "nvim-tree/nvim-web-devicons"
- "nvim-lua/plenary.nvim"
- 'hrsh7th/nvim-cmp'
- "nvim-neo-tree/neo-tree.nvim"
- "MunifTanjim/nui.nvim",
- "neovim/nvim-lspconfig"
- 'jakewvincent/mkdnflow.nvim',
- 'nvim-telescope/telescope.nvim',
