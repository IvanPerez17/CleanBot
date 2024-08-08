# Proyecto de Asistente Virtual

Este proyecto implementa un asistente virtual que ayuda a dar recomendaciones de productos de limpieza en una página web de ventas. Utiliza un modelo de lenguaje llamado `llama3` y se despliega utilizando Docker y Gradio.

## Estructura del Proyecto

## Requisitos

- Docker
- Docker Compose
- Python 3.x
- Librerías Python: [`requests`], [`json`], [`gradio`]

## Uso

1. Clona este repositorio en tu máquina local.
2. Navega al directorio del proyecto.

```sh
cd tu-directorio-del-proyecto
```
3. Construye y levanta los servicios de Docker.

```sh
docker-compose up --build
```
4. Asegúrate de descargar el modelo llama3 si no está disponible.

```sh
docker-compose exec ollama ollama pull llama3
```
5. Abre tu navegador y navega a http://localhost:7860 para interactuar con el asistente virtual.

## Archivos Importantes

`main.py`: Contiene el código principal para la interfaz de usuario y la generación de respuestas.

`Modelfile`: Configuración del modelo llama3.

`docker-compose.yaml`: Configuración de los servicios Docker necesarios para ejecutar el proyecto.

## Licencia

Este proyecto está licenciado bajo los términos de la licencia MIT.