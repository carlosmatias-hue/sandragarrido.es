# Web personal — Sandra Garrido Sotomayor

Página personal de una sola pantalla lista para publicar en GitHub Pages con el dominio `sandragarrido.es`.

## Contenido

- `index.html` — toda la página (HTML + CSS incluido, sin dependencias externas).
- `assets/sandra-photo.png` — foto de perfil.

## Cómo publicarla en GitHub Pages

1. En GitHub, crea un repositorio nuevo (público) — por ejemplo `sandragarrido.es`.
2. Sube estos archivos (`index.html` y la carpeta `assets/`) a la raíz del repositorio (arrastrándolos en "Add file" → "Upload files", igual que hicimos con la otra web).
3. En el repositorio, ve a **Settings → Pages**. En "Build and deployment" elige "Deploy from a branch", rama `main`, carpeta `/root`, y guarda.
4. En la misma pantalla, en **Custom domain**, escribe `sandragarrido.es` y guarda.
5. En dinahosting, dentro de `sandragarrido.es` → **Zonas DNS**, crea 4 registros tipo **A** con host `@`, apuntando a:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153
6. Espera a que se propague el DNS y comprueba que `sandragarrido.es` carga en el navegador.
7. Vuelve a Settings → Pages y activa **Enforce HTTPS**.

## Pendiente de completar

- **Email de contacto**: no se ha incluido un botón de email porque no tenemos una dirección que Sandra quiera hacer pública. En `index.html`, busca los dos comentarios `<!-- Añade aquí... -->` y `<!-- Sustituye este comentario... -->` y sustitúyelos por un botón como:
  ```html
  <a class="btn btn-ghost" href="mailto:SU_EMAIL">Contactar</a>
  ```
- Revisa el "Sobre mí": está copiado literalmente de LinkedIn y está en inglés (así lo escribió ella). Tradúcelo o ajústalo si prefieres que la web esté 100% en español.
