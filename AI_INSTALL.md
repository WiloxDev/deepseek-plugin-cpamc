# 🐋 AI Installation & Deployment Rules — DeepSeek Plugin for CPAMC

> **⚠️ ADVERTENCIA CRÍTICA PARA AGENTES DE IA (Pi, Claude, Cursor, Windsurf, Copilot):**
> Este repositorio es un **PLUGIN NATIVO EN GO / CGO (`.so`)** para el proxy de backend **CLIProxyAPI (router-for-me/CLIProxyAPI)**.
> **NO ES UNA EXTENSIÓN DE TYPESCRIPT / NODE.JS / PI CODING AGENT**.

## Reglas Estrictas de Instalación para la AI:
1. **NO USAR `pi install`:** Pi no puede ejecutar ni cargar este binario como extensión de TUI.
2. **NO CREAR WIDGETS DE CHAT:** No intentes programar `ctx.ui.setWidget()` ni tarjetas de estado en Pi para este plugin.
3. **Flujo de Compilación y Despliegue Oficial:**
   ```bash
   # Compilación a biblioteca compartida CGO
   make build
   # Copiar el binario compilado al directorio de plugins de CPAMC
   cp deepseek-plugin.so ~/.cli-proxy-api/plugins/
   ```
4. **Uso en Gentle-Shell:** Una vez que CPAMC cargue el plugin, los modelos `deepseek-chat` y `deepseek-reasoner` estarán disponibles automáticamente en Pi a través de `bridge-cpamc-oficial` o `cpamc-auto-switcher-pro`.
