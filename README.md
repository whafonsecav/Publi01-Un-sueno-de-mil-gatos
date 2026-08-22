# Un sueño de mil gatos · El Gatito

Presentación HTML en formato **16:9** para el ejercicio de análisis de personaje de
**«Un sueño de mil gatos»**, el segmento animado del episodio 11 de *The Sandman*
(Netflix, 2022). Personaje analizado: **El Gatito** (*The Tabby Kitten*).

**Politécnico Grancolombiano** — Institución Universitaria
**Asignatura:** Publicidad 2 · Tercer semestre
**Modalidad:** Presencial · Viernes nocturno
**Docente:** Rudiger Stuart González Preciado

**Integrantes:** Mariana Pinzón · Mariana Silva · William Fonseca

---

## Ver la presentación

> **https://whafonsecav.github.io/Publi02-Un_Sueno_de_Mil_Gatos/**

O abrir `index.html` en cualquier navegador moderno.

### Controles

| Acción | Tecla / gesto |
| --- | --- |
| Lámina siguiente | `→` · `Espacio` · `PageDown` · rueda abajo · swipe izquierda |
| Lámina anterior | `←` · `PageUp` · rueda arriba · swipe derecha |
| Primera / última | `Inicio` / `Fin` |
| Pantalla completa | `F` |
| Imprimir o exportar a PDF | `P` |

La barra de control está siempre visible en una franja propia debajo de la lámina, así
que nunca tapa el pie. En pantalla completa el puntero se oculta tras un segundo sin
moverse y reaparece al primer movimiento.

Para exportar a PDF: `P` → *Guardar como PDF* → horizontal, márgenes *Ninguno* y
activar *Gráficos de fondo*.

---

## Estructura (6 láminas)

| # | Lámina | Contenido |
| --- | --- | --- |
| 01 | **Portada** | Título, personaje, institución, asignatura, modalidad, docente e integrantes |
| 02 | **Trama** | Intro · Nudo · Desenlace, con tres escenas pintadas, y el tono desde el que se cuenta la historia |
| 03 | **Personaje** | Demográficos + Actitudes/Opiniones + Intereses + Intenciones |
| 04 | **Escenario** | Eje de una sola noche (anochecer → amanecer), los 5 escenarios y el resumen de lugares |
| 05 | **Motivación** | Emociones · Sentimientos · Conflicto/Situación |
| 06 | **Gracias** | Cierre |

---

## Dirección de arte

El diseño se derivó de **cómo está hecho el episodio**, no de una plantilla. La
investigación (ver `docs/`) confirmó que el director **Hisko Hulsing** pintó los
fondos en **óleo real sobre lienzo** en Submarine (Ámsterdam) y sobre ellos
**rotoscopió** a mano gatos animados en 3D por Untold Studios (Londres), con una
regla de oro: *«tenían que ser gatos reales: sin comportamiento antropomórfico»*.

De ahí salen las decisiones visuales:

- **Grano de lienzo** sobre toda la lámina, en modo `overlay`, como la trama del textil bajo el óleo.
- **Bordes desplazados** con un filtro SVG (`feTurbulence` + `feDisplacementMap`) para que las formas pintadas no se vean vectoriales.
- **Paleta por secuencia**, igual que el episodio: ámbar y ocre para la casa, azules profundos y violeta para la noche y el cementerio, carmesí y rosa para lo onírico, y oro sobre negro para lo divino.
- **Ojos luminosos verde-amarillos** como punto de luz recurrente, incluidos los pares de ojos que parpadean en la oscuridad de fondo.
- **Motas de sueño** que suben lentamente por cada lámina.

| Color | Hex | Uso |
| --- | --- | --- |
| Negro de lienzo | `#07060d` | Fondo |
| Noche / índigo | `#0e1730` · `#1a2952` | La noche, el camino |
| Violeta | `#3a2b60` | El cementerio |
| Carmesí | `#8f2130` | El viaje onírico |
| Ámbar / ocre | `#c98a37` · `#e2a94e` | La casa, el óleo cálido |
| Oro | `#f2cd72` | Acento principal, lo divino |
| Rosa amanecer | `#dd9484` | El cierre |
| Verde de los ojos | `#c3e05a` | El gatito, la esperanza |

**Tipografías:** Cormorant Unicase (titulares), Spectral (texto), Jost (etiquetas).

---

## Sobre la imagen del personaje

El gatito es una **ilustración vectorial original** hecha para esta presentación,
siguiendo el diseño del episodio: atigrado de pelo corto, ojos grandes verde-amarillos
con pupila vertical, la «M» tabby en la frente y proporciones de cría.

Se dibujó desde cero por dos razones: los fotogramas del episodio son material con
derechos y este repositorio es público, y una ilustración propia **se puede animar**.
El gatito parpadea, mueve la cola y las orejas, y aparece en las seis láminas.

---

## Estructura de archivos

```
index.html         Presentación completa (CSS + JS + ilustraciones e iconos SVG en línea)
assets/logo/       Logo del Politécnico Grancolombiano
assets/music/      Carpeta lista por si se añade música de fondo
docs/              La investigación verificada que sustenta el contenido
```

Sin dependencias externas más allá de Google Fonts: el gatito, las tres escenas
pintadas y todos los iconos son SVG escritos a mano en el propio archivo.
