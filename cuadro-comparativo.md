# Cuadro comparativo del instalador

Comparación entre las dos distribuciones usadas en el proyecto: **Fedora Workstation 45** (VM gráfica `g03-grafica`) y **Ubuntu Server 26.04 LTS** (VM consola `g03-consola`).

| Aspecto | Fedora Workstation 45 (`g03-grafica`) | Ubuntu Server 26.04 LTS (`g03-consola`) |
|---|---|---|
| **Instalador** | Anaconda | Subiquity |
| **Herramienta de particionado** | Anaconda (Manual Partitioning) | Subiquity (Custom storage layout) |
| **Comando para instalar paquetes** | `dnf install` | `apt install` |
| **Comando para actualizar paquetes** | `dnf update` | `apt update && apt upgrade` |
| **Firewall** | `firewalld` | `ufw` |
| **Grupo de administradores** | `wheel` | `sudo` |
| **Comando para iniciar/detener servicios** | `systemctl start/stop` | `systemctl start/stop` |
| **Sistema de archivos por defecto** | Btrfs | ext4 |
| **Instalación desatendida** | Kickstart | Autoinstall (cloud-init) |

---

## Notas

- **Instalador:** Fedora usa Anaconda, que permite particionado manual en "Manual Partitioning". Ubuntu Server usa Subiquity, que permite particionado manual en "Custom storage layout".
- **Gestor de paquetes:** Fedora usa `dnf` (familia Red Hat); Ubuntu usa `apt` (familia Debian). No son intercambiables.
- **Firewall:** Fedora usa `firewalld`; Ubuntu usa `ufw`. En el proyecto, la configuración del firewall se hace en `g03-consola` con `ufw`.
- **Grupo de administradores:** En Fedora el grupo es `wheel`; en Ubuntu es `sudo`.
- **Sistema de archivos:** Fedora Workstation usa Btrfs por defecto; Ubuntu Server usa ext4.
- **Instalación desatendida:** Ambas distribuciones ofrecen métodos desatendidos (Kickstart en Fedora, Autoinstall en Ubuntu), pero el proyecto usa la instalación manual.

---

## Fuentes consultadas

- Documentación oficial de Fedora: `https://docs.fedoraproject.org/`
- Documentación oficial de Ubuntu Server: `https://ubuntu.com/server/docs`
- Guía 2 del curso: Particionamiento y Sistemas de Archivos.
- Guía 3 del curso: Instalación, Particionado y Desatendida.
- Guía de Investigación Técnica por Distribución.
