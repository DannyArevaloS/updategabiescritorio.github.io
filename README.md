# updategabiescritorio.github.io

Este repositorio sirve `update.json` con GitHub Pages para que la app consulte metadata de actualización.

## URL de metadata (GitHub Pages)

Al ser un repositorio tipo `<usuario>.github.io`, el archivo queda publicado en:

`https://dannyarevalos.github.io/update.json`

En tu app JavaFX (`config.properties`):

`app.update.metadata-url=https://dannyarevalos.github.io/update.json`

## Binario (GitHub Releases)

Dentro de `update.json`, `downloadUrl` debe apuntar al instalador publicado en Releases, por ejemplo:

`https://github.com/tuusuario/javafx-app/releases/download/v1.0.3/GABI-Setup-1.0.3.exe`
