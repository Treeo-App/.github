# Guía de contribución

## Ramas
main es producción: protegida, solo recibe PRs desde develop. develop es la rama de integración: todos los PRs van aquí. Las ramas de trabajo salen de develop con prefijos feat/, fix/, chore/, docs/ o refactor/ (ejemplo: feat/pinned-collections).

## Flujo
Crea tu rama desde develop, haz commits pequeños, abre un PR hacia develop y espera a que pasen los checks. Cuando develop esté estable, se abre un PR de develop hacia main para liberar a producción.

## Commits
Usamos Conventional Commits: feat:, fix:, docs:, chore:, refactor:, test:.

## Antes de abrir el PR
Verifica localmente que pasen los chequeos del proyecto (typecheck, tests y build, según el repositorio).

## Seguridad
Nunca subas credenciales, claves de cuenta de servicio ni archivos .env. Lee SECURITY.md.
