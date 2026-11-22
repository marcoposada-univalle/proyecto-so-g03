# Glosario de términos del proyecto

Este glosario reúne los términos que aparecen en el proyecto final y que es necesario entender para desarrollarlo y sustentarlo.

---

## A

**Anaconda:** Instalador de Fedora Workstation. Permite el particionado manual a través de la opción "Manual Partitioning".

**APT:** Gestor de paquetes de la familia Debian/Ubuntu. Se usa en `g03-consola` con comandos como `apt install`, `apt update`, `apt upgrade`.

---

## B

**Btrfs:** Sistema de archivos por defecto de Fedora Workstation. Soporta instantáneas (copy-on-write).

---

## C

**Commit:** Guardado de un cambio en el historial del repositorio, con autor, fecha y mensaje. El proyecto exige mínimo 2 commits por integrante por sprint (6 en total en sprints 1, 2 y 3).

**Contenedor:** Instancia en ejecución de una imagen Docker. Comparte el kernel del anfitrión y se aísla del resto del sistema.

---

## D

**DNF:** Gestor de paquetes de la familia Fedora/RHEL. Se usa en `g03-grafica` con comandos como `dnf install`, `dnf update`.

**Docker:** Plataforma para empaquetar y ejecutar aplicaciones en contenedores.

**Docker Engine:** Motor de Docker. Se instala en `g03-consola` con la guía oficial de Ubuntu.

**Docker Hub:** Registro público de imágenes Docker. Allí se publica la imagen propia del proyecto (`marco/g03-fedora:v1`).

**Dockerfile:** Archivo de texto con las instrucciones para construir una imagen Docker. En el proyecto, parte de la imagen base Fedora 45.

---

## E

**ext4:** Sistema de archivos por defecto de Ubuntu Server. Es estable y ampliamente usado en servidores.

---

## F

**Fedora Workstation:** Distribución Linux con entorno gráfico asignada para `g03-grafica`. Versión elegida: Fedora 45.

**firewalld:** Firewall por defecto de Fedora. Se usa en `g03-grafica` (aunque la configuración principal del proyecto se hace en la consola con `ufw`).

---

## G

**GitHub:** Plataforma para alojar repositorios Git. El proyecto se entrega en un repositorio público.

**GitHub Pages:** Servicio de GitHub que publica los archivos del repositorio como un sitio web. El sitio del proyecto se publica con GitHub Pages.

---

## H

**Hostname:** Nombre del equipo. En el proyecto, `g03-grafica` y `g03-consola`.

---

## I

**Imagen:** Plantilla de solo lectura para crear contenedores. Se construye con `docker build` a partir de un Dockerfile.

**Inodo:** Estructura del sistema de archivos que guarda los metadatos de un archivo (dueño, permisos, tamaño, ubicación de bloques). No guarda el nombre.

---

## K

**Kubernetes:** Sistema de orquestación de contenedores. En el proyecto se usa Minikube para desplegar la imagen propia con 2 réplicas, escalar a 4 y borrar un pod.

---

## M

**MBR:** Tabla de particiones clásica (1983). Máximo 4 particiones primarias y discos de hasta 2 TB. Se usa con BIOS.

**Minikube:** Versión local de Kubernetes que corre en una sola máquina. En el proyecto se instala en `g03-consola` y se arranca con `minikube start --driver=docker` (sin sudo).

---

## N

**NAT:** Modo de red de VirtualBox que da internet a la VM pero no permite que las VMs se vean entre sí. En el proyecto, el Adaptador 1 está en NAT.

---

## P

**Partición:** División del disco. En el proyecto: `/`, `swap`, `/home` (en ambas VMs) y `/var` (solo en la consola).

**Pod:** Unidad mínima de Kubernetes. Contiene uno o más contenedores. El proyecto usa pods con la imagen `marco/g03-fedora:v1`.

---

## R

**ReplicaSet:** Controlador de Kubernetes que garantiza que el número deseado de réplicas de un pod esté siempre corriendo. Recrea los pods cuando se borran.

**Repositorio:** Carpeta del proyecto en GitHub con el historial de cambios. El del proyecto es `https://github.com/marcoposada-univalle/proyecto-so-g03`.

---

## S

**Sprint:** Periodo corto de trabajo con una meta y una entrega. El proyecto tiene 4 sprints más la sustentación.

**Subiquity:** Instalador de Ubuntu Server. Permite el particionado manual a través de "Custom storage layout".

**Swap:** Espacio de intercambio en disco que apoya a la RAM. En el proyecto: 2 GB en la consola, 4 GB en la gráfica.

---

## T

**Tabla de particiones:** Índice del disco que dice dónde empieza y termina cada partición. Puede ser MBR o GPT.

---

## U

**Ubuntu Server:** Distribución Linux sin entorno gráfico asignada para `g03-consola`. Versión elegida: Ubuntu Server 26.04 LTS.

**UFW:** Firewall por defecto de Ubuntu. Se activa con `ufw enable`, se permite SSH con `ufw allow ssh` y se abre el puerto 8080 con `ufw allow 8080`.

---

## V

**VirtualBox:** Software de virtualización para crear y ejecutar máquinas virtuales. En el proyecto se usan dos VMs: `g03-grafica` y `g03-consola`.

**VM (máquina virtual):** Computador simulado que ejecuta un sistema operativo completo. En el proyecto, las dos VMs Linux.

---

## W

**WSL 2:** Subsistema de Windows para Linux. Permite ejecutar Linux dentro de Windows sin VirtualBox. Entra al Parcial 2, pero no se usa en el proyecto final.

---

## X

**XFS:** Sistema de archivos usado por Red Hat, Rocky, AlmaLinux y Fedora Server. Solo se puede ampliar, no reducir.
