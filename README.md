# Nebai Ilg · Paisajismo

Sitio web de **Nebai Ilg Paisajismo**: diseño de jardines, jardinería y venta de plantas ornamentales, frutales y nativas en el Valle de Traslasierra, Córdoba.

> Cada jardín tiene una historia. Empecemos con la tuya.

## Qué tiene el sitio

- **Inicio**: presentación y foto de un proyecto terminado.
- **Servicios**: diseño, canteros, jardines para polinizadores, cercos vivos, rocallas, borduras, aromáticas y mantenimiento.
- **Proyectos**: planos de plantación y fotos de trabajos realizados.
- **Tienda**: buscador, 8 categorías y carrito de compras. El pedido se envía por WhatsApp.
- **Sobre mí** y **Contacto**: formulario que abre WhatsApp con el mensaje armado.

Es una página estática (HTML, CSS y JavaScript en un solo archivo). No necesita servidor, base de datos ni instalación.

## Archivos

```
index.html      → todo el sitio
img/            → logo, fotos y planos
README.md       → este archivo
.nojekyll       → le indica a GitHub Pages que publique los archivos tal cual
```

## Publicar en GitHub Pages

1. Entrá a [github.com](https://github.com) e iniciá sesión (o creá una cuenta).
2. Arriba a la derecha tocá **+ → New repository**.
   - **Repository name**: `nebai-ilg` (o el nombre que prefieras).
   - Marcá **Public**.
   - Tocá **Create repository**.
3. En la página del repositorio nuevo, tocá **uploading an existing file**.
4. Arrastrá **todo el contenido** de esta carpeta: `index.html`, `README.md`, `.nojekyll` y la carpeta `img`.
   - `index.html` tiene que quedar en la raíz, al mismo nivel que `img`.
   - Si `.nojekyll` no aparece (Windows oculta los archivos que empiezan con punto), no pasa nada: el sitio funciona igual.
5. Abajo tocá **Commit changes**.
6. Andá a **Settings → Pages**.
   - En **Source** elegí **Deploy from a branch**.
   - En **Branch** elegí `main` y la carpeta `/ (root)`. Tocá **Save**.
7. Esperá uno o dos minutos y recargá esa página: arriba aparece el link del sitio, por ejemplo:
   `https://TU-USUARIO.github.io/nebai-ilg/`

### Usar un dominio propio (opcional)

Si compran un dominio (por ejemplo `nebaiilg.com.ar`), en **Settings → Pages → Custom domain** se escribe el dominio y se configuran los DNS según las [instrucciones de GitHub](https://docs.github.com/es/pages/configuring-a-custom-domain-for-your-github-pages-site).

## Actualizar el sitio

1. En el repositorio, tocá el archivo que querés cambiar (por ejemplo `index.html`).
2. Tocá el lápiz ✏️ (**Edit this file**), hacé el cambio y tocá **Commit changes**.
3. En uno o dos minutos el sitio se actualiza solo.

Para reemplazar un archivo entero: **Add file → Upload files**, subí el archivo nuevo con el mismo nombre y tocá **Commit changes**.

### Cambiar precios o productos de la tienda

Todo está dentro de `index.html`, en la parte de `<script>`. Buscá (Ctrl+F) estos nombres:

| Lista | Qué contiene |
|---|---|
| `FRUTALES` | Frutales con tamaño y precio: `["Almendro Guara","10L",29700,"Frutos secos"]` |
| `SERVICIOS` | Servicios de jardinería |
| `CANTEROS` | Canteros a pedido |
| `NATIVOS` | Árboles nativos |
| `PASTOS` | Pastos |
| `FLORES` | Flores |
| `ARBUSTOS` | Arbustos |
| `CERCOS` | Plantas para cercos |

- Los precios van **sin puntos ni signo $**: `29700`, no `$29.700`.
- En las listas que no son frutales cada ítem es `["Nombre","Descripción"]` y aparece como “A consultar”.
- Cada línea termina en coma, salvo la última de la lista.

### Cambiar teléfono, email o Instagram

Buscá `5493544448781` (WhatsApp, con el formato 549 + característica + número), `nebai.paisajismo@gmail.com` y `nebaiilg.paisajismo`, y reemplazalos donde aparezcan.

### Cambiar fotos

Subí la foto nueva a la carpeta `img` **con el mismo nombre** que la que querés reemplazar. Conviene que pesen menos de 500 KB (podés achicarlas en [squoosh.app](https://squoosh.app)).

## Contacto

- WhatsApp: [3544 448781](https://wa.me/5493544448781)
- Email: nebai.paisajismo@gmail.com
- Instagram: [@nebaiilg.paisajismo](https://instagram.com/nebaiilg.paisajismo)

© Nebai Ilg Paisajismo · Traslasierra, Córdoba
