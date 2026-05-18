# OCI Tagging and Cost Guardrails

Guía práctica para mejorar trazabilidad, control de costos y gobierno operativo en OCI.

## Objetivo

Estandarizar etiquetas y controles para identificar dueños, ambientes, centro de costo y fecha de retiro de recursos.

## Recomendaciones base

1. Define un set mínimo de tags obligatorios:
   - `owner`
   - `environment` (`dev`, `qa`, `prod`)
   - `cost_center`
   - `lifecycle` (`temporary`, `persistent`)
   - `expires_on` (fecha para limpieza programada)
2. Usa defined tags cuando necesites enforcement organizacional.
3. Complementa con freeform tags para experimentación rápida de equipos.
4. Vincula tags a reportes de costos y presupuestos por compartimento.
5. Revisa recursos sin tags en una rutina semanal.

## Flujo recomendado

1. Crea una convención de nombres y tags por equipo.
2. Publica ejemplos en Terraform y OCI CLI para aplicar tags por defecto.
3. Configura budgets y alertas por compartimento/proyecto.
4. Ejecuta revisiones periódicas de recursos huérfanos o vencidos.
5. Aplica limpieza de recursos temporales en cada ciclo de pruebas.

## Checklist rápido

- [ ] Todo recurso nuevo tiene `owner`, `environment` y `cost_center`.
- [ ] Existe presupuesto con alertas para el compartimento.
- [ ] Se registran recursos temporales con `expires_on`.
- [ ] Se ejecuta limpieza de recursos expirados.
