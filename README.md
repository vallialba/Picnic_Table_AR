# Mesa Picnic WebAR con MindAR

Este proyecto permite lanzar una experiencia de realidad aumentada desde un QR, sin instalar ninguna app.

## Idea general

QR → abre una web → se activa la cámara → reconoce una imagen marcador → aparece la mesa en AR.

## Archivos

- `index.html`: página principal WebAR.
- `assets/mesa_cenital.png`: imagen que aparece en realidad aumentada.
- `assets/targets.mind`: archivo que debes generar con MindAR Compiler.
- `assets/AQUI_DEBES_PONER_targets.mind.txt`: recordatorio.

## Paso 1: Crear la imagen marcador

Usa una imagen con detalles, por ejemplo:

- mesa con césped,
- sombras,
- entorno,
- textura,
- contraste.

Cuantos más detalles tenga, mejor se reconocerá.

## Paso 2: Generar `targets.mind`

1. Entra en MindAR Compiler:
   https://hiukim.github.io/mind-ar-js-doc/tools/compile/

2. Sube la imagen marcador.

3. Descarga el archivo generado.

4. Renómbralo como:

   targets.mind

5. Guárdalo en:

   assets/targets.mind

## Paso 3: Subir a GitHub Pages

1. Crea un repositorio llamado, por ejemplo:

   mesaAR

2. Sube estos archivos.

3. Ve a:

   Settings → Pages

4. Selecciona:

   Deploy from branch → main → /root

5. Obtendrás una URL como:

   https://tuusuario.github.io/mesaAR/

## Paso 4: Crear el QR

Genera un QR que apunte a la URL de GitHub Pages.

Ejemplo:

   https://tuusuario.github.io/mesaAR/

Puedes usar Canva, QR Code Monkey o cualquier generador de QR.

## Resultado final

El usuario escanea el QR, se abre la página, permite el acceso a la cámara y apunta a la imagen marcador. Al reconocerla, aparece la mesa en realidad aumentada.

## Nota

Ahora mismo el contenido AR es una imagen 2D sobre un plano. Si más adelante quieres un resultado más realista, sustituye la imagen por un modelo 3D `.glb`.
