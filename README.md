# HidAgroSeed — sitio web

Sitio institucional de **HidAgroSeed**, productora de semillas hortícolas de San Juan, Argentina.

🌐 **hidagroseedar@gmail.com** · WhatsApp **+54 9 2645 614925** · [@hidagroseed\_](https://www.instagram.com/hidagroseed_/)

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

Es un sitio estático: no necesita base de datos ni servidor de aplicaciones.

- **GitHub Pages** — en *Settings → Pages*, elegir la rama `main` y la carpeta raíz.
- **Netlify** — arrastrar la carpeta a [app.netlify.com/drop](https://app.netlify.com/drop).
- **Hosting tradicional** — subir el contenido por FTP a `public_html`.

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
