# Entrega final — Auditoría de calidad de un equipo ágil

**Caso:** startup de una app de citas médicas con entregas quincenales, defectos escapados, pruebas manuales y despliegues los viernes.

## Evidencias incluidas

- `evidencias/01_tablero_kanban.png`: tablero con WIP y políticas.
- `evidencias/02_github_actions_ci.png`: ejecución demostrativa de la puerta de calidad.
- `evidencias/03_metricas_dora.png`: hoja de cálculo demostrativa con fórmulas y resultados.
- `docs/atributos_iso25010.md`: diagnóstico ISO/IEC 25010:2023.
- `docs/DoD.md`: Definition of Done de 6 criterios.
- `docs/politicas_kanban.md`: políticas y límites WIP.
- `tests/test_citas.py`: pruebas unitarias TDD.
- `src/citas.py`: implementación validada.
- `.github/workflows/ci.yml`: workflow de GitHub Actions.
- `docs/metricas.md`: métricas DORA y métricas por enfoque.
- `docs/guion_exposicion.md`: guion para la defensa de 3 minutos.

> Las imágenes incluidas son capturas demostrativas preparadas con los datos y configuración de esta entrega. La ejecución oficial de GitHub Actions se obtiene al subir el contenido a un repositorio y hacer push; el workflow está listo para ejecutarse sin cambios.

## Capturas

### Tablero Kanban

![Tablero Kanban](evidencias/01_tablero_kanban.png)

### Puerta de calidad en CI

![GitHub Actions](evidencias/02_github_actions_ci.png)

### Hoja de métricas DORA

![Métricas DORA](evidencias/03_metricas_dora.png)

## Resultado de validación local

- Pruebas: **4 passed**.
- Cobertura de `src`: **100 %**.
- Umbral configurado en CI: **80 %**.
- Datos DORA procesados: **20 despliegues**.

## Métricas DORA calculadas

| Métrica | Resultado |
|---|---:|
| Frecuencia de despliegue | 0,71 por día; aproximadamente 5 por semana |
| Lead time mediano | 20 horas |
| Tasa de fallo de cambios | 20 % |
| MTTR | 4,5 horas |

## Plan de cumplimiento

1. Todo cambio debe tener criterios de aceptación y una historia priorizada.
2. El desarrollo se limita a 2 tarjetas simultáneas y la revisión/pruebas a 2.
3. Cada cambio debe incluir pruebas automatizadas y pasar el umbral de cobertura.
4. Ningún cambio llega a despliegue sin revisión, DoD y aprobación.
5. Se evita concentrar despliegues en viernes; se usa despliegue controlado y rollback.
6. Las métricas se revisan en cada retrospectiva para mejorar sin usar indicadores aislados para castigar personas.
