# 🐍 Ciencia de Datos con Python

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![pandas](https://img.shields.io/badge/pandas-3.0-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Estado](https://img.shields.io/badge/estado-semana%201-2ea44f)](#-estado-del-proyecto)

Repositorio de trabajo del curso **Ciencia de Datos con Python**. La primera semana se centra en preparar un ambiente de desarrollo reproducible y en comprender el valor de los datos para la toma de decisiones.

---

## 📋 Descripción

Este proyecto reúne los notebooks, scripts y documentación necesarios para desarrollar el curso de ciencia de datos con Python. Todo el trabajo se ejecuta dentro de un entorno virtual, de modo que cualquier persona pueda clonar el repositorio y reproducir los resultados con las mismas versiones de librerías.

## 🎯 Objetivos

- Preparar un ambiente de trabajo reproducible con Python y Jupyter.
- Comprender el ciclo de vida del dato: captura, almacenamiento, procesamiento y análisis.
- Aplicar buenas prácticas de organización, documentación y protección de datos.
- Dar el primer paso hacia el análisis de datos con `pandas` y `numpy`.

## 🗂️ Estructura del repositorio

```
ciencia-datos-python/
├── data/
│   ├── raw/                  # Datos originales (no se modifican)
│   └── processed/            # Datos limpios y transformados
├── docs/                     # Documentación del curso
├── notebooks/                # Notebooks de análisis y ejercicios
│   └── semana_01_contexto_ambiente.ipynb
├── outputs/                  # Reportes y archivos exportados
├── scripts/                  # Código reutilizable
│   └── verificar_ambiente.py
├── .gitignore
├── requirements.txt          # Dependencias con versiones fijas
└── README.md
```

> Las carpetas `data/` y `outputs/` se mantienen en el repositorio mediante archivos `.gitkeep`, pero su contenido se ignora para no publicar datos ni resultados generados.

## ✅ Requisitos

- [Python 3.12](https://www.python.org/downloads/) o superior
- [Git](https://git-scm.com/)
- Windows, macOS o Linux

## 🚀 Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/TU-USUARIO/ciencia-datos-python.git
cd ciencia-datos-python
```

### 2. Crear y activar el entorno virtual

**Windows (PowerShell):**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Instalar las dependencias

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Registrar el kernel de Jupyter

```bash
python -m ipykernel install --user --name ciencia-datos --display-name "Python (ciencia-datos)"
```

### 5. Verificar el ambiente

```bash
python scripts/verificar_ambiente.py
```

Salida esperada:

```
Ambiente listo para iniciar Ciencia de Datos con Python
Python: 3.12.x
Pandas: 3.0.x
NumPy: 2.5.x
Verificada: .../data/raw
...
```

## ▶️ Uso

Iniciar Jupyter Lab desde la raíz del proyecto:

```bash
jupyter lab
```

Luego abrir el notebook [`notebooks/semana_01_contexto_ambiente.ipynb`](notebooks/semana_01_contexto_ambiente.ipynb) y seleccionar el kernel **Python (ciencia-datos)**.

También puedes ejecutar el notebook sin abrir la interfaz:

```bash
jupyter nbconvert --to notebook --execute notebooks/semana_01_contexto_ambiente.ipynb --output-dir outputs
```

## 📦 Dependencias principales

| Librería | Versión | Uso |
| --- | --- | --- |
| [pandas](https://pandas.pydata.org/) | 3.0.6 | Manipulación y análisis de datos |
| [numpy](https://numpy.org/) | 2.5.3 | Cálculo numérico |
| [matplotlib](https://matplotlib.org/) | 3.11.2 | Visualización de datos |
| [seaborn](https://seaborn.pydata.org/) | 0.13.2 | Visualización estadística |
| [openpyxl](https://openpyxl.readthedocs.io/) | 3.1.5 | Lectura y escritura de Excel |
| [Faker](https://faker.readthedocs.io/) | 40.40.0 | Generación de datos de prueba |
| [JupyterLab](https://jupyter.org/) | 4.6.4 | Entorno de notebooks |

El listado completo y fijado está en [`requirements.txt`](requirements.txt).

## 🧪 Contenido de la semana 1

| Archivo | Descripción |
| --- | --- |
| [`notebooks/semana_01_contexto_ambiente.ipynb`](notebooks/semana_01_contexto_ambiente.ipynb) | Verificación del entorno y primeras operaciones con `pandas` y `numpy`. |
| [`scripts/verificar_ambiente.py`](scripts/verificar_ambiente.py) | Comprueba las librerías instaladas y crea la estructura de carpetas del proyecto. |

## 🧭 Buenas prácticas del proyecto

1. **No modificar los datos originales**: todo cambio se hace sobre `data/processed/`.
2. **Documentar cada decisión** relevante en el notebook o en `docs/`.
3. **Proteger los datos personales**: no publicar información sensible.
4. **Usar rutas relativas** para que el proyecto funcione en cualquier equipo.
5. **Mantener el notebook ordenado y comentado**, ejecutando las celdas en orden.
6. **Fijar versiones** en `requirements.txt` para garantizar la reproducibilidad.

## 📌 Estado del proyecto

- [x] Ambiente virtual y dependencias
- [x] Verificación automática del entorno
- [x] Notebook de contexto y primeras operaciones
- [ ] Semanas siguientes del curso

## 🤝 Contribuciones

Las sugerencias y correcciones son bienvenidas. Si encuentras un error, abre un *issue* describiendo el problema y los pasos para reproducirlo.

## 📄 Licencia

Material con fines educativos. Puedes reutilizarlo y adaptarlo citando la fuente.
