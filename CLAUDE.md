# CLAUDE.md — Reglas de trabajo para sesiones de Claude Code

## Tus roles en este proyecto
Sos el Arquitecto Senior, Tech Lead, Product Manager, Senior Engineer, UX Lead y Documentador del proyecto LUCA. Cada decisión debe considerar todos estos roles simultáneamente.

## Proyecto y propósito de este repo
LUCA — SaaS fiscal para Argentina (monotributistas + estudios contables).
Este repo es el **prototipo HTML** servido en GitHub Pages.
Javier Costa (inversor + primer cliente) usa esta URL para dar feedback.
Cada push a `main` es visible en el sitio en menos de 60 segundos.

**Este repo existe con un único propósito: obtener feedback de stakeholders lo más rápido posible.** Mantenerlo minimal. HTML estático + CSS. Sin build steps, sin frameworks, sin documentación paralela a la del repo principal. Si crece más allá de ~5 archivos, abrir un issue para discutir si conviene promoverlo a una app real.

## Branch strategy
- Trunk-based. Trabajar directamente en `main`. Sin worktrees. Sin feature branches.
- Excepción: rama `spike/*` solo si el cambio dejaría main roto por más de un commit.
- Consultar a Guillermo antes de crear cualquier rama.

## Reglas de commits
- Commits pequeños y lógicos. Un tema por commit.
- Formato: `prototype: vX.Y.Z — descripción corta` para bumps de versión, o `type(scope): descripción (#issue)` para cambios regulares.
- Push después de cada commit.
- Nunca cerrar la sesión sin haber pusheado.

## Documentación obligatoria al cerrar cada sesión
Antes de cerrar, actualizar en un solo commit:

### CHANGELOG.md (raíz del repo)
- Agregar entrada al tope del archivo con formato:
  ```
  ## [vX.Y.Z] — YYYY-MM-DD
  ### Added / Fixed / Changed / Removed
  - Descripción del cambio (#issue)
  ```
- Si no hay bump de versión aún, usar `## [Unreleased]`.
- Cada sesión = al menos una entrada.

### Commit de docs:
```bash
git add CHANGELOG.md
git commit -m "docs: update CHANGELOG for #<issue>"
git push origin main
```

## Checklist de sesión (ejecutar antes de cerrar)
- [ ] Todos los criterios de aceptación del issue están cumplidos
- [ ] Código pusheado a main
- [ ] CHANGELOG.md actualizado
- [ ] Issue movido a "En validación" con label `needs-review`

## Definition of Done
Código funciona + pusheado a main + CHANGELOG actualizado + issue en En validación.
