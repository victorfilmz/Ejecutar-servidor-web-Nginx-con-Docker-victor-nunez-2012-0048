# Práctica 6: Ejecutar Servidor Web Nginx con Docker

## 📌 Descripción

Esta práctica consiste en configurar y ejecutar un servidor web **Nginx** local utilizando contenedores mediante **Docker Compose**. Los archivos estáticos se administran desde el directorio local `src/` y se conectan en tiempo real al directorio raíz web del contenedor (`/usr/share/nginx/html`) mediante un volumen montado en modo solo lectura (`:ro`).

---

## 🎯 Objetivos de la Práctica

- Configurar un entorno local con contenedores usando **Docker Compose**.
- Servir contenido HTML estático personalizado a través de **Nginx Alpine**.
- Implementar el mapeo de volúmenes locales al sistema de archivos del contenedor.
- Administrar el ciclo de vida de los contenedores mediante la CLI de Docker.

---

## 📂 Estructura del Proyecto

```text
.
├── docker-compose.yml   # Archivo de definición del servicio Nginx y volúmenes
├── README.md            # Documentación y guía de ejecución
└── src/
    └── index.html       # Página web principal personalizada con estilo moderno
```

---

## 🚀 Instrucciones de Ejecución

### Requisitos Previos
Tener instalado y en ejecución [Docker Desktop](https://www.docker.com/products/docker-desktop/).

### Pasos

1. **Clonar este repositorio:**
   ```bash
   git clone https://github.com/victorfilmz/Ejecutar-servidor-web-Nginx-con-Docker-victor-nunez-2012-0048.git
   cd Ejecutar-servidor-web-Nginx-con-Docker-victor-nunez-2012-0048
   ```

2. **Iniciar el servidor web en segundo plano:**
   ```bash
   docker compose up -d
   ```

3. **Verificar el estado del contenedor:**
   ```bash
   docker compose ps
   ```

4. **Acceder en el navegador:**
   Ingresa a: [http://localhost:8080](http://localhost:8080)

5. **Detener el servidor:**
   ```bash
   docker compose down
   ```

---

## 👨‍💻 Autor

- **Nombre:** Víctor Núñez
- **Matrícula:** 2012-0048
