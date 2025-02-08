# Plantillas de proyectos
Las plantillas de Quantil están diseñadas con base en nuestra experiencia y los estándares modernos de la industria. Sus características principales son:

   - `uv` para manejo de dependencias y de ambientes virtuales
   - CI/CD con [Github Actions](link)
   - Calidad de código con `ruff` y `mypy`.
   - Testing y coverage con `pytest` y `coverage`.
   - Documentación con `mkdocs`
   - Compatibilidad de testeo para múltiples versiones de python con `tox-uv`
   - Recetas para ejecutar con `make`
   
Utilizamos la herramienta [**CookieCutter**](link) para inicializar las plantillas de forma óptima.

## Proyecto de ciencia de datos
Dado que en este tipo de proyectos trabajamos con datos, modelos, entre otras cosas, nos basamos parcialmente en las plantillas [Cookie Cutter Data Science](link) y [CookieCutter uv](link). 

```
uvx cookiecutter https://github.com/quantilma/template-ds
```
??? info "Comando uvx"
	`uvx` viene con la instalación de `uv`. Para instalar `uv`:
	=== "Linux/MacOS"
		``` console
		curl -LsSf https://astral.sh/uv/install.sh | sh	
		```
	=== "Windows"
		```console
		powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
		```
	Para mayor información de cómo instalar `uv`, seguir la [guía oficial de instalación de uv](https://docs.astral.sh/uv/getting-started/installation/).
	
	En caso de no usar `uv`, se puede reemplazar por `pip`:
	```
	pip install cookiecutter
	cookiecutter https://github.com/quantilma/template-ds
	```
	
El anterior comando genera la siguiente estructura de directorio:

```{ .yaml .no-copy }
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         {{ cookiecutter.module_name }} and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
│
└── {{ cookiecutter.module_name }}   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes {{ cookiecutter.module_name }} a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

**TODO: Trabajo futuro, construir documentación para cada plantilla**

## Proyecto de desarrollo de librería

```
uvx cookiecutter https://github.com/quantilma/template-lib
```
??? info "Comando uvx"
	`uvx` viene con la instalación de `uv`. Para instalar `uv`:
	=== "Linux/MacOS"
		``` console
		curl -LsSf https://astral.sh/uv/install.sh | sh	
		```
	=== "Windows"
		```console
		powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
		```
	Para mayor información de cómo instalar `uv`, seguir la [guía oficial de instalación de uv](https://docs.astral.sh/uv/getting-started/installation/).
	
	En caso de no usar `uv`, se puede reemplazar por `pip`:
	```
	pip install cookiecutter
	cookiecutter https://github.com/quantilma/template-ds
	```

**TODO: Trabajo futuro, construir documentación para cada plantilla**
## Otros proyectos
