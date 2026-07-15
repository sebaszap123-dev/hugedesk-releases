# HugeDesk — Releases

Casa pública de **HugeDesk**: descargas, auto-update e issues.
El código fuente vive en un repositorio privado; aquí se construyen y publican
los binarios oficiales y los metadatos de actualización que consume la app.

## Descargas

Última versión: [Releases](https://github.com/sebaszap123-dev/hugedesk-releases/releases/latest)

| Plataforma | Archivo |
| --- | --- |
| macOS (Apple Silicon) | `.dmg` — firmado y notarizado por Apple |
| Fedora / RHEL | `.rpm` |
| Linux (genérico) | `.AppImage` |
| Windows | `.exe` (instalador NSIS) |

La app se auto-actualiza desde este repo (`latest-mac.yml` y equivalentes).

## Reportar un problema

Bugs y peticiones: [Issues](https://github.com/sebaszap123-dev/hugedesk-releases/issues).
Incluye versión de HugeDesk, sistema operativo y pasos para reproducir.

## Cómo se construyen los binarios

El CI de este repo (`.github/workflows/desktop-release.yml`) compila HugeDesk
para las cuatro plataformas, firma y notariza el build de macOS, y publica el
Release. El código se obtiene del repo privado en el tag correspondiente; el
build y la publicación ocurren aquí, que es donde se distribuye la app.
