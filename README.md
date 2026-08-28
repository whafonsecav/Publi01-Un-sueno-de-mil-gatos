# Un sueño de mil gatos · La gatica

Presentación HTML en formato **16:9** para el ejercicio de análisis de personaje de
**«Un sueño de mil gatos»**, el segmento animado del episodio 11 de *The Sandman*
(Netflix, 2022). Personaje analizado: **la gatica atigrada** (*The Tabby Kitten*,
voz de Rosie Day).

**Politécnico Grancolombiano** — Institución Universitaria
**Asignatura:** Publicidad 2 · Tercer semestre
**Modalidad:** Presencial · Viernes nocturno
**Docente:** Rudiger Stuart González Preciado

**Autor:** William Fonseca

---

## Ver la presentación

> **https://whafonsecav.github.io/Publi01-Un-sueno-de-mil-gatos/**

O abrir `index.html` en cualquier navegador moderno. No necesita servidor ni conexión:
GSAP va incluido en `assets/js/` y lo único que se descarga de fuera son las tipografías
(si no cargan, el navegador usa las de respaldo y todo sigue funcionando).

### Controles

| Acción | Tecla / gesto |
| --- | --- |
| Lámina siguiente | `→` · `Espacio` · `PageDown` · rueda abajo · swipe izquierda |
| Lámina anterior | `←` · `PageUp` · rueda arriba · swipe derecha |
| Primera / última | `Inicio` / `Fin` |
| Pantalla completa | `F` o el botón ⛶ de la barra |
| Imprimir o exportar a PDF | `P` |

La barra de control ocupa una franja propia debajo de la lámina, así que nunca tapa el
pie. En pantalla completa el puntero se oculta tras un segundo sin moverse.

### En celular y tablet

La lámina es 16:9, así que en vertical quedaría en una franja diminuta: en esa posición
aparece un aviso para girar el dispositivo, con un botón de pantalla completa que además
intenta fijar la orientación horizontal (Android lo permite; iOS no, ahí toca girar a mano).
En pantallas pequeñas se apagan la deriva del fondo, el grano y los desenfoques de la barra:
son los efectos caros de componer y sin ellos el cambio de lámina va suave. El sistema
operativo también manda — si está activado "reducir movimiento", se apagan igual.

Para exportar a PDF: `P` → *Guardar como PDF* → horizontal, márgenes *Ninguno* y
activar *Gráficos de fondo*.

### Música

La música arranca sola **en cuanto se toca la página** por primera vez (los navegadores
no permiten sonido antes de un gesto del usuario) y entra al **15 %**. El control de
volumen está en la barra inferior: la huella silencia y reactiva, y el deslizador ajusta
el nivel.

---

## Las siete láminas

| # | Lámina | Contenido |
| --- | --- | --- |
| 01 | Portada | Título, datos de la asignatura y autor |
| 02 | La trama | Intro, nudo y desenlace + el tono del relato, contado desde la gatica |
| 03 | Personajes | Ficha del personaje, actitudes, intereses e intenciones |
| 04 | Escenario | Los seis lugares del recorrido, lo que representa cada uno, y las tres etapas de la noche |
| 05 | Emociones y sentimientos | Unas y otros en el orden en que le aparecen esa noche |
| 06 | El conflicto | Los hallazgos flotando, la idea a la que apuntan todos, y el conflicto con su tipo |
| 07 | Cierre | Gracias |

> El punto de «Motivaciones, conflicto y situación» ocupa **dos** láminas (05 y 06). En una
> sola no cabía el análisis momento a momento con un cuerpo de letra legible desde el fondo
> del salón. Si el ejercicio exige seis láminas exactas, se fusionan reduciendo la lluvia de
> ideas a los hallazgos sin su lectura.

---

## Dirección de arte

Hisko Hulsing pintó los fondos del segmento en **óleo real sobre lienzo** y encima
rotoscopió a los gatos animados en 3D. De ahí la idea de toda la pieza: la presentación
no se dibuja sobre una diapositiva, se dibuja **dentro del lienzo pintado**. El fondo
entregado (`assets/img/Fondo.png`) es ese lienzo, y el contenido son láminas de papel
puestas encima, como las planchas de un cuaderno de campo.

La paleta se muestreó directamente del archivo de fondo — del `#2f271f` de los árboles
al `#f2ece1` de la luna — y el único acento es el ámbar de los ojos de la gatica,
desaturado para que no rompa el conjunto.

### Archivos gráficos

| Archivo | Qué es |
| --- | --- |
| `assets/img/Fondo.png` | El lienzo pintado. Fondo global de toda la presentación |
| `assets/img/Intro.png` · `Nudo.png` · `Desenlace.png` | Las tres gaticas originales, tal como se entregaron |
| `assets/img/gatica-camina.png` · `gatica-sentada.png` · `gatica-acostada.png` | Las mismas, recortadas al contenido y reescaladas — son las que usa la lámina 02 |
| `assets/img/Huella.png` | Huella dibujada siguiendo la geometría de las que ya están pintadas en el fondo |
| `assets/img/Rasguno.png` | Zarpazo, en el mismo lenguaje pictórico |

> Si se reemplaza alguna de las tres imágenes de la gatica, hay que **volver a generar
> su versión recortada**: la presentación usa `gatica-*.png`, no los originales.

### Método de análisis

La lámina 06 no narra el capítulo, lo analiza. Cada hallazgo es una **conclusión**, no lo que
pasó: la frase dice qué significó ese momento y la nota debajo cuenta de dónde sale. Van
apareciendo de a uno cada ~3 segundos y se quedan flotando alrededor, dejando libre el
centro; ahí aterriza la idea a la que apuntan todos, y de ella sale el conflicto.
**Un clic en la lámina salta al final**, por si hay que ir de afán.

**El tono no es «esperanzador».** La esperanza mira al resultado, y a la gatica le dicen en
la cara que mil gatos nunca harán nada al mismo tiempo — y se duerme igual de tranquila a
soñarlo. Lo que hace no depende de que se cumpla. El tono es **convicción tranquila**: cree
sin ruido y empieza a hacerlo esa misma noche.

**Intereses e intenciones no son lo mismo** y la lámina 03 los separa: el interés se queda
en las ganas (salir, oír la historia, descansar); la intención es un plan que ella ejecuta
esa noche (escaparse, volver a tiempo, soñar).

Un dato que cambió la lectura: **el ronroneo no es señal fiable de bienestar**. Las fuentes
veterinarias coinciden en que el gato también ronronea por autoconsuelo cuando está
estresado, dolorido o en una situación que no controla. Por eso el momento en que la gatica
se encoge y luego ronronea no se lee como "está a gusto" sino como "se calma sola".

Sobre los diálogos: no se pudo acceder a ninguna transcripción completa del episodio, así
que las frases del gato adulto se parafrasean y no van entre comillas. La única cita
verificada es su remate escéptico sobre convencer a mil gatos de hacer algo a la vez, que
viene igual del cómic #18.

### Animación

`assets/js/gsap.min.js` (GSAP 3.12.5, incluido en el repositorio). Cada elemento lleva
su propio retardo en la variable CSS `--d`, así que el ritmo de entrada se compone en el
marcado y no queda enterrado en el JavaScript. **Si GSAP no cargara**, un respaldo en CSS
puro se encarga de las mismas entradas.

El fondo no se queda quieto: deriva y respira de forma continua en un ciclo de 44 s, y
además responde con un paralaje suave al movimiento del ratón.

---

## Nota de rigor

El episodio **no declara país, ciudad ni año**, y el cómic #18 tampoco: no hay topónimo
en pantalla, los dueños no dicen nada que ubique la casa, y la producción nunca anunció
una ambientación — Londres figura solo como sede de rodaje y de los estudios, que no es
lo mismo. Por eso la presentación **no nombra ningún lugar geográfico**: hacerlo sería
presentar como dato de la obra lo que es una inferencia del espectador.
