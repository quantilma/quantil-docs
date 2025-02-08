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
Esta sección es dirigida al responsable de crear la arquitectura del proyecto usando alguna plantilla. Se sugiere que sea el **lider del proyecto** que configure correctamente la plantilla y cargue el repositorio a github.
### Paso 1: 
## Entrar a un proyecto
Si ya existe un repositorio (que se creó usando alguna plantilla) y entra un nuevo integrante, estos son los pasos a seguir:

### Paso 1: 

## GIT
