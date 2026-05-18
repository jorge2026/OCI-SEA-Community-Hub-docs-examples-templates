# OCI Tagging and Cost Guardrails

Guia practica para mejorar trazabilidad, control de costos y gobierno operativo en OCI.

## Objetivo

Estandarizar etiquetas y controles para identificar dueños, ambientes, centro de costo y fecha de retiro de recursos.

## Recomendaciones base

1. Define un set minimo de tags obligatorios:
   - `owner`
   - `environment` (`dev`, `qa`, `prod`)
   - `cost_center`
   - `lifecycle` (`temporary`, `persistent`)
   - `expires_on` (fecha para limpieza programada)
2. Usa defined tags cuando necesites enforcement organizacional.
3. Complementa con freeform tags para experimentacion rapida de equipos.
4. Vincula tags a reportes de costos y presupuestos por compartimento.
5. Revisa recursos sin tags en una rutina semanal.

## Flujo recomendado

1. Crea una convencion de nombres y tags por equipo.
2. Publica ejemplos en Terraform y OCI CLI para aplicar tags por defecto.
3. Configura budgets y alertas por compartimento/proyecto.
4. Ejecuta revisiones periodicas de recursos huerfanos o vencidos.
5. Aplica limpieza de recursos temporales en cada ciclo de pruebas.

## Checklist rapido

- [ ] Todo recurso nuevo tiene `owner`, `environment` y `cost_center`.
- [ ] Existe presupuesto con alertas para el compartimento.
- [ ] Se registran recursos temporales con `expires_on`.
- [ ] Se ejecuta limpieza de recursos expirados.
