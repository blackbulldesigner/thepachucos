# Página web de The Pachucos

Página sencilla para el QR: **redes sociales primero**, luego el **menú** y la **ubicación**.

## Qué hay aquí

- `index.html`: la página completa.
- `assets/`:
  - logos: `logo.webp` y `logo.png` arriba, `logo-blanco.png` en el pie;
  - íconos de la pestaña y del celular;
  - `og.jpg`: la imagen que sale al compartir el link por WhatsApp o Facebook;
  - `carnal.woff`: la fuente Carnal;
  - `menu-comida.jpg` y `menu-bebidas.jpg`: los menús impresos para verlos en grande.

## Cómo se ve

1. **Arriba:** el logo, "SÍGUENOS" y tres botones grandes (Instagram, TikTok y Facebook). En el celular se ven completos sin bajar.
2. **Menú:** pestañas *Comida* y *Bebidas*, con las mismas bandas negras y puntitos del menú impreso.
   - En la web, Tacos y Montados van en la misma tabla, con las columnas Orden · Media · Montado.
   - Los Extras quedaron en *Comida*.
3. **Ubicación:** la dirección, el mapa de Google y botones para *Cómo llegar* (Google Maps) y *Waze*.
4. **Pie:** el logo en blanco, las redes y la leyenda de bebidas alcohólicas.

## Cambiar un precio o un producto

1. Abre `index.html` con el Bloc de notas o VS Code.
2. Busca el nombre del producto (Ctrl+F).
3. Cada producto es un renglón como este:

   ```html
   <li class="row"><span class="name">Sirloin</span><span class="price">$158</span>...</li>
   ```

4. Cambia el texto o el precio y guarda.

Si también cambias el menú impreso, reemplaza `assets/menu-comida.jpg` y `assets/menu-bebidas.jpg`.

## Dónde está publicada

- **Link:** https://blackbulldesigner.github.io/thepachucos/
- **Repositorio:** https://github.com/blackbulldesigner/thepachucos (GitHub Pages, rama `main`)
- **QR:** carpeta `QR/`, afuera de esta carpeta. Ese QR apunta al link de arriba, así que no hay que reimprimirlo cuando cambies la página.

## Subir un cambio

Esta carpeta es el repositorio. Después de editar, abre una terminal aquí y corre:

```
git add .
git commit -m "Cambio de precios"
git push
```

GitHub Pages se actualiza solo en uno o dos minutos.
