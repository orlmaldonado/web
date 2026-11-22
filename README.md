# Web Personal · José Orlando Maldonado Bautista

Sitio académico estático de docencia, investigación y recursos didácticos.

- **Página pública:** https://orlmaldonado.github.io/web/
- **Repositorio:** https://github.com/orlmaldonado/web
- **Recursos:** https://orlmaldonado.github.io/web/recursos.html
- **Perceptrón:** https://orlmaldonado.github.io/web/animaciones/perceptron_simple.html
- **Publicación:** GitHub Pages, rama `main`, archivos en la raíz.

## Continuar el trabajo

Leer primero [BITACORA.md](BITACORA.md): contiene versiones anteriores, formato, decisiones, comprobaciones y procedimiento de actualización. [AGENTS.md](AGENTS.md) resume las instrucciones para futuras sesiones. El archivo local `ESTADO_PUBLICACION.local.json`, si existe, registra el último commit y despliegue comprobados.

## Archivos activos

`index.html`, `docencia.html`, `investigacion.html`, `recursos.html` y `blog.html` comparten `styles.css`. El retrato está en `assets/`. El simulador está en `animaciones/perceptron_simple.html` y su adaptación visual en `animaciones/perceptron.css`.

La fuente activa está en la raíz. `propuesta-multipagina/` conserva la propuesta histórica y no se publica.

## Revisión y publicación

Abrir `index.html` o `recursos.html` en un navegador. No requiere instalación, compilación ni servidor. Las tipografías provienen de Google Fonts y tienen alternativas locales.

Comprobar navegación, enlaces y controles afectados. Publicar sobre la cabeza vigente de `main`, conservando los archivos remotos ajenos al cambio y `.nojekyll`. Verificar el despliegue en [GitHub Actions](https://github.com/orlmaldonado/web/actions). No publicar respaldos, archivos temporales, credenciales ni el estado local de publicación.
