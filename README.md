# Fecha y Hora Actual - React App

Una aplicación simple en React que muestra la fecha y hora actual con un hermoso fondo azul degradado.

## Características

- Muestra la fecha actual en formato largo (español)
- Muestra la hora actual que se actualiza cada segundo
- Fondo azul degradado moderno
- Diseño responsivo
- Efecto de cristal esmerilado en el contenedor

## Instalación

1. Asegúrate de tener Node.js instalado en tu sistema
2. Instala las dependencias:
   ```bash
   npm install
   ```

## Ejecución

Para iniciar la aplicación en modo desarrollo:

```bash
npm start
```

La aplicación se abrirá automáticamente en tu navegador en `http://localhost:3000`

## Construcción

Para crear una versión optimizada para producción:

```bash
npm build
```

## Docker

Para construir y ejecutar la aplicación en un contenedor Docker:

### Construir la imagen Docker
```bash
docker build -t fecha-hora-react .
```

### Ejecutar el contenedor
```bash
docker run -p 8080:80 fecha-hora-react
```

La aplicación estará disponible en `http://localhost:8080`

### Construcción y ejecución con Docker Compose (opcional)
Si prefieres usar Docker Compose, puedes crear un archivo `docker-compose.yml`:

```yaml
version: '3.8'
services:
  app:
    build: .
    ports:
      - "8080:80"
    container_name: fecha-hora-react
```

Y ejecutar con:
```bash
docker-compose up -d
```

## Tecnologías utilizadas

- React 18.2.0
- React DOM 18.2.0
- React Scripts 5.0.1
- CSS3 con gradientes y efectos de glassmorphism

## Estructura del proyecto

```
src/
├── App.js          # Componente principal
├── App.css         # Estilos del componente principal
├── index.js        # Punto de entrada de React
└── index.css       # Estilos globales

public/
└── index.html      # Plantilla HTML
```
