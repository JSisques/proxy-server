![Banner](./img/proxy-server.png)

# Proxy Server

## 📜 Descripción del Proyecto

El propósito principal de este proyecto es permitir el acceso a los servicios de una red privada, como Grafana o Portainer, utilizando nombres de dominio en lugar de direcciones IP. Este proyecto se basa en el uso de Duck DNS para gestionar los dominios.

## 🔧 Requisitos Previos

Antes de empezar, asegúrate de tener los siguientes requisitos:

- Un sistema operativo compatible con Docker.
- Un script de "puesta a punto" (setup.sh) para instalar la última versión de Docker.

## 📦 Instrucciones de Instalación y Uso

### Clonar el Repositorio

Primero, clona el repositorio a tu máquina local:

```bash
git clone https://github.com/tu-usuario/proxy-server.git
cd proxy-server
```

### Ejecutar el Script de Puesta a Punto

El archivo setup.sh ya está creado en la carpeta ./scripts. Solo necesitas ejecutarlo para instalar Docker y Docker Compose:

```bash
cd scripts
chmod +x setup.sh
./setup.sh
```

### Construir y Ejecutar el Contenedor

Construye y ejecuta el contenedor usando Docker Compose:

```bash
docker-compose up -d
```

### Configurar y Usar Duck DNS

Sigue las instrucciones en Duck DNS para configurar tu dominio y apuntarlo a la IP de tu servidor.

### Acceder al Administrador del Proxy

Accede al administrador del proxy en http://tu-ip:81. Por defecto, las credenciales para acceder al panel de administración son las siguientes:

- Email address: `admin@example.com`
- Password: `changeme`

Asegúrate de cambiar estas credenciales después del primer acceso para mantener la seguridad.

## 📄 Licencia

Este proyecto está licenciado bajo la GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007.

## ✍️ Autoría y Contribución

- Autor: Javier Plaza Sisqués
- GitHub: [JSisques](https://github.com/JSisques)

### Cómo Contribuir

Las contribuciones son bienvenidas. Por favor, abre un issue o envía un pull request para contribuir a este proyecto.
