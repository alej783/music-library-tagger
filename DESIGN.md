# Arquitectura

## Canales separados

### Aplicación
Código local que se ejecuta en macOS y se comunica con Música mediante Apple Events/AppleScript.

### Taxonomía
Reglas de clasificación, nombres de géneros, jerarquías y criterios. Se distribuye desde `taxonomy/taxonomy.json` y puede actualizarse sin reinstalar la aplicación.

## Actualizaciones

La aplicación consulta `update_manifest.json`.

Flujo previsto:

1. comprobar versión;
2. descargar archivos declarados;
3. verificar SHA-256;
4. crear backup;
5. sustituir archivos;
6. reiniciar cuando cambie código.

## Privacidad

La biblioteca del usuario permanece local. GitHub se utiliza para distribuir código y taxonomía, no para almacenar automáticamente canciones, playlists ni credenciales.
