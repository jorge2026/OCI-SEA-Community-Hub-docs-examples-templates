# Getting Started

Guia rapida para empezar a contribuir o ejecutar ejemplos del repositorio de forma segura y reproducible.

## Objetivo

Al finalizar esta guia deberias poder:

- Entender la estructura del repositorio.
- Preparar tu entorno local para OCI.
- Ejecutar un ejemplo de forma controlada.
- Limpiar recursos para evitar costos innecesarios.

## Prerequisitos

| Requisito | Estado |
| --- | --- |
| Cuenta y tenancy de OCI | Obligatorio |
| Permisos IAM minimos para pruebas | Obligatorio |
| OCI CLI instalado | Recomendado |
| Terraform instalado | Recomendado |

## Recomendaciones de seguridad

- Habilita MFA en tus cuentas de acceso.
- Aplica principio de minimo privilegio en IAM.
- No subas secretos al repositorio.
- Usa variables de entorno y, cuando aplique, OCI Vault.

## Flujo recomendado (15 minutos)

1. Revisa la vista general en [README.md](../README.md).
2. Lee buenas practicas en [docs/best-practices/README.md](best-practices/README.md).
3. Elige una ruta inicial:
   - Terraform: [examples/terraform/README.md](../examples/terraform/README.md)
   - OCI CLI: [examples/cli/README.md](../examples/cli/README.md)
4. Ejecuta los pasos del ejemplo.
5. Ejecuta cleanup o destroy al terminar.

## Checklist rapido

- [ ] Tengo credenciales de OCI fuera del repositorio.
- [ ] Entiendo el costo potencial del ejemplo.
- [ ] Voy a ejecutar cleanup despues de validar.
- [ ] No voy a exponer datos sensibles en PRs o issues.

## Proximos pasos

- Usa una plantilla base en [templates/README.md](../templates/README.md).
- Si vas a contribuir, sigue [CONTRIBUTING.md](../CONTRIBUTING.md).
- Si detectas un problema de seguridad, revisa [SECURITY.md](../SECURITY.md).
