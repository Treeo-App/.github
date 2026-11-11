# Política de seguridad

## Reportar una vulnerabilidad
Si encuentras una vulnerabilidad en cualquier repositorio de Treeo-App, no abras un issue público ni la menciones en un PR. Repórtala de forma privada usando la opción Security > Report a vulnerability del repositorio afectado, o escribe al responsable del proyecto (@erikodes) por mensaje privado.

Intentamos confirmar la recepción en pocos días y mantener informado a quien reporta hasta que se corrija.

## Secretos y datos sensibles
Nunca se hacen commits de credenciales, claves de cuenta de servicio, certificados de firma, tokens ni archivos .env. Si un secreto se expone por error, hay que rotarlo de inmediato y avisar al responsable.

## Flujo de ramas
Todo cambio entra por Pull Request hacia develop. La rama main representa producción y solo recibe PRs desde develop.
