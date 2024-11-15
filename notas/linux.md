# .Dotfiles
Crear un sistema para administrar los dotfiles. De forma de tenerlos en un repositorio. Y poder replicar mi configuración rapidamente en cualquier computadora.
quisiera contar con configuraciónes para varios windows manager, como son: Awesome WM, dwm, Hyprland y Qtile.

# Scripts
Para simplificar algunas tareas reptitivas que tengo que realizar al cambiar de contexto (trabajo freelance, diseño de hardware. trabajo, fotografía, etc.) la idea es crear scripts que ejecuten y preparen el entorno necesario. Estos script pueden diferencia si estamos en un entorno de solo consola o en un entorno gráfico. Crear launcher rofi (o uno específico del WM) para simplificar el llamdo de los diferentes scripts.

Script para commitear y pushear contraseñas


# Repositorios y colecciones
Debo crear repositorio y/o colecciones centralizadas de los siguientes recursos.
- Imagenes
- Fotos
- Libros
- Comics

Teniendo estos repositorios es mucho mas facil hubicar recursos y crear backups.

# Herramientas a probar
- Yazi
- Qtile
- Hyprland

# Nuevo proceso de instalación
1. Scripts de instalación (durante chroot)
2. Scripts de instalación (dentro del sistema)
3. Clonar repositorio de scripts
4. Descargar y configurar certificados git
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

