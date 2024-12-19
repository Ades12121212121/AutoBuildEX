Descripción:

Descripción general de la aplicación:
Es un convertidor de archivos Python a ejecutables EXE utilizando la biblioteca PyInstaller.
Proporciona una interfaz gráfica para simplificar el proceso de conversión.
Permite a los usuarios configurar opciones como el nombre del archivo EXE, el icono, la imagen y la visualización de la consola.
Funcionalidades:

**Interfaz Gráfica de Usuario (GUI):**

Utiliza PyQt6 para crear una ventana con campos de texto para ingresar información y botones para interactuar.
Presenta un estilo oscuro moderno.
Funcionalidades de la GUI:

Seleccionar Archivo Python:
Permite al usuario seleccionar el archivo Python que desea convertir a EXE a través de un cuadro de diálogo de selección de archivos.
Seleccionar Icono:
Permite al usuario seleccionar un archivo de icono (.ico) para el EXE.
Seleccionar Imagen:
Permite al usuario seleccionar una imagen (.png) que será incluida en el paquete EXE.
Opción de Consola:
Proporciona un checkbox para elegir si el EXE mostrará una ventana de consola.
Convertir a EXE:
Ejecuta PyInstaller con los parámetros configurados por el usuario.
Genera un archivo EXE en el directorio actual.
Muestra un mensaje de éxito o error al finalizar la conversión.
Detalles del código:

Imports: Importa las bibliotecas necesarias: os, subprocess, PyQt6.
Clase PyToExeApp: Define la ventana principal de la aplicación:
__init__: Inicializa la ventana, establece el título y el tamaño, declara variables para almacenar la información del usuario.
set_style: Define el estilo de la GUI, incluyendo colores y estilos de elementos como botones y etiquetas.
init_ui: Crea la interfaz de usuario con:
Una etiqueta de título.
Un formulario con:
Un campo de texto para el nombre del archivo EXE.
Botones para seleccionar el archivo Python, el icono y la imagen.
Checkbox para mostrar/ocultar la consola.
