# GRZ

Un sitio de una sola página con una colección de textos escritos para GRZ.

👉 **Ver el sitio:** https://lucasvicente-com-ar.github.io/grz/

## Qué contiene

- Seis textos (poemas y prosa poética), cada uno con su fecha original de escritura.
- Una ilustración por texto: algunas son imágenes generadas por IA subidas directamente (`img/*.png`); las que todavía no tienen imagen propia usan un arte vectorial (SVG) simbólico de reemplazo, en el mismo estilo oscuro/dorado del sitio.
- Mismo diseño editorial oscuro usado en [el-amenazado](https://github.com/lucasvicente-com-ar/el-amenazado) (tipografía Cormorant Garamond + Cinzel, acentos dorados, animaciones de aparición al hacer scroll). Totalmente responsive.

## Estructura

```
.
├── index.html      # el sitio completo: HTML + CSS + JS inline, sin build ni dependencias
├── img/            # una ilustración por texto (.png subidas o .svg de reemplazo)
├── escritos.txt    # textos en bruto, fuente original
├── REGISTRO-IA.md  # registro de qué IA trabajó en el proyecto y cuándo
└── README.md
```

## Reemplazar una ilustración

En `index.html`, cada poema tiene un bloque como:

```html
<img class="poem-image" src="img/apocalipsis-i.svg" alt="descripción breve">
```

Para usar otra imagen (por ejemplo una foto o un dibujo distinto), subí el archivo a `img/` y actualizá el `src` y el `alt`.

## Publicación

El sitio se sirve con **GitHub Pages** desde la rama `main`, raíz del repositorio (`/`). Cualquier `git push` a `main` se refleja automáticamente en unos minutos en:

https://lucasvicente-com-ar.github.io/grz/
