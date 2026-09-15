# Music Library Tagger

Aplicación local para macOS que organiza y enriquece una biblioteca de Apple Music/Música sin subir la colección musical a GitHub.

## Arquitectura

- **Aplicación local**: lee y modifica Música mediante Apple Events/AppleScript.
- **Actualizaciones**: la app consulta `update_manifest.json` en este repositorio.
- **Taxonomía**: vive en `taxonomy/taxonomy.json` y puede sincronizarse sin reinstalar la app.
- **Privacidad**: MP3/FLAC/M4A, playlists, exports de biblioteca, Apple ID y credenciales permanecen locales salvo que el usuario los exporte explícitamente.

## Convenciones actuales

- `Grupo = Sello | Ciudad`
- El **género** describe el sonido/escena musical.
- La **ciudad** describe la ciudad editorial asociada al sello o a la edición concreta, no el origen estilístico del track.

## Versiones

La primera versión bootstrap con autoactualización es `0.4.0`. Las versiones posteriores se distribuyen mediante el manifiesto del repositorio.
