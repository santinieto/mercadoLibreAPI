### Que es Django? ###

### Para que sirve? ###

### Como inicializar un proyecto ###
1. Instalar Anaconda para utilizar Python

Referencia: https://www.anaconda.com/

2. Instalar Django: Si aún no tienes Django instalado, necesitas instalarlo en tu sistema. Puedes instalarlo utilizando pip en la línea de comandos de Anaconda. Por ejemplo, en Linux o macOS, abre una terminal y escribe el siguiente comando:

> pip install django

3. Crear un proyecto: Una vez que tengas Django instalado, puedes crear un nuevo proyecto utilizando el comando django-admin. Abre una terminal o ventana de comandos y escribe lo siguiente:

> django-admin startproject nombre_proyecto

Esto creará una carpeta llamada "nombre_proyecto" con los archivos y la estructura inicial de un proyecto de Django.

4. Crear una aplicación: Django trabaja con el concepto de "aplicaciones", que son módulos de Python que contienen modelos, vistas y templates para un conjunto específico de funcionalidades. Puedes crear una nueva aplicación utilizando el comando:

> cd nombre_proyecto
> python manage.py startapp nombre_aplicacion

5. Esto creará una carpeta llamada "nombre_aplicacion" dentro del proyecto con los archivos necesarios para una aplicación.

### Archivos importantes ###
- <nombre_proyecto>/manage.py ---> Archivo basico del proyecto
- <nombre_proyecto>/<nombre_proyecto>/__init__.py ---> Le decimos a Python que interprete este directorio como un paquete
- <nombre_proyecto>/<nombre_proyecto>/settings.py ---> Contiene las configuraciones del proyecto de Django
- <nombre_proyecto>/<nombre_proyecto>/urls.py ---> Es donde se almacenan las URLs del proyecto (se puede tratar como un indice)
- <nombre_proyecto>/<nombre_proyecto>/wsgi.py ---> Relativo al servidor web del proyecto

### Notas importantes
- El archivo <nombre_proyecto>/<nombre_proyecto>/settings.py contiene todas las aplicaciones instaladas del proyecto en la lista "INSTALLED_APPS"