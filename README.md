# SENSUS GRAECUS

> *La máxima espontaneidad solo es posible cuando se obedece, con gozo y lucidez, la ley que ya vive dentro de las cosas mismas.*
> — Werner Jaeger, *Paideia*

Un diccionario filosófico de griego clásico, 31 entradas que trazan los fundamentos del pensamiento occidental: desde los presocráticos hasta el helenismo, desde *logos* hasta *kenoma*, desde la verdad como desvelamiento (*aletheia*) hasta el vacío constitutivo (*kenoma*). Cada término no se define: se explora en su genealogía conceptual, sus derivados modernos, sus resonancias filosóficas y sus cognados en cinco lenguas vivas.

Un solo archivo HTML. Sin servidor. Sin dependencias. Doble clic y funciona.

**[Ver en vivo](https://nigelmoonwriter.github.io/sensus_graecus/)**

---

## La posición

SENSUS GRAECUS nace de una pregunta: ¿qué palabras fundaron la manera en que el pensamiento occidental concibe el mundo?

Los griegos no alcanzaron su célebre libertad por haber cultivado la subjetividad moderna, sino porque su constitución espiritual les permitió descubrir, en el mismo acto de mirarse a sí mismos, las leyes objetivas que gobiernan las cosas. Esa libertad sin esfuerzo, "sofrenada sin esfuerzo" dice Jaeger, nace precisamente de la conciencia clara de que toda realidad lleva en su interior una norma inmanente.

Este diccionario documenta esa norma inmanente a través del lenguaje. No como inventario léxico, sino como cartografía del pensamiento. *Logos* no es solo "palabra", es el principio racional que ordena el cosmos. *Physis* no es solo "naturaleza", es el proceso por el cual las cosas devienen lo que son. *Aletheia* no es solo "verdad", es el des-velamiento, el acto de arrancar lo real del olvido.

Cada entrada es un nodo en una red conceptual donde filosofía, filología y poética se tocan sin disolverse. Los términos se conectan a través de la etimología protoindoeuropea, los derivados en lenguas modernas y las resonancias filosóficas que cada palabra transporta a través de los siglos.

---

## Contenido

### Inventario de entradas

| # | Lema | Nivel | Ámbito filosófico |
|---|---|---|---|
| 1 | technema (τέχνημα) | intermedio | Creación, artificio, técnica |
| 2 | logos (λόγος) | básico | Razón, palabra, principio |
| 3 | physis (φύσις) | intermedio | Naturaleza, devenir |
| 4 | arche (ἀρχή) | básico | Principio, origen |
| 5 | aletheia (ἀλήθεια) | intermedio | Verdad como desvelamiento |
| 6 | aether (αἰθήρ) | avanzado | Éter, quintaesencia |
| 7 | kosmos (κόσμος) | básico | Orden, universo |
| 8 | nous (νοῦς) | intermedio | Intelecto, mente |
| 9 | eudaimonia (εὐδαιμονία) | intermedio | Florecimiento humano |
| 10 | arete (ἀρετή) | básico | Excelencia, virtud |
| 11 | paideia (παιδεία) | intermedio | Formación integral |
| 12 | agon (ἀγών) | básico | Competencia, lucha |
| 13 | mimesis (μίμησις) | intermedio | Imitación, representación |
| 14 | catharsis (κάθαρσις) | intermedio | Purificación emocional |
| 15 | moira (μοῖρα) | avanzado | Destino, porción |
| 16 | eros (ἔρως) | básico | Deseo, amor |
| 17 | demos (δῆμος) | básico | Pueblo |
| 18 | polis (πόλις) | básico | Ciudad, comunidad política |
| 19 | demokratia (δημοκρατία) | intermedio | Gobierno del pueblo |
| 20 | agora (ἀγορά) | básico | Plaza pública, mercado |
| 21 | theos (θεός) | básico | Dios, divinidad |
| 22 | hubris (ὕβρις) | intermedio | Desmesura, orgullo |
| 23 | nomos (νόμος) | avanzado | Ley, convención |
| 24 | pragma (πρᾶγμα) | básico | Acción, hecho |
| 25 | aisthesis (αἴσθησις) | avanzado | Percepción, sensación |
| 26 | kairos (καιρός) | intermedio | Momento oportuno |
| 27 | phronesis (φρόνησις) | avanzado | Prudencia, sabiduría práctica |
| 28 | sophia (σοφία) | básico | Sabiduría |
| 29 | dynamis (δύναμις) | intermedio | Potencia, poder |
| 30 | kenoma (κενωμα) | avanzado | Vacío, carencia |
| 31 | soma (σῶμα) | básico | Cuerpo |

### Distribución por nivel

| Nivel | Entradas | Ejemplos |
|---|---|---|
| Básico | 12 (39%) | logos, kosmos, eros, demos, polis, theos, sophia, soma |
| Intermedio | 10 (32%) | technema, physis, aletheia, mimesis, catharsis, kairos |
| Avanzado | 9 (29%) | aether, moira, nomos, aisthesis, phronesis, kenoma |

### Áreas temáticas

| Tema | Etiqueta | Entradas |
|---|---|---|
| I | Filosofía fundamental | 15 |
| VII | Epistemología | 10 |
| III | Política y sociedad | 9 |
| IV | Ciencia y naturaleza | 7 |
| V | Mitología y teología | 8 |
| VI | Ethos y pathos | 8 |
| II | Retórica y poesis | 5 |
| VIII | Estética | 5 |
| IX | Vida cotidiana | 4 |

---

## Arquitectura técnica

SENSUS GRAECUS es un archivo HTML autónomo de 1170 líneas que contiene:

```
sensus-graecus.html
├── <style>         — CSS embebido (85 líneas, estética Bauhaus)
│   ├── Paleta: crema, negro, rojo (misma familia que LATINUS)
│   ├── Tipografía: Georgia (serif) / system-ui (sans) / Consolas (mono)
│   └── Modos de lectura (body.mode-basico / .mode-intermedio / .mode-avanzado)
├── <body>          — Estructura HTML
│   ├── Hero + búsqueda
│   ├── Barra de temas (10 botones: I–X)
│   ├── Área de contenido (renderizado dinámico)
│   └── Footer
└── <script>        — JavaScript embebido (IIFE, ~1040 líneas)
    ├── THEMES[]    — Definición de 10 categorías
    ├── ENTRIES[]   — 31 entradas
    └── Lógica      — Búsqueda difusa, filtrado por tema, modos de lectura
```

### Funcionalidades

- **Búsqueda difusa** con debounce de 150ms. Busca en: lema, definiciones, raíz PIE, derivados, cognados, citas.
- **Filtrado por tema** — 10 categorías filosóficas.
- **Modos de lectura** — Tres niveles progresivos (Aficionado / Estudiante / Profesor).
- **Entrada destacada** — *technema* funciona como proto-entrada con schema expandido.
- **Prevención de XSS** — Sanitización mediante nodos de texto del DOM.
- **Responsive** — Media query a 600px con tipografía fluida.

---

## Esquema de datos

SENSUS GRAECUS maneja dos esquemas de datos:

### Schema expandido (entrada prototipo: *technema*)

```json
{
  "id": "technema",
  "lemma": "τέχνημα",
  "lang": "greek",
  "pos": "sustantivo, neutro",
  "themes": ["I", "II", "VIII"],
  "level": "intermedio",
  "featured": true,
  "ipa": "/tékʰ.nɛː.ma/",
  "defs": [
    { "text": "Lo producido por la técnica...", "audience": "basico" },
    { "text": "Producto material o intelectual de un proceso creativo...", "audience": "intermedio" },
    { "text": "En la filosofía griega, el technema es el objeto resultante...", "audience": "avanzado" }
  ],
  "etym": {
    "pie": "*tekʰ-",
    "gloss": "fabricar, construir",
    "path": ["PIE *tekʰ- → gr. τέχνη (téchne) → τέχνημα (téchnēma)"],
    "notes": "Raíz que da techne, técnica, tecnología, arquitectura en lenguas modernas"
  },
  "evo": [
    { "s": "gr.", "from": "kʰ", "to": "t", "rule": "desaspiración", "exp": "tékʰnēma → léxico" }
  ],
  "deriv": [
    { "w": "técnica", "l": "es", "u": "conjunto de procedimientos" },
    { "w": "technology", "l": "en", "u": "application of knowledge" },
    { "w": "technique", "l": "fr", "u": "méthode de fabrication" },
    { "w": "tecnologia", "l": "it", "u": "scienza delle tecniche" },
    { "w": "Technik", "l": "de", "u": "Verfahren zur Herstellung" },
    { "w": "tekhnología", "l": "el", "u": "τέχνη + λόγος" },
    { "w": "tecnología", "l": "pt", "u": "ciência aplicada" },
    { "w": "技術 (gijutsu)", "l": "ja", "u": "技術的手段" }
  ],
  "cogn": [
    { "w": "textile", "l": "en", "m": "fabricado por tejido" },
    { "w": "tejido", "l": "es", "m": "entramado de hilos" },
    { "w": "tissue", "l": "en", "m": "tejido biológico" },
    { "w": "tessuto", "l": "it", "m": "tessuto di stoffa" },
    { "w": "Tuch", "l": "de", "m": "tela, paño" }
  ],
  "example": {
    "quote": "El technema no es la técnica: es lo que la técnica deja cuando ya nadie recuerda quién la inventó.",
    "gloss": "Reflexión sobre la persistencia del artificio",
    "author": "Rei García",
    "work": "Notas para SENSUS GRAECUS",
    "year": "2026",
    "lang": "es"
  },
  "cmp": { "griego": "τέχνημα", "es": "artefacto", "it": "manufatto", "fr": "artefact", "en": "artifact", "de": "Artefakt" },
  "researchNotes": "La noción de technema en Aristóteles se opone a physis...",
  "relatedEntries": ["mimesis", "poiesis"],
  "famousPhrases": [
    { "phrase": "ὁ δὲ ἀνὴρ ἀργὸς οὔτε γῆν οὔτε θάλατταν ἔσθιεν", "translat": "El hombre ocioso no comería ni tierra ni mar", "gloss": "Sobre la necesidad de la técnica", "author": "Epicuro", "note": "Acerca de la vida feliz" }
  ],
  "negativeTheologyTags": ["apofatismo", "silencio", "innombrable"],
  "sources": [
    { "type": "lexicon", "title": "LSJ - Liddell, Scott, Jones", "url": "https://logeion.uchicago.edu/", "confidence": "alta", "used_for": "definiciones" }
  ],
  "flags": { "reviewed": true, "aria_ready": false, "bw_ready": false, "semansis_version": "1.0" }
}
```

### Schema simplificado (entradas 2–31)

Las 30 entradas restantes usan un schema más compacto:

| Campo | Tipo | Diferencia con el expandido |
|---|---|---|
| `id`, `lemma`, `lang`, `pos` | string | Idéntico |
| `themes`, `level` | array / string | Idéntico |
| `ipa` | string | Idéntico |
| `defs` | `string[]` | Strings simples, no objetos `{text, audience}` |
| `etym` | object | Sin subcampo `gloss` |
| `evo` | `object[]` | Siempre vacío (`[]`) |
| `deriv` | `object[]` | Idéntico (3–5 items) |
| `cogn` | `object[]` | Idéntico (2 items) |
| `example` | `string` | String simple, no objeto rico |
| `cmp` | object | Solo 5 lenguas (sin `de` alemán) |
| `researchNotes` | — | No presente |
| `relatedEntries` | — | No presente |
| `famousPhrases` | — | No presente |
| `negativeTheologyTags` | — | No presente |
| `sources` | — | No presente |

El código JavaScript maneja ambas variantes mediante comprobaciones de tipo en tiempo de renderizado.

---

## Corpus teórico y fuentes

SENSUS GRAECUS opera desde la tradición filosófica griega:

- **Werner Jaeger** — *Paideia: los ideales de la cultura griega* (1933–1947). La legalidad inmanente como principio estético y ético. La base teórica de este diccionario.
- **Liddell, Scott & Jones** — *A Greek-English Lexicon* (1940). Referencia lexicográfica estándar.
- **Calvert Watkins** — *The American Heritage Dictionary of Indo-European Roots*. Etimología PIE.
- **G.S. Kirk, J.E. Raven, M. Schofield** — *Los filósofos presocráticos* (1983). Para el contexto de las raíces del pensamiento.
- **Perseus Digital Library** — Corpus textual y herramientas morfológicas.
- **Logeion** — Interfaz unificada para LSJ.

### Tradición filosófica cubierta

Las 31 entradas abarcan tres períodos:

- **Presocráticos** — arche, physis, kosmos, aether, nous, dynamis
- **Clásico (siglos V–IV a.C.)** — logos, aletheia, eudaimonia, arete, paideia, agon, mimesis, catharsis, eros, demos, polis, demokratia, agora, theos, hubris, nomos, pragma, aisthesis, kairos, phronesis, sophia
- **Helenístico** — moira, kenoma, soma, gnosis, philosophia

---

## Diseño como posición

SENSUS GRAECUS comparte la estética de Paula Scher con SENSUS LATINUS: tipografía como imagen, composición diagonal, monocromático con acento rojo. La diferencia está en el contenido: donde LATINUS explora la geología del sonido, GRAECUS explora la arquitectura del concepto.

- **Crema `#f5f0e8`** — El pergamino como metáfora del pensamiento que perdura.
- **Negro `#0a0a0a`** — La tinta como herramienta de precisión.
- **Rojo `#c23b22`** — La marca del significado que persiste.

El diseño rechaza la ilustración decorativa y confía en la tipografía para construir significado visual. Una entrada de diccionario es también un micro-ensayo visual donde la jerarquía tipográfica guía el ojo desde el lema griego hacia la definición, de ahí a la etimología, y finalmente a los derivados en lenguas modernas.

---

## Cómo usarlo

### Opción A — Clonar el repositorio
```bash
git clone https://github.com/NigelMoonwriter/sensus_graecus.git
```
Abrir `sensus-graecus.html` en cualquier navegador.

### Opción B — Descargar directamente
Ir al repositorio → `sensus-graecus.html` → Download raw file → doble clic.

### Opción C — Usar en línea
**[sensus-graecus en GitHub Pages](https://nigelmoonwriter.github.io/sensus_graecus/)**

---

## Parte del Entorno Greka

| Diccionario | Campo | Entradas |
|---|---|---|
| [SENSUS LATINUS](https://github.com/NigelMoonwriter/sensus_latinus) | Latín · Griego | 27 |
| [SENSUS GRAECUS](https://github.com/NigelMoonwriter/sensus_graecus) | Griego clásico | 31 |
| [SENSUS SEMANNSIS](https://github.com/NigelMoonwriter/sensus_semannsis) | Griego · IA | 61 |
| [SENSUS NEPANTLA](https://github.com/NigelMoonwriter/sensus_nepantla) | Spanglish | 27 |

El índice central: [entorno_greka](https://github.com/NigelMoonwriter/entorno_greka)

---

## Licencia

`CC BY-NC-SA 4.0` — Libre para uso y adaptación no comercial con atribución.

---

**Rei García / KhaosLiminal / Sarayu Aguilar**
Morelia, Michoacán, México — 2026

*La libertad no es romper la ley, sino reconocerla como inmanente.*