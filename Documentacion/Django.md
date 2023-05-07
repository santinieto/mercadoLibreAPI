### Que es Django? ###
Django es un framework de desarrollo web de alto nivel escrito en Python que sigue el patrón de arquitectura de software Modelo-Vista-Controlador (MVC) y Modelo-Vista-Template (MVT).

### Para que sirve? ###
Django fue creado para facilitar la creación de aplicaciones web complejas y escalables, al mismo tiempo que se enfoca en la eficiencia del desarrollo y en la seguridad de la aplicación.

Django proporciona una amplia variedad de características y herramientas que permiten a los desarrolladores crear aplicaciones web de manera más rápida y eficiente, incluyendo:

- Un sistema de enrutamiento que permite dirigir solicitudes HTTP a la vista correspondiente.
- Un ORM (Object-Relational Mapping) que permite interactuar con la base de datos de manera orientada a objetos.
- Una interfaz de administración que permite crear, leer, actualizar y eliminar datos de la base de datos.
- Un sistema de plantillas que permite crear y renderizar vistas HTML dinámicamente.
- Un sistema de autenticación y autorización que permite gestionar el acceso de los usuarios a las diferentes funcionalidades de la aplicación.
- Un conjunto de herramientas de seguridad que permiten proteger la aplicación contra diferentes tipos de ataques, como inyecciones SQL, cross-site scripting (XSS), entre otros.

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

6. Agregar la App a la lista de Apps instaladas

> Abrir el archivo urls.py del proyecto\
> INSTALLED_APPS = [\
>     "django.contrib.admin",\
>     "django.contrib.auth",\
>     "django.contrib.contenttypes",\
>     "django.contrib.sessions",\
>     "django.contrib.messages",\
>     "django.contrib.staticfiles",\
>     "nombre_aplicacion",\
> ]

### Archivos importantes ###
- <nombre_proyecto>/manage.py ---> Archivo basico del proyecto
- <nombre_proyecto>/<nombre_proyecto>/__init__.py ---> Le decimos a Python que interprete este directorio como un paquete
- <nombre_proyecto>/<nombre_proyecto>/settings.py ---> Contiene las configuraciones del proyecto de Django
- <nombre_proyecto>/<nombre_proyecto>/urls.py ---> Es donde se almacenan las URLs del proyecto (se puede tratar como un indice)
- <nombre_proyecto>/<nombre_proyecto>/wsgi.py ---> Relativo al servidor web del proyecto

### Notas importantes
- El archivo <nombre_proyecto>/<nombre_proyecto>/settings.py contiene todas las aplicaciones instaladas del proyecto en la lista "INSTALLED_APPS"
- Cuando creamos una App tenemos que agregarla a la lista de Apps instaladas "INSTALLED_APPS" que esta en settings.py
- Cada App tiene su archivo Python de vistas que se llama views.py y se encuentra en la carpeta de la App