# .Dotfiles
Crear un sistema para administrar los dotfiles. De forma de tenerlos en un repositorio. Y poder replicar mi configuración rapidamente en cualquier computadora.
quisiera contar con configuraciónes para varios windows manager, como son: Awesome WM, dwm, Hyprland y Qtile.

# Scripts
Para simplificar algunas tareas reptitivas que tengo que realizar al cambiar de contexto (trabajo freelance, diseño de hardware. trabajo, fotografía, etc.) la idea es crear scripts que ejecuten y preparen el entorno necesario. Estos script pueden diferencia si estamos en un entorno de solo consola o en un entorno gráfico. Crear launcher rofi (o uno específico del WM) para simplificar el llamdo de los diferentes scripts.

Script para commitear y pushear contraseñas

# Herramientas a probar
- Yazi
- Qtile
- Hyprland

# Fuera de los repositorios oficiales
Paquetes AUR: slack zoom teams tty-clock cava
[Marktext](https://github.com/marktext/marktext)

# Nuevo proceso de instalación
1. Scripts de instalación (durante chroot)
    a. Junto a los scripts de instalación hay un archivo con todos los paquetes basicos y diferentes categorías.
3. Scripts de instalación (dentro del sistema)
4. Clonar repositorio de scripts
5. Descargar y configurar certificados git
    ~/.ssh/nombre
    ~/.ssh/nombre.pub
    ~/.ssh/config

```
Host github.com
  User git
  IdentityFile ~/.ssh/nombre
```
5. Crear estructura de repositorios
    per/
    pro/
    3rd/
```
./myrepos.sh crear_estructura ~/repos
./myrepos.sh clonar_personal ~/repos
```
6. Linkear dotfiles a .config
7. Configuraciones importante

Cambiar el shel principal por fish

```bash
chsh -s /usr/bin/fish
```
Bajar repositorio de contraseñas. Setear variable de entorno PASSWORD_STORE_DIR e importar clave privada

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
