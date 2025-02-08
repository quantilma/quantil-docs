# Herramientas y estándares

En Quantil, confiamos en un conjunto de herramientas para garantizar consistencia, eficiencia y calidad en todos nuestros proyectos. A continuación, se encuentra una lista de las herramientas que utilizamos, junto con enlaces a su documentación.

## Herramientas

### Python Development ToolKit
- **Version**: Python 3.9+
- **Linting**: `ruff` Se utiliza para resaltar bugs y errores de estilo. Ver estándares para revisar que reglas se aplican.
- **Formatter**: `ruff` Se utiliza para formatear código y que sea más consistente el proyecto. Ver estándares para revisar que reglas se aplican.
- **Testing**: `pytest`, `coverage`
!!! note "Trabajar en el editor de texto"
    Herramientas como `ruff` tienen extensiones para trabajar en su editor de texto favorito. Se recomienda fuertemente sustituir las que vengan por defecto.
### Manejo de dependencias y ambientes virtuales
**UV:** Se sugiere trabajar con una solución moderna de manejo de dependencias como `uv` que también permite crear y manipular ambientes virtuales de una forma sencilla.  No obstante, se deja a preferencia del investigador si usa `conda`, `poetry`, `pixi` entre otros.

!!! warning "Proyectos sin `uv`"

    Si el investigador usa una herramienta distinta a `uv`, como `conda` + `pip`, perderá beneficios de las [plantillas de proyectos](/templates) como el `Makefile`. Esto se debe a que las recetas `make` utilizan `uv` de forma interna.
	
### Control de versiones y plataformas
- **Git**: Utilizamos `git` como nuestro sistema de control de versiones.
- **Commitizen**: Lo utilizamos para crear commits con estructura específica (ver estándares) y generar changelog.
- **Github**: Lo utilizamos para nuestros repositorios y repositorios de clientes.
- **AzureDevops**: Lo utilizamos para repositorios de clientes en algunos casos (e.g., Ecopetrol).

### CI/CD
**TODO: AGREGAR INFO DE GITHUB ACTIONS**, EXPLICAR QUE SE EJECUTA CODE QUALITY EN EL PUSH...

### Otras herramientas relevantes
- **Tox**: Permite probar distintas versiones de python para un proyecto/librería.
- **Make**: Agrupa comandos largos en recetas. Por ejemplo, `make test` ejecuta la suite de pruebas, `make data` hace todo el preprocesamiento de datos y deja el conjunto de datos listo para los modelos.
- **CookieCutter**: Definir
- **TeamWork**: Definir

## Estándares

### PEP621
Todos los proyectos deben llevar un archivo `pyproject.toml` con los metadatos y dependencias del proyecto. Si utiliza un manejador de dependencias moderno, este genera ademas un archivo `.lock` que permite contruir el mismo ambiente sin importar el sistema operativo.

**TODO: Revisar la configuración del archivo pyproject.toml que funcione para todos los OS con librerías como pytorch**

### PEP8
**TODO: COMPLETAR SECCIÓN**

### Conventional commits
**TODO: COMPLETAR SECCIÓN**

<!-- ## Documentation -->
<!-- - **MkDocs**: For generating static sites. -->
<!-- - **Material Theme**: For a modern, responsive design. -->
<!-- - **GitHub Pages**: For hosting documentation. -->

<!-- ## Data Science Tools -->
<!-- - **Cookiecutter Data Science**: For project structure. -->
<!-- - **DVC**: For data versioning. -->
<!-- - **MLflow**: For experiment tracking. -->

<!-- ## Library Tools -->
<!-- - **UV**: For library structure. -->
<!-- - **Semantic Versioning**: For versioning libraries. -->
<!-- - **mkdocstrings**: For auto-generating API docs. -->


<!-- ## sdkljfa -->
