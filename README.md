# Contenido de este repositorio

Este repo cuenta con tres proyectos que usarás para tu curso de Git y Github.

Los proyectos son los siguientes:

## Plantilla web para presentación

Una muy colorida plantilla HTML básica para lograr una muy buena presentación y llevar a tu audiencia a todos tus canalaes sociales.

Puedes verla [aquí](/miSitio/).

## API de Python básica

Una API básica con solo tres métodos de prueba. ¡Lo que importa es aprender de Github ahora!

Si quieres probarla en modo local solo necesitas escribir los comandos:

```bash
pip install -r requirements.txt
```

Y luego podrás ejecutar la aplicación usando [uvicorn](https://www.uvicorn.org/).

```bash
uvicorn app:app --reload
```

Puedes verla [aquí](/API_Python/).

## Paquete de PIP

Un paquete muy simple de PIP que servirá para crear un artefacto. ¿Te imaginas publicando tu primer paquete PIP?

Todos los archivos preconstruidos están ya cargados en este repo, sin embargo los únicos dos que necesitas son **setup.py** y el contenido de la carpeta **mi_paquete**, todo lo demás lo puedes borrar.

Modifica **setup.py** con tu propia información.

```python
from setuptools import setup, find_packages

setup(
    name="paquetePlatzi",                           # Nombre del paquete
    version="0.1.0",                                # Versión inicial
    packages=find_packages(),                       # Paquetes a incluir
    description="Un paquete pip simple de saludo",  # Breve descripción
    author="Amin Espinoza",                         # Tu nombre
    author_email="amin@platzi.com",                 # Tu correo electrónico
    url="https://github.com/platzi/git-github",     # URL del proyecto
)
```

Después de eso si es necesario, instala las herramientas adecuadas para empaquetar el proyecto.

```bash
pip install setuptools wheel
```

Empaqueta tu proyecto.

```bash
python setup.py sdist bdist_wheel
```

Aquí es donde están todos los archivos de esta carpeta y donde la clase comenzará.

Puedes verla [aquí](/Paquete/).

Genial con toda en este curso
Lo haremos como debe ser

Git y GitHub! Estos son pilares fundamentales para cualquier desarrollador o científico de datos, ya que permiten un control de versiones eficiente, colaboración en proyectos y despliegue de código en la nube.

Acerca de
Aprende sobre control de versiones y colaboración en proyectos de software. Gestiona repositorios, ramas y conflictos con Git, y utiliza GitHub para alojar proyectos, gestionar issues y realizar pull request. Al finalizar, estarás listo para trabajar en equipo y contribuir a proyectos reales, mejorando tu perfil profesional en desarrollo.

Se realiza la bifurcacion del repo Patzi y se clona con exito en la pc local 


# Para verificar la rama activa y actualizar el repositorio local
$ git branch                # Verifica la rama activa
$ git pull origin main      # Jala los últimos cambios de la rama main en GitHub

# Para subir cambios desde el repositorio local a la nube
$ git add .                 # Prepara los archivos para el commit
$ git commit -m "Descripción del cambio" # Realiza el commit
$ git push origin main      # Sube los cambios a GitHub

Resumen

¿Cómo sincronizar tus repositorios con git pull, git push y git fetch?
La gestión de repositorios es una habilidad esencial en el desarrollo de software moderno. Git y GitHub permiten a los desarrolladores colaborar y sincronizar cambios de manera eficiente. Aquí te explicaremos cómo los comandos git pull, git push y git fetch juegan un papel crucial en este proceso, ayudándote a entender cuándo y cómo utilizarlos para mantener tus repositorios actualizados.


# Descargar cambios sin aplicarlos de inmediato
$ git fetch origin                # Jala los cambios de la rama origen

# Comparar y evaluar diferencias entre ramas
$ git log main..origin/main       # Compara las diferencias entre la rama local y la remota

# Una vez evaluados, fusionar cambios en la rama local
$ git merge origin/main           # Fusiona los cambios evaluados
