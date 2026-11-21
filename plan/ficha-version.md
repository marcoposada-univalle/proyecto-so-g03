# Ficha de verificación de versión · Grupo 03

---

## 1. Fedora Workstation (VM gráfica `g03-grafica`)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión elegida y fecha de lanzamiento | Fedora Workstation 45, lanzada el 3 de noviembre de 2026 | https://fedoraproject.org/es/workstation/download/ |
| Hasta cuándo recibe actualizaciones de seguridad | Hasta el 8 de diciembre de 2027 | https://www.csirt-bfc.fr/eol/fedora.html |
| Requisitos de hardware y si funciona en VirtualBox | 40 GB de disco y 4 GB de RAM recomendados; funciona en VirtualBox | https://fedoraproject.org/es/workstation/download/   https://packages.fedoraproject.org/pkgs/virtualbox-guest-additions/virtualbox-guest-additions/ |
| ¿El instalador permite particionado manual? | Sí, Anaconda ofrece "Manual Partitioning" (particionado manual) | https://docs.fedoraproject.org/en-US/fedora/latest/ |
| ¿Existe guía oficial para instalar Docker Engine? | Sí, Docker soporta oficialmente Fedora 45 | https://docs.docker.com/engine/install/fedora/ |
| ¿Existe la imagen base del Dockerfile para esa versión? | Sí, `fedora:latest` apunta a la última versión estable | https://hub.docker.com/_/fedora |

---

## 2. Ubuntu Server (VM consola `g03-consola`)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión elegida y fecha de lanzamiento | Ubuntu Server [versión LTS, ej: 24.04 LTS], lanzada el [fecha] | https://ubuntu.com/download/server |
| Hasta cuándo recibe actualizaciones de seguridad | [fecha, ej: 5 años para LTS] | https://ubuntu.com/about/release-cycle |
| Requisitos de hardware y si funciona en VirtualBox | [RAM, disco, CPU] | https://ubuntu.com/server/docs |
| ¿El instalador permite particionado manual? | Sí, Subiquity → "Manual" | https://ubuntu.com/server/docs |
| ¿Existe guía oficial para instalar Docker Engine? | Sí | https://docs.docker.com/engine/install/ubuntu/ |
| ¿Existe la imagen base del Dockerfile para esa versión? | Sí, `ubuntu:latest` | https://hub.docker.com/_/ubuntu |

---

## 3. Fedora (imagen base del Dockerfile)

| Pregunta | Respuesta | Enlace |
|---|---|---|
| Versión elegida y fecha de lanzamiento | Fedora [versión, ej: 43] | https://hub.docker.com/_/fedora |
| Hasta cuándo recibe actualizaciones de seguridad | [fecha aproximada] | https://fedoraproject.org/wiki/Releases |
| Requisitos de hardware y si funciona en VirtualBox | N/A (es imagen de contenedor) | https://hub.docker.com/_/fedora |
| ¿El instalador permite particionado manual? | N/A (no aplica a contenedor) | — |
| ¿Existe guía oficial para instalar Docker Engine? | Sí | https://docs.docker.com/engine/install/fedora/ |
| ¿Existe la imagen base del Dockerfile para esa versión? | Sí, `fedora:latest` | https://hub.docker.com/_/fedora |
