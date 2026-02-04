# Proyecto Gemini API - Python

Este proyecto es una implementación base para interactuar con los modelos de inteligencia artificial de Google Gemini utilizando la librería oficial `google-genai`.

## 📋 Requisitos Previos

- Python 3.9 o superior.
- Una clave de API de Google Gemini (puedes obtenerla en [Google AI Studio](https://aistudio.google.com/)).

## 🛠️ Instalación y Configuración

Sigue estos pasos para poner en marcha el proyecto:

### 1. Clonar o descargar el proyecto
Asegúrate de estar en la carpeta raíz del proyecto (`gemini-api`).

### 2. Crear y activar un entorno virtual (Recomendado)
Es una buena práctica para mantener las dependencias aisladas.

```bash
# Crear el entorno virtual
python -m venv env

# Activar el entorno (Windows)
.\env\Scripts\activate

# Activar el entorno (Linux/Mac)
source env/bin/activate
```

### 3. Instalar dependencias
Instala las librerías necesarias ejecutando:

```bash
pip install -r requirements.txt
```

### 4. Configurar variables de entorno
Crea un archivo llamado `.env` en la raíz del proyecto (si no existe ya) y añade tu clave de API:

```env
GEMINI_API_KEY=tu_clave_aqui
```

## 🚀 Ejecución

El proyecto cuenta con dos scripts principales:

### Verificar el entorno
Para asegurarte de que el entorno virtual está activo y tienes conexión:
```bash
python pruebaentorno.py
```

### Ejecutar consulta a Gemini
Para probar la conexión con el modelo Gemini y recibir una respuesta:
```bash
python app_gemini.py
```

## 📁 Estructura del Proyecto

- `app_gemini.py`: Script principal que conecta con el modelo `gemini-3-flash-preview`.
- `pruebaentorno.py`: Utilidad para verificar la activación del entorno y conexión a red.
- `requirements.txt`: Lista de librerías de Python necesarias.
- `.env`: Archivo de configuración para la clave de API (no debe compartirse públicamente).
- `env/`: Carpeta del entorno virtual.

## 📄 Notas adicionales
- El script `app_gemini.py` utiliza actualmente el modelo `gemini-3-flash-preview`. Puedes cambiarlo en el código si deseas probar otros modelos disponibles.
