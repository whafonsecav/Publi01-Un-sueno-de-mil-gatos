# Las imágenes de la presentación

## Lo que hay aquí

| Archivo | Dónde sale | Notas |
| --- | --- | --- |
| `Fondo.png` | Fondo global de las seis láminas | El lienzo pintado. De aquí sale toda la paleta |
| `Intro.png` | *(original)* | La gatica caminando |
| `Nudo.png` | *(original)* | La gatica sentada |
| `Desenlace.png` | *(original)* | La gatica acostada |
| `gatica-camina.png` | Lámina 02 · Intro | `Intro.png` recortada al contenido |
| `gatica-sentada.png` | Lámina 02 · Nudo | `Nudo.png` recortada al contenido |
| `gatica-acostada.png` | Lámina 02 · Desenlace | `Desenlace.png` recortada al contenido |
| `Huella.png` | Portada, cierre, rastro de la lámina 04, barra de control | Generada |
| `Rasguno.png` | Portada y cierre | Generada |

**La presentación usa las versiones `gatica-*.png`, no los originales.** Los tres
archivos originales se conservan intactos como respaldo.

---

## Si se reemplaza alguna gatica

Los originales traen mucho espacio transparente alrededor, y las posiciones sobre las
tarjetas dependen de que la imagen esté recortada justo al contenido. Después de
reemplazar cualquiera de los tres, hay que volver a generar su versión recortada:

```bash
python -c "
from PIL import Image
def recortar(src, dst, largo):
    im = Image.open(src).convert('RGBA')
    im = im.crop(im.split()[3].point(lambda v: 255 if v > 10 else 0).getbbox())
    s = largo / float(max(im.size))
    im.resize((round(im.width*s), round(im.height*s)), Image.LANCZOS).save(dst)
recortar('Intro.png',     'gatica-camina.png',   1000)
recortar('Nudo.png',      'gatica-sentada.png',  1000)
recortar('Desenlace.png', 'gatica-acostada.png', 1200)
"
```

Si una gatica queda mal encajada sobre su tarjeta, se ajusta en el CSS de `index.html`,
en las reglas `.cat-walk`, `.cat-sit` y `.cat-lie`: `width` cambia el tamaño y
`margin-bottom` cuánto se hunde en el canto de la lámina.

---

## Si se reemplaza el fondo

`Fondo.png` es horizontal y se recorta con `object-fit: cover` sobre un lienzo de
1600 × 900, así que conviene que sea **16:9** o parecido. Al cambiarlo, revisar que la
paleta de `:root` en `index.html` siga pegando: los tokens `--ink`, `--umber`, `--sepia`,
`--taupe`, `--stone`, `--sand`, `--linen`, `--vellum` y `--moon` se muestrearon de la
imagen actual.

---

## Sobre la huella y el rasguño

Se dibujaron para este trabajo, siguiendo la geometría de las huellas que ya están
pintadas en `Fondo.png` (una almohadilla ancha y trilobulada más cuatro dedos en arco) y
con el mismo tratamiento: relleno sepia plano, borde suave y ligeramente irregular, y un
grano de lienzo apenas perceptible.

En la presentación se usan siempre con opacidad baja, para que se lean como parte de la
pintura y no como una calcomanía encima. La huella hace además de viñeta en la barra de
control y de tirador del deslizador de volumen.
