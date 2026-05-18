# Getting Started

Guía rápida para empezar a contribuir o ejecutar ejemplos del repositorio de forma segura y reproducible.

## Objetivo

Al finalizar esta guía deberías poder:

- Entender la estructura del repositorio.
- Preparar tu entorno local para OCI.
- Ejecutar un ejemplo de forma controlada.
- Limpiar recursos para evitar costos innecesarios.

## Prerrequisitos

| Requisito | Estado |
| --- | --- |
| Cuenta y tenancy de OCI | Obligatorio |
| Permisos IAM mínimos para pruebas | Obligatorio |
| OCI CLI instalado | Recomendado |
| Terraform instalado | Recomendado |

## Recomendaciones de seguridad

- Habilita MFA en tus cuentas de acceso.
- Aplica el principio de mínimo privilegio en IAM.
- No subas secretos al repositorio.
- Usa variables de entorno y, cuando aplique, OCI Vault.

## Flujo recomendado (15 minutos)

1. Revisa la vista general en [README.md](../README.md).
2. Lee buenas prácticas en [docs/best-practices/README.md](best-practices/README.md).
3. Elige una ruta inicial:
   - Terraform: [examples/terraform/README.md](../examples/terraform/README.md)
   - OCI CLI: [examples/cli/README.md](../examples/cli/README.md)
4. Ejecuta los pasos del ejemplo.
5. Ejecuta cleanup o destroy al terminar.

## Checklist rápido

- [ ] Tengo credenciales de OCI fuera del repositorio.
- [ ] Entiendo el costo potencial del ejemplo.
- [ ] Voy a ejecutar cleanup después de validar.
- [ ] No voy a exponer datos sensibles en PRs o issues.

## Próximos pasos

- Usa una plantilla base en [templates/README.md](../templates/README.md).
- Si vas a contribuir, sigue [CONTRIBUTING.md](../CONTRIBUTING.md).
- Si detectas un problema de seguridad, revisa [SECURITY.md](../SECURITY.md).
