# Instrucciones de entrega

## Opción rápida

1. Descomprimir `plantilla-estudiantes-completada.zip`.
2. Subir la carpeta a GitHub usando **Add file → Upload files** o **Use this template**.
3. Confirmar que aparece la carpeta `.github/workflows/`.
4. Abrir **Actions** y comprobar la ejecución verde de `CI de calidad`.
5. Crear un tablero gratuito en GitHub Projects o Trello con las columnas y límites descritos en `docs/politicas_kanban.md`.
6. Añadir el enlace real del tablero en el documento y, si el docente lo exige, reemplazar `evidencias/01_tablero_kanban.png` por la captura oficial.

## Evidencia técnica

Ejecutar localmente:

```bash
pip install -r requirements.txt
pytest --cov=src --cov-report=term-missing --cov-fail-under=80
```

Resultado esperado: **4 passed** y cobertura total igual o superior al 80 %.
