🎥 Zoom Mass Downloader (Colab Edition)
Este proyecto proporciona una solución automatizada e interactiva para descargar grabaciones de Zoom de forma masiva directamente a Google Drive utilizando la potencia de Google Colab.

Ideal para estudiantes, investigadores y profesionales que necesitan respaldar clases o reuniones sin saturar su conexión local de internet ni el almacenamiento de su computadora.

✨ Características principales
Integración con Google Drive: Descarga de "nube a nube", ahorrando tus datos locales.

Interfaz Interactiva: El script te solicita el nombre de la carpeta de destino y te permite subir el archivo de enlaces directamente.

Nomenclatura Personalizada: Los videos se guardan con los nombres que tú definas en tu lista.

Detección de Duplicados: Si una descarga se interrumpe o el archivo ya existe, el script lo salta automáticamente para ahorrar tiempo.

Motor yt-dlp: Utiliza una de las herramientas de extracción de video más potentes para manejar enlaces de Zoom.

📊 Preparación del archivo (CSV/TXT)
Para que el script funcione correctamente, debes preparar un archivo con la lista de videos. El script detecta automáticamente si usas comas (CSV) o tabulaciones (TXT).

Formato requerido:

El archivo no debe tener encabezados (headers) y debe seguir esta estructura de dos columnas:

Columna A (Nombre del archivo)	Columna B (Enlace de Zoom)
Clase_01_Introduccion	https://utec.zoom.us/rec/share/...
Clase_02_Machine_Learning	https://utec.zoom.us/rec/share/...
Nota: No incluyas caracteres especiales prohibidos en nombres de archivos (como \ / : * ? " < > |). El script limpiará el nombre automáticamente, pero es mejor ser precavido.

🚀 Cómo utilizarlo
Crea un nuevo cuaderno en Google Colab.

Copia el código del script en una celda.

Ejecuta la celda (Play).

Sigue las instrucciones en pantalla:

Conecta tu cuenta de Google Drive cuando se te solicite.

Escribe el nombre de la carpeta donde quieres guardar los videos.

Haz clic en el botón "Elegir archivos" para subir tu archivo de enlaces.

¡Listo! El script comenzará la descarga secuencial.

🛠️ Tecnologías utilizadas
Python 3

yt-dlp: Para la extracción y descarga del flujo de video.

Pandas: Para el procesamiento eficiente de la lista de enlaces.

Google Colab API: Para la interacción con archivos locales y Drive.

⚠️ Disclaimer
Este script debe ser utilizado únicamente para descargar contenido sobre el cual tengas derechos de acceso o permiso del propietario. El autor no se hace responsable por el mal uso de esta herramienta.
