# Tabla Periódica e Ingeniería de Materiales

Aplicación de escritorio hecha con Flet para explorar la tabla periódica, consultar datos de elementos y analizar combinaciones simples de materiales.

## Estructura actual

La app Flet generada vive en:

```bash
periodic_table_app/
```

Archivos principales:

- `periodic_table_app/src/main.py`: interfaz principal
- `periodic_table_app/src/algorithm.py`: lógica de configuración electrónica y valencia
- `periodic_table_app/src/elements.json`: datos de elementos químicos
- `periodic_table_app/src/table.json`: distribución visual de la tabla periódica
- `periodic_table_app/src/colors.json`: colores por categoría

## Dependencias

- Python 3.10 o superior
- Flet 0.86.5 o superior
- Flet CLI 0.86.5 o superior
- Flet Desktop 0.86.5 o superior
- Flet Web 0.86.5 o superior

El entorno local del repositorio ya fue creado en `.venv` y Flet quedó instalado ahí.

## Instalación desde cero

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r periodic_table_app/requirements.txt
```

## Verificar instalación

```bash
.venv/bin/flet --version
.venv/bin/python -m pip show flet
```

## Ejecutar la app

```bash
.venv/bin/flet run periodic_table_app
```

También puedes entrar a la app y correrla desde ahí:

```bash
cd periodic_table_app
../.venv/bin/flet run
```

## Pruebas

```bash
.venv/bin/python -m py_compile periodic_table_app/src/main.py periodic_table_app/src/algorithm.py
```
