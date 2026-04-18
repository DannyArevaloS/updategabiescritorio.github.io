# updategabiescritorio.github.io

Este repositorio sirve `update.json` con GitHub Pages para que la app consulte metadata de actualización.

## URL de metadata (GitHub Pages)

Al ser un repositorio tipo `<usuario>.github.io`, el archivo queda publicado en:

`https://dannyarevalos.github.io/update.json`

En tu app JavaFX (`config.properties`):

`app.update.metadata-url=https://dannyarevalos.github.io/update.json`

## Binario (GitHub Releases)

Dentro de `update.json`, `downloadUrl` debe apuntar al instalador publicado en Releases, por ejemplo:

`https://github.com/dannyarevalos/javafx-app/releases/download/v1.0.3/GABI-Setup-1.0.3.exe`

## Proceso recomendado por release

1. Publicar el instalador (`.exe`/`.msi`) como asset de un GitHub Release.
2. Actualizar `update.json` con:
   - `version`
   - `downloadUrl`
   - `releaseNotes`
   - (Opcional recomendado, cuando la app lo valide) `checksumSha256` del instalador publicado.  
     El ejemplo mínimo actual de `update.json` no lo incluye.
3. Confirmar que `https://dannyarevalos.github.io/update.json` refleja el contenido actualizado.
