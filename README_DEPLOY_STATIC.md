# CM Banquetería · carpeta pública lista para GitHub Pages

Esta carpeta contiene solo la web pública estática.

Backend/panel interno configurado:

```js
window.CM_API_BASE = 'https://cmbanqueteria.onrender.com';
window.CM_ADMIN_URL = 'https://cmbanqueteria.onrender.com/admin.html';
```

Para subir a GitHub Pages, sube el contenido de esta carpeta a la raíz del repositorio público.
No subas la carpeta completa como `public-static/`; sube sus archivos directamente.

El archivo `CNAME` ya contiene:

```txt
cmbanqueteria.cl
```

## Actualización 2026-08-03

- `config.js` apunta a `https://admin.cmbanqueteria.cl` para usar Render solo como backend/panel interno.
- Correo público actualizado a `claudiamendezbanqueteria@gmail.com`.
- La sección ubicación usa la imagen vertical `assets/terraza.jpeg` y un mapa horizontal inferior.
- CM Experience permanece oculto.

## Actualización 2026-08-04 · navegación móvil y visual vertical

- Navegación móvil convertida a botón Menú con despliegue accesible (`aria-expanded`, cierre por clic en enlace, clic fuera o Escape).
- Acceso interno queda visible junto al logo en móvil.
- Hero y montajes usan mejor las imágenes verticales disponibles (`assets/banqueteria.jpeg`, `assets/terraza.jpeg`).
- Secciones ajustadas para ocupar una pantalla promedio en escritorio y evitar superposiciones en móvil.
- Horario público unificado: lunes a viernes, 12:00 a 15:00 hrs.
