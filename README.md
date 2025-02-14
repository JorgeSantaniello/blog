Django Blog

Un blog completo desarrollado con Django 5.1.6, que incluye sistema de usuarios, gestión de posts y una interfaz responsive usando Bootstrap 5.
🚀 Características

Sistema de autenticación de usuarios
Operaciones CRUD completas para posts
Interfaz responsive con Bootstrap 5
Panel de administración personalizado
Sistema de permisos basado en usuarios
Paginación de posts
Ordenamiento por fecha

📋 Prerrequisitos

Python 3.11.5 o superior
pip (gestor de paquetes de Python)
Entorno virtual (recomendado)

🔧 Instalación

Clona el repositorio

bashCopygit clone https://github.com/tuusuario/django-blog.git
cd django-blog

Crea y activa el entorno virtual

bashCopy# Windows
python -m venv venv
venv\Scripts\activate

# Linux/macOS
python3 -m venv venv
source venv/bin/activate

Instala las dependencias

bashCopypip install -r requirements.txt

Configura las variables de entorno

bashCopy# Crea un archivo .env en la raíz del proyecto
SECRET_KEY=tu_clave_secreta
DEBUG=True

Realiza las migraciones

bashCopypython manage.py makemigrations
python manage.py migrate

Crea un superusuario

bashCopypython manage.py createsuperuser

Inicia el servidor

bashCopypython manage.py runserver
🗂️ Estructura del Proyecto
Copyblog/
├── manage.py
├── requirements.txt
├── blog/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
└── posts/
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── models.py
    ├── forms.py
    ├── urls.py
    ├── views.py
    └── templates/
        └── posts/
            ├── base.html
            ├── post_list.html
            ├── post_detail.html
            ├── post_form.html
            └── post_confirm_delete.html
💻 Uso

Accede al panel de administración:

URL: http://127.0.0.1:8000/admin/
Usa las credenciales del superusuario creado


Gestión de Posts:

Crear: /post/new/
Listar: /
Detalle: /post/<id>/
Editar: /post/<id>/update/
Eliminar: /post/<id>/delete/


🛠️ Tecnologías Utilizadas

Django - Framework web
Bootstrap - Framework CSS
SQLite - Base de datos
django-widget-tweaks - Personalización de formularios


✨ Autor

Tu Nombre - Trabajo Inicial - tuusuario
