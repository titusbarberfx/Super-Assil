# Conectar Cursor y Claude para mejorar Super Assil

Este proyecto ya incluye la configuración compartida. Solo falta **activar** el servidor MCP y la API key.

## 1. API key de Google Stitch

1. Abre [stitch.withgoogle.com](https://stitch.withgoogle.com/) con tu cuenta Google.
2. En el proyecto **Super Assil**, genera o copia la **API key**.
3. Crea un archivo `.env` en la raíz del proyecto (copia de `.env.example`):

   ```env
   STITCH_API_KEY=tu-clave-real
   ```

4. Define la misma variable en Windows para que Cursor/Claude la lean:
   - **Configuración → Sistema → Acerca de → Configuración avanzada del sistema → Variables de entorno**
   - Nueva variable de usuario: `STITCH_API_KEY` = tu clave
   - Reinicia Cursor después de guardar.

## 2. Activar MCP en Cursor

1. Abre este proyecto en Cursor.
2. Ve a **Cursor Settings → MCP** (o `Ctrl+Shift+J` → pestaña MCP).
3. Debería aparecer el servidor **`stitch`** desde `.cursor/mcp.json`.
4. Actívalo y confirma que el estado sea **Connected** (verde).
5. Si pide aprobación del servidor del proyecto, acéptala.

Si no carga el `.env`, pega la key en la configuración del servidor MCP en Cursor (campo de entorno `STITCH_API_KEY`).

## 3. Claude Code (opcional, mismo proyecto)

Instala Claude Code si quieres usar Claude en terminal con los mismos tools:

```powershell
# Con npm instalado (nodejs.org):
npm install -g @anthropic-ai/claude-code
cd "c:\Users\santi\Downloads\stitch_super_assil_hogar_y_perfumer_a"
claude
```

El archivo `.mcp.json` en la raíz es el equivalente para Claude Code. Tras definir `STITCH_API_KEY`, ejecuta `/mcp` dentro de Claude y conecta `stitch`.

## 4. Cómo pedir mejoras

En **Cursor Agent** o **Claude**, con MCP activo:

- *"Revisa el diseño en Stitch y propón mejoras para la sección hero de code.html"*
- *"Alinea la tipografía y espaciado de code.html con DESIGN.md"*
- *"Añade una sección de perfumería siguiendo el design system"*

`CLAUDE.md` y `.cursor/rules/super-assil-design.mdc` dan contexto automático a ambos asistentes.

## Alternativa: Google Cloud (sin API key)

Si prefieres OAuth en lugar de API key:

1. Instala [Google Cloud SDK](https://cloud.google.com/sdk/docs/install).
2. `gcloud auth login` y `gcloud auth application-default login`
3. Habilita: `gcloud beta services mcp enable stitch.googleapis.com`
4. Cambia `.cursor/mcp.json` por el servidor stdio documentado en [stitch-mcp](https://www.npmjs.com/package/stitch-mcp) (requiere Node.js + `npx` en PATH).

## Problemas frecuentes

| Problema | Solución |
|----------|----------|
| MCP `stitch` en rojo | Comprueba `STITCH_API_KEY` y reinicia Cursor |
| `npx` no reconocido | Instala Node.js LTS desde [nodejs.org](https://nodejs.org/) |
| Sin herramientas Stitch | Verifica la key en Stitch y que el proyecto exista en la web |
