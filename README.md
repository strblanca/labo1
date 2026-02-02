# laboratorio-1
"Infraestructura de microservicios con Docker, Portainer y Nginx Proxy Manager."


# Laboratorio de Microservicios y Orquestación Ligera con Docker

## 🚀 Descripción del Proyecto
Este repositorio contiene la configuración de un entorno de servicios virtualizados mediante contenedores. El objetivo principal es demostrar la capacidad de desplegar, gestionar y asegurar aplicaciones utilizando **Docker** y **Docker Compose**, optimizando el uso de recursos frente a la virtualización tradicional.

## 🛠️ Tecnologías Utilizadas
* **Docker & Docker Compose:** Para el empaquetado y despliegue de aplicaciones.
* **Portainer CE:** Interfaz de gestión visual para el control del ciclo de vida de los contenedores.
* **Nginx Proxy Manager:** Gestión de proxy inverso, terminación SSL y seguridad de red.
* **Ubuntu Server 22.04 LTS:** Sistema operativo base para el host de contenedores.

## 🏗️ Arquitectura del Laboratorio
El sistema está diseñado bajo una arquitectura de **Proxy Inverso**. 
1. El tráfico entra por los puertos estándar (80/443).
2. **Nginx Proxy Manager** actúa como puerta de enlace, dirigiendo el tráfico al contenedor correspondiente según el nombre de dominio o hostname.
3. **Portainer** permite la monitorización de logs, estados de salud (healthchecks) y consumo de recursos (CPU/RAM) de cada microservicio.

## 📦 Cómo desplegarlo
Para replicar este entorno en cualquier servidor con Docker instalado, ejecute:

```bash
git clone [URL_DE_TU_REPOSITORIO]
cd [NOMBRE_CARPETA]
docker-compose up -d
