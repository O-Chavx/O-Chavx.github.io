# O-Chavx.github.io

Mi portafolio personal: https://o-chavx.github.io

Es un solo `index.html` (estilo Jon Barron): HTML y CSS puros, sin Jekyll ni dependencias.

## Estructura

| Ruta | Qué es |
|---|---|
| `index.html` | Todo el sitio: inicio, proyectos, video y herramientas |
| `images/` | Figuras de cada proyecto (JPG livianos) y `foto.jpg` (la pones tú) |
| `files/cv.pdf` | El CV |
| `.nojekyll` | Le dice a GitHub Pages que publique los archivos tal cual |

## Lo que falta poner

1. `images/foto.jpg`: una foto cuadrada, de unos 400 × 400 px. Mientras no esté, se ven las iniciales.
2. `files/cv.pdf`: el CV. El botón «CV en PDF» se muestra solo cuando el archivo existe.
3. En `index.html`, al final, el bloque `PERFIL`: el link de LinkedIn y el correo. Vacíos no se muestran.

## Publicarlo

1. En GitHub, **New repository** → nombre exacto `O-Chavx.github.io`, **Public**, sin README.
2. En esta carpeta:
   ```bash
   git init -b main
   git add .
   git commit -m "Primer portafolio"
   git remote add origin https://github.com/O-Chavx/O-Chavx.github.io.git
   git push -u origin main
   ```
3. **Settings → Pages → Source: Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. Esperar el check verde en **Actions** (1 a 2 minutos) y abrir https://o-chavx.github.io
5. Pegar el link en el issue #203.

## Agregar un proyecto

Copiar un bloque `<article class="card">…</article>` en `index.html`, cambiar título, pregunta, resultado, imagen y links.
La imagen va en `images/`, exportada en JPG de unos cientos de KB.
