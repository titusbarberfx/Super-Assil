# Super Assil — Hogar y Perfumería

Sitio exportado desde **Google Stitch**. Cursor y Claude Code comparten esta carpeta y el mismo MCP (`stitch`).

## Archivos

| Archivo | Rol |
|---------|-----|
| `code.html` | Página principal (Tailwind CDN, tokens en `tailwind.config`) |
| `DESIGN.md` | Design system: colores, tipografía, espaciado, componentes |

## Objetivo

Mejorar la web manteniendo lujo minimalista mediterráneo-oriental: mucho espacio en blanco, fotografía protagonista, sin sombras, esquinas rectas (radius 0), acento oro `#79591d` / `#B89150` con moderación.

## Reglas al editar

1. Usar tokens de `DESIGN.md` y las clases Tailwind ya definidas (`headline-*`, `body-*`, `label-sm`, colores `primary`, `secondary`, `surface-*`).
2. No añadir `rounded-lg` ni sombras salvo que el design system lo pida explícitamente.
3. Espaciado entre secciones: `section-gap-desktop` / `section-gap-mobile`.
4. Texto en español; tono editorial y premium.
5. Tras cambios grandes, validar responsive y contraste.

## MCP Stitch

Con el servidor `stitch` conectado, puedes listar proyectos/diseños en Stitch y alinear `code.html` con el diseño fuente.
