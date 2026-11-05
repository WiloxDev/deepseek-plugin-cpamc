<p align="center">
  <img src="assets/logo.png" alt="DeepSeek Plugin for CPAMC" width="220" />
</p>

# 🐋 DeepSeek Plugin for CLI PROXY API CONSOLE (CPAMC)

[![Ecosistema](https://img.shields.io/badge/Ecosistema-CPAMC%20%7C%20Gentle--Shell%20%7C%20Auto--Switcher--Pro-purple?style=flat-square)](#)
[![Release](https://img.shields.io/badge/Release-v1.0.0-blue?style=flat-square)](https://github.com/WiloxDev/deepseek-plugin-cpamc/releases)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-green?style=flat-square)](LICENSE)

Plugin de **DeepSeek** para **CLI PROXY API CONSOLE (CPAMC)** y el ecosistema **Gentle-Shell**, con soporte nativo para pools de trabajo continuo en **CPAMC Auto Switcher Pro**.

---

## 🌟 Modelos Soportados

- `deepseek-chat` (DeepSeek V3)
- `deepseek-reasoner` (DeepSeek R1 con capacidad de razonamiento profundo / Chain-of-Thought)

---

## 🔄 Integración Dual: Standalone & Pools con Auto Switcher Pro

- **Modo Nativo Directo**: Conexión limpia y ligera en CLI PROXY API CONSOLE (CPAMC) y Gentle-Shell para una cuenta individual.
- **Modo Pool de Trabajo Continuo**: Compatible al 100% con **CPAMC Auto Switcher Pro** para crear grupos de cuentas con rotación automática, conmutación por error (failover ante 429/401) y operación ininterrumpida 24/7.
- 💡 **Multi-Cuenta**: También si tienes dos o más cuentas complementa con el plugin Auto Switcher Pro, así podrás tener una Rotación Continua, distribuir el consumo y evitar agotamiento de cuotas.

---

## 🛠️ Compilación e Instalación

Para compilar e instalar directamente en el directorio de plugins de CPAMC:

```bash
make install
```

O compilar manualmente la biblioteca compartida C-ABI (`.so`):

```bash
make build
```

El binario resultante se ubicará en `~/services/cliproxy/plugins/deepseek-plugin-linux-amd64.so`.
