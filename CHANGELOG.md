# Changelog — luca-prototype

All notable changes to the LUCA prototype. Newest at top.

## [v5.1] — 2026-04-17
### Changed
- Sidebar: collapsed by default (64px), auto-expand on hover (220px)
- Removed duplicate LUCA logo (sidebar no longer has its own logo, only topbar)
- Content stays centered regardless of sidebar state
- Topbar pushed right to accommodate sidebar (84px padding-left, 240px when pinned)

### Added
- Pin toggle at bottom of sidebar: click pin icon to keep sidebar permanently expanded
- localStorage persistence: remembers pinned state across sessions

## [v5.0] — 2026-04-17
### Changed
- Sidebar lateral colapsable para desktop (reemplaza topbar dnav)
- Renombrar "Panel fiscal" a "Comprobantes"
- Bottom nav mantenido para mobile

### Removed
- Todas las referencias a "Compras recibidas" (dashboard, panel fiscal)
- Sección "Comprobantes recibidos" del Panel Fiscal
- Métrica "Compras últ. 12 meses" del dashboard

### Added
- Nueva pantalla "Configuración" (placeholder)
- Separator antes de WhatsApp en sidebar (visual hierarchy)

## [v4.1] — 2026-04-15
### Changed
- Restored comprobante type cards with show/hide UX (select one → others disappear, "Cambiar tipo" to reset)
- Replaced bar chart with invoice liberation table showing 5 oldest invoices that will free margen
- Liberation section collapsed by default with intuitive expand affordance (▾ chevron + "5 facturas" hint)
- Exclusion detail in Recategorización also uses collapsible pattern
- LUCA logo: non-selectable text, click/tap navigates to Inicio on all screens
### Improved
- Light mode: better contrast on secondary text (#475569 vs #334155), warmer amber (#D97706)
- Softer shadows across both themes (lighter, less aggressive)
- Focus states on inputs: emerald glow ring (box-shadow) for better accessibility
- Hover transitions on cards, buttons, nav items, FAB, avatar
- Topbar and bottom nav: backdrop-filter blur for depth
- Form labels: font-weight 500 for better readability
- Button hover states: primary buttons dim slightly, secondary show border change
- Card hover: subtle border brightening

## [v4.0] — 2026-04-15
### Added
- FB-004: Dashboard — dual limit toggle (actual vs IPC), two progress bars (recategorización + exclusión), CCMA card, collapsible chart
- FB-005: Comprobante — margen hero card, dropdown type selector, stronger date warnings
- FB-006: WhatsApp send button in success screen, Agenda de Clientes screen with search and add
- FB-007: Recategorización screen replaces Alerta Exclusión — step-by-step guide, dates, exclusion collapsible
- FB-008: WhatsApp menu tree per Javier spec — Emitir (texto/voz), Consultas (5 opciones), Asesor chatbot
- Feedback History panel — view submitted feedback, mark items as resuelto (localStorage)
### Changed
- Dashboard: categoría card restructured with big letter, descriptive text, no comprobante count
- Dashboard: compras shows últimos 12 meses + 40% Cat K limit
- Chart title: "Evolución del Margen de Facturación Disponible"
- Nav: "Alertas" renamed to "Recat", Agenda added to desktop nav
- Service date warning: RED and prominent per Javier feedback
### Removed
- Comprobante type cards (replaced with dropdown)
- Alerta Exclusión as dedicated screen (content moved to Recategorización)

## [v3.5] — 2026-04-14
### Changed
- Chart shows cumulative margen disponible por fecha

## [v3.4.2] — 2026-04-14
### Fixed
- Chart outside amounts clipping

## [v3.4.1] — 2026-04-14
### Fixed
- Chart amount visibility, overflow clipping

## [v3.4] — 2026-04-14
### Fixed
- FB-003 third disclaimer
### Changed
- Chart amounts rendered inside bars

## [v3.3] — 2026-04-14
### Changed
- UX fixes from feedback session 2026-04-14

## [v3.2] — 2026-04-14
### Fixed
- Contraste dark mode definitivo

## [v3.1] — 2026-04-14
### Fixed
- Clave fiscal onboarding, contraste dark mode completo
### Changed
- Feedback Javier: clave fiscal onboarding, pvta en comprobante

## [v3.0] — 2026-04-14
### Added
- Paleta premium slate+emerald+indigo, comprobantes, WhatsApp

## [v2.0] — 2026-04-13
### Added
- Comprobantes, 3 métricas, WhatsApp

## [v1.0] — 2026-04-13
### Added
- Prototipo Sprint 00 — LUCA UX inicial
