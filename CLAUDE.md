# Orbit Armory

Fork independiente de Destiny Item Manager (DIM), licencia MIT. Plan completo:
https://claude.ai/artifact/25rMeAfU5yeQ8M81Sx4W1f

## Reglas
- Orbit Armory es una app propia: nunca usar el nombre, logo ni marca de DIM ni de Bungie
  como marca propia. Mantener el aviso de copyright MIT de DIM.
- Codigo nuevo en carpetas propias (por ejemplo src/app/orbit-armory/) y detras de feature
  flags (config/feature-flags.ts). Tocar lo minimo los archivos de DIM para que la fusion
  semanal con upstream (remoto "upstream") tenga pocos conflictos.
- Textos de interfaz nuevos con i18next, en espanol y catalan ademas de ingles.
- Interfaz: mobile-first (PWA en iPhone), WCAG 2.2 AA, tokens de diseno en formato W3C.
  Usar las skills de diseno y revisar con web-design-guidelines y ux-heuristics.
- Privacidad: guardar el minimo de datos, nada de cookies de seguimiento ni publicidad,
  tokens de Bungie siempre cifrados. Sin donaciones, anuncios ni patrocinios.
- Datos de terceros (Clarity, Destiny Data Compendium, wishlists) siempre citados.
- La API de Bungie no permite desmantelar objetos: no intentarlo.

## Comandos
- pnpm start: servidor de desarrollo en https://localhost:8080
- pnpm test / pnpm lint / pnpm typecheck / pnpm fix
- En Windows, pnpm test usa sintaxis de Bash: ejecutarlo desde Git Bash.

## Primera tarea
Modo "mas cercano" del Loadout Optimizer: stats objetivo con pesos, orden por distancia
ponderada y restriccion de origen. Ver la seccion "Linea 3" del plan.
