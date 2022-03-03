## Test Vocacional UniCaribe App

### Tecnologias Usadas:

#### Frontend

- Bootstrap

#### Backend

- Django
- RestFramework
- Sqlite3


## Instalar aplicación


### Configuración del entorno virtual
Se configura el entorno virtual para aislar la aplicación, el uso de la herramienta `virtualenv` nos ayuda a manejar las versiones de las dependencias de forma eficiente:

```sh
$ python3.8 -m venv .env
$ source .env/bin/activate
$ pip install -r requirements.txt
```

Es importante configurar las variables de entorno para realizar una conexión segura con la base de datos.

Para finalizar e iniciar la instancia del servidor de Django debemos migrar las configuraciones de los modelos para la base de datos y correr nuestra aplicación:

```sh
$ python manage.py migrate
$ DEVELOPMENT=1 python manage.py runserver
```

## Organización de archivos en backend:
En "TestVocacional" encontraremos todas las configuraciones importantes en nuestro archivo "settings" para hacer correr la aplicación y configurar las variables correctas para las conexiones a la base de datos.

## Sobre el proyecto

### Problema :

Muchos estudiantes de preparatoria desconocen la vocacion que les apasiona y se sienten indesisos a la hora de escoger una universidad, esta deriva que en el algun momento pudieran abandonar la carrera porque se dieron cuenta que no era lo suyo, de esta manera el estudiante podría perder años escolares en una carrera que no le apasiona.
### Solución :
Nuestra solución es brindarle al estudiante de preparatoria una plataforma que les proporciona un test vocacional y de acuerdo a las respuestas de los usuarios, recomendarle una carrera del plan académico de la universidad.

### Autor
- Joan Méndez Pool - FullStack