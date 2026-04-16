# Generador de Facturas - Zoo Picasso

Aplicacion de escritorio para generar facturas en formato `.xlsx` con Flet.

## Funcionalidades actuales

- Login de acceso.
- Creacion de facturas por lineas (concepto, cantidad, precio unitario).
- Guardado de archivo Calc/Excel (`.xlsx`) con selector de ruta.
- Limpieza automatica del formulario tras guardado correcto.
- Acumulado diario de importes en la sesion.
- Contador de facturas del dia en la sesion.
- Ajuste manual del acumulado (resta), por Enter o boton.
- Confirmaciones para evitar cierres/salidas por error.

## Estructura principal

- `main.py`: app de escritorio (Flet).
- `src/`: logica de modelo, contador, writer y settings.

## Requisitos

- Python 3.11+ (el proyecto corre con entornos mas nuevos tambien).
- `uv` para gestionar dependencias.

## Ejecutar

Desde la carpeta del proyecto:

```bash
uv sync
uv run main.py
```

## Tests

La documentacion completa de pruebas esta en `TESTING.md`.

Comando rapido:

```bash
./.venv/bin/python -m pytest tests/ -q
```
