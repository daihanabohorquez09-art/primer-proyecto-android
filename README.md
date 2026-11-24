# Primer Proyecto Android

Proyecto Android Studio en Java con cuatro idiomas y fondo Nine-Patch.

## Requisitos
- Android Studio reciente
- JDK 17
- Android SDK 35

## Abrir
1. Descomprime el ZIP.
2. En Android Studio selecciona **Open** y elige la carpeta `PrimerProyectoAndroid`.
3. Espera a que Gradle termine la sincronización.
4. Ejecuta la aplicación en un emulador o dispositivo.

## Idiomas
Android selecciona automáticamente los textos según el idioma del dispositivo:
- Español: `res/values/strings.xml` (predeterminado)
- Inglés: `res/values-en/strings.xml`
- Francés: `res/values-fr/strings.xml`
- Alemán: `res/values-de/strings.xml`

## Nine-Patch
El fondo está en `res/drawable-nodpi/fondo_android.9.png`.
Los marcadores de estiramiento se ubicaron en zonas de cielo azul sin elementos:
- Borde superior: franja horizontal de estiramiento.
- Borde izquierdo: franja vertical de estiramiento.

Así se prioriza que el marcianito y las nubes inferiores permanezcan en la zona fija de la imagen mientras se amplía el cielo. Android procesa el archivo `.9.png` al compilar los recursos.

La imagen original también se conserva como `fondo_original.png`.

## Adaptación de pantalla
La pantalla usa `ConstraintLayout`, tamaños en `dp`/`sp` y restricciones relativas. La actividad permite orientación vertical y horizontal; Android vuelve a distribuir el contenido al cambiar la orientación.
