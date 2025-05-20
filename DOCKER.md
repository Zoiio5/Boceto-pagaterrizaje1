# Instrucciones para Dockerizar la Aplicación

## Requisitos Previos
- Docker instalado
- Docker Compose instalado (opcional)

## Construcción y Ejecución

### Usando Docker directamente

1. Construir la imagen:
```bash
docker build -t pw-landing .
```

2. Ejecutar el contenedor:
```bash
docker run -p 80:80 pw-landing
```

La aplicación estará disponible en: http://localhost

### Usando Docker Compose

1. Ejecutar la aplicación:
```bash
docker-compose up -d
```

2. Detener la aplicación:
```bash
docker-compose down
```

## Personalización

- El Dockerfile utiliza Nginx para servir la aplicación estática
- La configuración de Nginx se puede personalizar según sea necesario
- Los archivos estáticos se sirven desde `/usr/share/nginx/html` 