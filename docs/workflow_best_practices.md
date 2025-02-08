# Flujo de trabajo y mejores prácticas
<!-- En el futuro flujo de trabajo se explica como se trabaja en equipo, pull requests, cuantas personas deben ser reviewers, conventional commits, lo que ocurre en CI/CD, etc -->
### Descargar uv
Dado que las plantillas usan `uv` para CI/CD, recetas con `make` y para replicación de ambientes con el archivo `uv.lock`, se recomienda fuertemente su uso. 
=== "Linux/MacOS"
	``` console
	curl -LsSf https://astral.sh/uv/install.sh | sh	
	```
=== "Windows"
	```console
	powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
	```
Revisar que la instalación se haya completado con:
```
uv --version
```
## Crear un nuevo proyecto
Esta sección es dirigida al responsable de crear la arquitectura del proyecto usando alguna plantilla. Se sugiere que sea el **líder del proyecto** que configure correctamente la plantilla y cargue el repositorio a github.

**TODO**

### Paso 1: 
## Entrar a un proyecto
Si ya existe un repositorio (que se creó usando alguna plantilla) y entra un nuevo integrante, estos son los pasos a seguir:

### Paso 1: Configurar usuario de Git  
Si es la primera vez que usa Git, debe configurar su usuario y correo:  

```
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
``` 

### Paso 2: Clonar el repositorio
Una vez configurado el usuario, debe clonar el repositorio. Esto descargará el proyecto en su computador. La URL del repositorio se puede encontrar en GitHub, en la página principal del proyecto, haciendo clic en el botón `Code` y copiando el enlace HTTPS.
```
git clone <url>
``` 

### Paso 3: Configurar la rama para trabajar
Después de clonar el repositorio, debe entrar a su carpeta y cambiar a la rama `dev`, o a la rama indicada por el líder del proyecto:
```
cd <nombre-del-repositorio>
git checkout dev
```

### Paso 4: Subir cambios
Una vez que se quieran subir cambios al repositorio, se debe primero verificar el estado. Esto mostrará todos los cambios que se han realizado:
```
git status
```
Luego, se deben agregar todos los archivos modificados:
```
git add .
```
Una vez agregados los cambios se realiza un commit, en donde se pide un mensaje que resume los cambios que se subirán al repositorio.
```
git commit -m "Descripción corta de los cambios realizados"
```
Por último se deben subir los cambios a la rama `dev`:

```
git push origin dev
```

!!! note "Practica comandos de Git"

    Para mejorar tu manejo de Git, te recomendamos este [juego interactivo](https://learngitbranching.js.org/) que te ayudará a practicar comandos de Git de forma visual y dinámica.