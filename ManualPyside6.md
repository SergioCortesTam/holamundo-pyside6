# Hola Mundo con PySide6

Este repositorio contiene una aplicación simple de "Hola Mundo" utilizando PySide6. A continuación, encontrarás las instrucciones para instalar y ejecutar la aplicación en Windows y Linux. Prueba2


## Requisitos

- Python 3.x
- pip

## Instalación y Configuración

### 1. Instalación de Python 3 y pip

#### Windows
Descarga e instala Python desde [python.org](https://www.python.org/downloads/). Asegúrate de seleccionar la opción "Add Python to PATH" durante la instalación.

Para verificar la instalación, ejecuta en la terminal (cmd o PowerShell):
```sh
python --version
pip --version
```

#### Linux
Instala Python3 y pip utilizando el gestor de paquetes de tu distribución:
```sh
sudo apt update && sudo apt install python3 python3-pip -y  # Para Debian/Ubuntu
sudo dnf install python3 python3-pip -y  # Para Fedora
```

Verifica la instalación:
```sh
python3 --version
pip3 --version
```

### 2. Creación y Activación de un Entorno Virtual

#### Windows
```sh
python -m venv venv
venv\Scripts\activate
```

#### Linux
```sh
python3 -m venv venv
source venv/bin/activate
```

### 3. Instalación de Dependencias

Con el entorno virtual activado, instala PySide6:
```sh
pip install PySide6
```

### 4. Creación de la Aplicación "Hola Mundo"

Crea un archivo `main.py` y agrega el siguiente código:

```python
from PySide6.QtWidgets import QApplication, QLabel
import sys

app = QApplication(sys.argv)
window = QLabel('¡Hola, Mundo!')
window.show()
sys.exit(app.exec())
```

### 5. Ejecución de la Aplicación

#### Windows
```sh
python main.py
```

#### Linux
```sh
python3 main.py
```

¡Listo! Ahora deberías ver una ventana con el mensaje "¡Hola, Mundo!".
