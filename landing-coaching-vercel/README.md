# Landing de Coaching Ejecutivo

Proyecto Vite listo para Vercel.

## Personalización antes de publicar

En `index.html`, reemplaza:

- `Tu Nombre` por tu nombre.
- `tu-correo@ejemplo.com` por tu correo.
- Los enlaces `href="#"` de agenda y LinkedIn por tus URLs.
- El bloque `portrait-placeholder` por una imagen profesional cuando la tengas.
- La letra `S` y el nombre `Strengths & Leadership` por tu marca.

## Usar una fotografía

1. Guarda la foto como `public/perfil.jpg`.
2. Sustituye este bloque en `index.html`:

```html
<div class="portrait-placeholder" role="img" aria-label="Espacio para fotografía profesional">
  <span>Tu fotografía<br />profesional</span>
</div>
```

por:

```html
<img class="portrait-placeholder" src="/perfil.jpg" alt="Tu nombre, coach ejecutivo" />
```

Y agrega a `.portrait-placeholder` en `src/style.css`:

```css
object-fit: cover;
object-position: center;
```

## Desarrollo local

```bash
npm install
npm run dev
```

## Publicación en Vercel

Importa el repositorio o sube la carpeta. Vercel detectará Vite. El comando de construcción es `npm run build` y el directorio de salida es `dist`.
