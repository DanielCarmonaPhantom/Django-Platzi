# Proyecto del curso de Django de Platzi

Contenido:

1. Instalación de paquetes para el proyecto
2. Crear una App
3. Crear el modelo ORM
4. Vistas

## 1. Instalación

Crear una carpeta
```Bash
mkdir project
```

### Crear entorno virtual
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
django-admin startproject myproject .
```

Esto creara un proyecto de django que te creara varios archivos.
```
project/                  
 |-- myproject/             <-- carpeta del Proyecto django
 |    |-- myproject/
 |    |    |-- __init__.py
 |    |    |-- settings.py
 |    |    |-- urls.py
 |    |    |-- wsgi.py
 |    +-- manage.py
 +-- venv/                  <-- carpeta del entorno virtual
```
### Levantar servidor
Entramos a nuestra carpeta `myproject` y utilizaremos el comando: 
```Bash
python manage.py runserver
```

Esto nos dara como resultado la url de nuestro servidor local que se desplego en el puerto 8000.

Para acceder solo escribe en tu navegador <a href='http://127.0.0.1:8000' target='_blank'>http://127.0.0.1:8000</a>

## 2. Crear una App

Como myproject es el proyecto principal, a este se le pueden agregar o crear apps, y para crear una app utilizamos

```Bash
django-admin startapp app1
```

Esto crea una app1 dentro de la carpeta


## 3. Crear un archivo para describir las tablas de bases de datos ORM
```Bash
python manage.py makemigrations polls
````

```Bash
python manage.py migrate
````

## Consola interactiva
```Bash
python manage.py shell
```
