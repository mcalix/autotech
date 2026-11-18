# Autotech Retrofitting Gasteiz

Web estática lista para alojar: index.html y assets/. No requiere Node, Java ni compilación.

Cambios: teléfono 945 234 709; WhatsApp eliminado; electrónica sin ECU; galería con cámara de marcha atrás; Instagram @autotechretrofitting. Falta confirmar el correo: buscar CORREO_PENDIENTE en index.html y sustituir el span por <a class="social" href="mailto:CORREO_CONFIRMADO">CORREO_CONFIRMADO</a>, usando la dirección real en ambos lugares.

## Publicación desde IntelliJ y GitHub Pages

1. Descomprimir el ZIP. La raíz debe contener index.html, assets/, .github/workflows/publicar-web.yml y .gitignore. En Finder, Cmd+Shift+. permite ver .github.
2. Si ya hay repositorio: abrirlo en IntelliJ, actualizar con Git > Pull y copiar estos archivos a su raíz, conservando .git. Revisar las diferencias antes de sustituir archivos. No subir el ZIP como único archivo. Si ya hay otro workflow de publicación, revisar cuál conservar para evitar dos despliegues distintos.
3. Si no hay repositorio: abrir la carpeta con File > Open. Activar Git con VCS > Enable Version Control Integration > Git (o Git > Create Git Repository, según versión).
4. Usar main como rama de publicación. En un repositorio nuevo se puede crear/renombrar desde el selector de ramas. No renombrar una rama compartida existente sin coordinarlo: si publica otra rama, ajustar branches en el YAML.
5. Abrir Commit, seleccionar index.html, assets/, .github/workflows/publicar-web.yml, .gitignore y este documento. Mensaje: Actualiza contactos, galería y publicación automática. Hacer Commit.
6. Para un repositorio nuevo: Git > GitHub > Share Project on GitHub, iniciar sesión si se solicita y crear un repositorio público para usar Pages con GitHub Free. No marcar Private. Si ya existe remoto, usar Git > Push. Revisar el destino y subir a origin/main.
7. En GitHub: repositorio > Settings > Pages > Build and deployment > Source > GitHub Actions.
8. En Actions, abrir Publicar web en GitHub Pages. Si la primera ejecución ocurrió antes de habilitar Pages y falló, usar Re-run all jobs o Run workflow en main. Esperar a que termine correctamente. El enlace está en el despliegue y en Settings > Pages.
9. En adelante: editar en IntelliJ, guardar, revisar Commit y usar Commit and Push (o Commit seguido de Git > Push). Cada push a main publica automáticamente. Un commit solo local no dispara Actions.

Este workflow publica exclusivamente en GitHub Pages. Si ya utilizas otro alojamiento gratuito, su mecanismo de despliegue debe configurarse para ese proveedor.

La dirección será https://TU_USUARIO.github.io/TU_REPOSITORIO/ (datos de ejemplo). No necesita un token personal ni secretos para este workflow. La URL exacta la indica GitHub tras publicar. El workflow se entrega preparado, pero no se ha ejecutado en tu cuenta.

## Fotografía de cámara

Lukas Beck, Berlin Opel Corsa lub 2025-11-28 reversing camera.jpg. CC BY 4.0.
https://commons.wikimedia.org/wiki/File:Berlin_Opel_Corsa_lub_2025-11-28_reversing_camera.jpg
https://creativecommons.org/licenses/by/4.0/
Archivo original conservado; encuadre visual adaptado con CSS. Imágenes de referencia, no trabajos reales del taller.
