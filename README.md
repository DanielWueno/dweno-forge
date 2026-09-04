# dweno-forge

Marketplace personal de plugins de Claude Code. Este repositorio no contiene
código ejecutable propio — es un catálogo (`.claude-plugin/marketplace.json`)
que apunta a los repositorios donde vive cada plugin.

## Plugins disponibles

| Plugin | Qué hace |
|---|---|
| [`credential-read-guard`](https://github.com/DanielWueno/credential-read-guard) | Bloquea de forma determinista la lectura o búsqueda de material de credenciales. |
| [`arnes-plan`](https://github.com/DanielWueno/arnes-plan) | Ejecuta un plan de ingeniería un ítem por sesión, con el avance en un ledger versionado. |
| [`postgres-readonly-mcp`](https://github.com/DanielWueno/postgres-readonly-mcp-plugin) | Acceso MCP de solo lectura a bases PostgreSQL. |

## Instalación

Añadir el marketplace una sola vez:

```
/plugin marketplace add DanielWueno/dweno-forge
```

Instalar los plugins que interesen (cada uno por separado):

```
/plugin install credential-read-guard@dweno-forge
/plugin install arnes-plan@dweno-forge
/plugin install postgres-readonly-mcp@dweno-forge
```

`claude plugin update` recoge nuevas versiones publicadas en cada repositorio
individual — este catálogo no fija versión por plugin, así que sigue siempre
la última etiqueta disponible en el repositorio de origen.

## Requisitos

Claude Code con soporte de marketplaces de plugins (`/plugin marketplace`).

## Licencia

MIT
