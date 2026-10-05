# zlt-web-v2

Material de la web ZLT v2 (ver `LEEME.txt`). Se publica en GitHub Pages
(https://conradoremyzlt.github.io/zlt-web-v2/) con `.github/workflows/pages.yml`,
que arma la copia del sitio en cada push a `main` y cada 6 horas.

## Subir una version nueva del HTML
- Home → `Home/html/ZLT-WEB-V2-home.html`; novedades → `novedades/html/ZLT-WEB-V2-novedades.html`.
- **Antes de commitear, vaciar la clave de YouTube**: `clave:'AIza...'` → `clave:''`.
  El repo es publico; la clave vive solo en el secreto `YT_API_KEY` del repo.
  El workflow falla si el HTML publicado trae una clave.
- No hace falta insertar el login ni corregir rutas: lo hace el workflow.
- `Home/PROYECTOS SIN PUBLICAR/` esta en `.gitignore` y no se sube.

## Login
`gate.js` es copia exacta del de `zltdev/presentacion` (mismos usuarios). Si
cambian los usuarios alla, copiar el archivo de nuevo. Es un login del lado del
navegador: frena a quien entra por la URL, no a quien lea el repo, y los PDF de
`brochures/` quedan accesibles por link directo.
