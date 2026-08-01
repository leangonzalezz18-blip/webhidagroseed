# HidAgroSeed — sitio web

Sitio institucional de **HidAgroSeed**, productora de semillas hortícolas de San Juan, Argentina.

🌐 **[hidagroseed.netlify.app](https://hidagroseed.netlify.app)** · **hidagroseedar@gmail.com** · WhatsApp **+54 9 2645 614925** · [@hidagroseed\_](https://www.instagram.com/hidagroseed_/)

---

## Qué es

Una página estática de una sola vista, sin dependencias ni proceso de compilación. Todo el CSS y el JavaScript están dentro de `index.html`, así que basta con abrir el archivo o servir la carpeta.

```
index.html    la página completa (HTML + CSS + JS)
img/          fotografías, miniaturas, logotipos y pósters de video
video/        clips de campo y planta
fonts/        tipografías incrustadas
```

**El sitio no carga ningún recurso externo.** Las tipografías están incluidas en `fonts/`, así que se ve exactamente igual siempre, sin depender de Google Fonts ni de que el visitante tenga conexión a servicios de terceros.

## Cómo verla

Abrir `index.html` en cualquier navegador moderno, o servir la carpeta:

```bash
npx serve .
```

## Cómo publicarla

El sitio está publicado en **Netlify**, conectado a este repositorio: cada `push` a la rama `main` se despliega solo en [hidagroseed.netlify.app](https://hidagroseed.netlify.app). No hay compilación — *build command* vacío y directorio de publicación la raíz.

Es un sitio estático, así que también funciona en cualquier otro lado sin cambios: GitHub Pages (*Settings → Pages*, rama `main`, carpeta raíz) o un hosting tradicional por FTP a `public_html`.

Si algún día se cambia el dominio, hay que actualizar la dirección en las etiquetas `canonical`, `og:url` y `og:image` del `<head>` de `index.html`, que están escritas completas para que funcione la vista previa al compartir el enlace.

## Detalles técnicos

- Diseño adaptable, verificado a 390, 768 y 1280 px.
- Navegación con menú desplegable por debajo de 1180 px.
- Todas las fotografías se amplían al hacer clic, con teclado y deslizamiento táctil.
- Respeta `prefers-reduced-motion`; si el JavaScript no carga, el contenido se muestra igual.
- Tipografías Manrope y Fraunces incrustadas (variables, subconjuntos latin y latin-ext), bajo SIL Open Font License 1.1.

| | |
|---|---|
| Verde de marca | `#03AD29` |
| Verde profundo | `#062A15` |
| Fondo claro | `#FBFAF7` |

---

## Derechos

**Todas las fotografías y videos de este repositorio son propiedad de HidAgroSeed** y se publican únicamente como parte de este sitio. No están licenciados para reutilización.

© HidAgroSeed. San Juan, Argentina.
