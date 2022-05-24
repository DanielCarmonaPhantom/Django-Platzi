# Proyecto del curso de Django de Platzi


## Instalación

Crear una carpeta
```Bash
mkdir project
```

### Crear entorno virtual

Instalaremos virtualenv
```Bash
pip install virtualenv
```

Ejecturar para crear nuestros archivos venv. 
```Bash
python -m venv venv
```

### Activar entorno virtual

Si estas en windows:
```Bash
.\venv\Scripts\activate.bat
```

Para Linux\Mac:
```Bash
source venv/bin/activate
```
### Instalar Django

Utilizaremos pip
```Bash
pip install django
```
Entramos a nuestra carpeta app y ejecutamos:

```Bash
django-admin startproject myproject
```

Esto creara un proyecto de django que te creara varios archivos.

project/                  
 |-- myproject/             <-- carpeta del Proyecto django
 |    |-- myproject/
 |    |    |-- __init__.py
 |    |    |-- settings.py
 |    |    |-- urls.py
 |    |    |-- wsgi.py
 |    +-- manage.py
 +-- venv/                  <-- carpeta del entorno virtual
