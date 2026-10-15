# Pulso — versión PWA

Esta carpeta contiene una primera adaptación de tu HTML para instalarlo como aplicación web (PWA).

## Archivos
- `index.html`: tu app original con metadatos PWA y botón de instalación.
- `manifest.webmanifest`: nombre, colores y configuración de instalación.
- `sw.js`: service worker para caché básica y funcionamiento más resistente cuando vuelve a abrirse.
- `icons/pulso-icon.svg`: icono SVG.

## Publicarla gratis con GitHub Pages
1. Crea o inicia sesión en GitHub.
2. Crea un repositorio nuevo (por ejemplo `pulso-app`).
3. Sube el contenido de esta carpeta al nivel principal del repositorio: `index.html`, `manifest.webmanifest`, `sw.js` y la carpeta `icons`.
4. En el repositorio, abre **Settings → Pages**.
5. En **Build and deployment**, selecciona **Deploy from a branch**, elige la rama `main` y la carpeta `/ (root)`, y guarda.
6. Espera a que GitHub Pages publique la web. La URL suele ser `https://TU-USUARIO.github.io/pulso-app/`.
7. Abre la URL desde el móvil. En Android/Chrome, usa el botón “Instalar app” cuando aparezca. En iPhone/iPad, abre la página en Safari → Compartir → Añadir a pantalla de inicio.

## Importante
- GitHub Pages proporciona HTTPS, necesario para que el service worker funcione.
- Esta versión es una PWA, no un APK ni una app nativa publicada en las tiendas.
- Los datos se guardan localmente en el navegador/dispositivo mediante `localStorage`; no se sincronizan entre dispositivos y borrar los datos del navegador puede borrarlos.
- La app original carga la fuente Plus Jakarta Sans desde Google Fonts, por lo que esa fuente necesita internet salvo que se empaquete localmente.
- Antes de anunciarla públicamente, prueba las funciones principales en Android y iPhone. El botón de instalación depende del navegador y del dispositivo.
