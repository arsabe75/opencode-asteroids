---
description: Crea un git worktree en .worktrees/<nombre> derivado del argumento y el contexto.
agent: build
---

Argumento recibido: $ARGUMENTS

Analiza el argumento anterior (puede contener espacios) junto con el contexto de la
conversación y deriva un nombre para el worktree: corto, descriptivo, en minúsculas
y kebab-case (palabras separadas por guiones, sin espacios ni caracteres especiales).
Si el argumento está vacío, deriva el nombre únicamente del contexto.

Luego ejecuta ÚNICAMENTE este comando, reemplazando <nombre> por el nombre derivado:

git worktree add ".worktrees/<nombre>"

Restricciones estrictas:

- No cambies de directorio.
- No ejecutes ningún otro comando.
- No edites ni crees archivos.
- No hagas nada más antes ni después.
- Si los argumentos son muy largos, simplifícalos a un nombre significativo.
