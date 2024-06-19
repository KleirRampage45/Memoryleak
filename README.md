Descripción del código:
Fuga de memoria:

Se crea una lista large_list que se llena continuamente con bloques de datos de 1 MB (bytearray(1024 * 1024)), lo que causa que el programa use cada vez más memoria sin liberarla.
Optimización deficiente:

El método waste_time realiza cálculos innecesarios en un bucle muy grande (for i in range(1000000)), lo que hace que el programa consuma mucho tiempo de CPU.
Monitoreo:

Se usa la biblioteca psutil para obtener el uso de memoria del proceso actual.
Se usa time.time() para medir el tiempo transcurrido.
Cada 100 iteraciones, se imprime el uso de memoria y el tiempo transcurrido en la consola.
Ejecución del código en Visual Studio Code
Para ejecutar este código en Visual Studio Code (VS Code), sigue estos pasos:

Paso 1: Instalar Python
Asegúrate de tener instalado Python. Puedes descargarlo desde el sitio web de Python.

Paso 2: Instalar Visual Studio Code
Descarga e instala Visual Studio Code desde el sitio web de VS Code.

Paso 3: Instalar la Extensión de Python
Abre VS Code y ve a la sección de extensiones (puedes abrirla presionando Ctrl+Shift+X). Busca e instala la extensión de Python proporcionada por Microsoft.

Paso 4: Instalar la Biblioteca psutil
Abre una terminal en VS Code (Ctrl+ñ en Windows o Ctrl+Shift+ en macOS) y ejecuta el siguiente comando para instalar la biblioteca psutil:

bash
Copiar código
pip install psutil
Paso 5: Crear un Nuevo Archivo Python
Crea un nuevo archivo llamado memory_leak_example.py:
bash
Copiar código
code memory_leak_example.py
Copia el código proporcionado anteriormente en el archivo memory_leak_example.py.
Paso 6: Ejecutar el Archivo Python
Abre una terminal en VS Code (Ctrl+ñ en Windows o Ctrl+Shift+ en macOS).
Ejecuta el archivo Python con el siguiente comando:
bash
Copiar código
python memory_leak_example.py
Esto ejecutará el programa y podrás ver en la consola la salida con el uso de memoria y el tiempo transcurrido. Verás cómo el programa consume cada vez más memoria y el tiempo de ejecución aumenta debido a la ineficiencia intencional del código.
