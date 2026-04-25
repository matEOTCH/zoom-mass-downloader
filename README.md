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
