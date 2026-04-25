# 🎥 Zoom Mass Downloader — Colab Edition

Este proyecto proporciona una solución automatizada e interactiva para descargar grabaciones de Zoom de forma masiva directamente a Google Drive utilizando Google Colab.

Es ideal para estudiantes, investigadores, docentes y profesionales que necesitan respaldar clases, reuniones o sesiones grabadas sin saturar su conexión local de internet ni ocupar almacenamiento en su computadora.

---

## ✨ Características principales

- **Descarga nube a nube:** los videos se descargan directamente desde Zoom hacia Google Drive.
- **Compatible con Google Colab:** no requiere instalación local.
- **Interfaz interactiva:** solicita carpeta de destino y permite subir el archivo de enlaces.
- **Nomenclatura personalizada:** cada video se guarda con el nombre definido por el usuario.
- **Detección de duplicados:** si el archivo ya existe, se omite automáticamente.
- **Motor `yt-dlp`:** utiliza una herramienta robusta para extraer y descargar videos.
- **Compatible con CSV y TXT:** detecta separadores por coma o tabulación.

---

## 📊 Formato del archivo de enlaces

Debes preparar un archivo `.csv` o `.txt` **sin encabezados** con dos columnas:

| Columna A | Columna B |
|---|---|
| Nombre del archivo | Enlace de Zoom |
| Clase_01_Introduccion | https://utec.zoom.us/rec/share/... |
| Clase_02_Machine_Learning | https://utec.zoom.us/rec/share/... |

Ejemplo:

```csv
Clase_01_Introduccion,https://utec.zoom.us/rec/share/...
Clase_02_Machine_Learning,https://utec.zoom.us/rec/share/...

---

## 🚀 Cómo utilizarlo

Sigue estos pasos para ejecutar el proyecto en Google Colab:

### 1. Crear entorno
- Ve a: https://colab.research.google.com/
- Crea un nuevo notebook.

### 2. Configurar el script
- Copia el código del proyecto en una celda.
- Ejecuta la celda (`▶ Run`).

### 3. Autenticación
- Autoriza el acceso a tu cuenta de Google Drive cuando se te solicite.

### 4. Configuración de descarga
- Ingresa el nombre de la carpeta donde deseas guardar los videos.

### 5. Subir archivo de enlaces
- Haz clic en **"Elegir archivos"**.
- Sube tu archivo `.csv` o `.txt` con los enlaces de Zoom.

### 6. Ejecución
- El script iniciará automáticamente la descarga secuencial.
- Los archivos se guardarán directamente en Google Drive.

---

## 🧪 Comandos clave

Durante la ejecución, se utilizan los siguientes comandos:

### Instalación de dependencias
```bash
pip install yt-dlp pandas

# Descarga de video
yt-dlp -o "ruta_de_salida/%(filename)s.%(ext)s" "URL_DEL_VIDEO"`

## 🛠️ Tecnologías utilizadas

- **Python 3**  
  Lenguaje principal utilizado para la ejecución del script en Google Colab.

- **yt-dlp**  
  Herramienta avanzada para la extracción y descarga de contenido multimedia desde múltiples plataformas, incluyendo enlaces de Zoom.

- **Pandas**  
  Librería utilizada para el procesamiento eficiente de archivos estructurados (CSV/TXT), permitiendo la lectura, limpieza y validación de datos.

- **Google Colab API**  
  Permite la ejecución del script en la nube, así como la interacción con archivos locales y la integración directa con Google Drive.

---

## ⚠️ Disclaimer

Este script debe ser utilizado únicamente para descargar contenido sobre el cual tengas derechos de acceso o autorización explícita del propietario.

El autor no se hace responsable por el uso indebido de esta herramienta, incluyendo —pero no limitado a— la descarga no autorizada de contenido protegido por derechos de autor.

El uso de este proyecto implica la aceptación de estas condiciones.

---
