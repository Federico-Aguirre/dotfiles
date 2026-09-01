# Dotfiles & Linux Setup

Repositorio personal con configuraciones de entorno para Linux/WSL2.

## Contenido
- `bashrc`: Alias y atajos personalizados para la terminal.
- `gitconfig`: Configuración global de Git (nombre, email).
- `install.sh`: Script para vincular los archivos mediante enlaces simbólicos.

## Instalación en una máquina nueva

```bash
# 1. Instalar GitHub CLI e iniciar sesión
sudo apt update && sudo apt install gh -y
gh auth login

# 2. Clonar dotfiles
git clone [https://github.com/Federico-Aguirre/dotfiles.git](https://github.com/Federico-Aguirre/dotfiles.git) ~/dotfiles

# 3. Vincular configuraciones
cd ~/dotfiles
chmod +x install.sh
./install.sh
source ~/.bashrc
