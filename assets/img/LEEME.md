# Ranuras de imagen

Basta con **dejar el archivo en esta carpeta con el nombre exacto** y la presentación
lo toma sola. No hay que tocar el HTML.

Mientras un archivo no exista, en su lugar se ve la **escena pintada en SVG** que ya
trae la presentación como respaldo. En cuanto aparezca la imagen, la tapa.

| Archivo | Dónde sale | Proporción | Tamaño sugerido | Qué debería mostrar |
| --- | --- | --- | --- | --- |
| `02-01-intro.png` | Lámina 02 · Intro | **2:1** horizontal | 1200 × 600 px | El Gatito en la casa de sus dueños, luz cálida de interior, antes de salir |
| `02-02-nudo.png` | Lámina 02 · Nudo | **2:1** horizontal | 1200 × 600 px | El cementerio de noche: el Gatito escuchando a la Profeta entre otros gatos |
| `02-03-desenlace.png` | Lámina 02 · Desenlace | **2:1** horizontal | 1200 × 600 px | El Gatito dormido al amanecer, soñando |
| `01-gatito.png` | Lámina 01 · Portada | vertical | 800 × 950 px | El Gatito de cuerpo entero, **fondo transparente (PNG)** |

## Notas

- **Formato:** `.png` (o `.jpg` si se renombra la extensión en las tres primeras; la
  portada conviene que sea PNG con transparencia).
- Las tres imágenes de la lámina 02 se recortan con `object-fit: cover`, así que lo
  importante debe quedar **centrado**: la parte inferior la cubre un degradado oscuro
  donde va el título del acto.
- La imagen de portada se funde con el fondo mediante una máscara redonda, por eso
  funciona mejor con **fondo transparente** o muy oscuro.
- Si una imagen se ve mal recortada, avísame y ajusto el `object-position` de esa celda.

## Estilo recomendado para generarlas

Para que peguen con el episodio y con el diseño de la presentación:

> Pintura al óleo sobre lienzo, pincelada visible, estilo del corto animado
> *A Dream of a Thousand Cats* de Hisko Hulsing. Gato atigrado de pelo corto,
> ojos grandes verde-amarillos con pupila vertical. Iluminación nocturna con
> contraste fuerte. **Interior:** ámbar y ocre cálidos. **Cementerio:** azules
> profundos, índigo y violeta, luna. **Amanecer:** rosa pálido y oro suave.
> Nada de rasgos faciales humanizados: gato realista.
