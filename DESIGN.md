---
colors:
  primary: "#113051"
  background: "#F9F7EF"
  surface: "#FFFFFF"
  ink: "{colors.primary}"
  ink-on-background: "{colors.primary}"
  ink-on-primary: "{colors.background}"
  muted: "rgba(17, 48, 81, 0.72)"
  line: "{colors.primary}"
  border-subtle: "rgba(17, 48, 81, 0.18)"
  overlay: "rgba(17, 48, 81, 0.06)"
typography:
  display:
    fontFamily: "'Handsome Pro', cursive"
    fontWeight: 400
    fontSize: "clamp(48px, 6vw, 76px)"
    lineHeight: 1.05
    letterSpacing: "0em"
    color: "{colors.primary}"
    usage: "Solo titulos principales de grandes secciones"
  heading:
    fontFamily: "'Kumbh Sans', sans-serif"
    fontWeight: 700
    fontSize: "28px"
    lineHeight: 1.2
    color: "{colors.primary}"
  subheading:
    fontFamily: "'Kumbh Sans', sans-serif"
    fontWeight: 600
    fontSize: "20px"
    lineHeight: 1.3
    color: "{colors.primary}"
  body:
    fontFamily: "'Kumbh Sans', sans-serif"
    fontWeight: 400
    fontSize: "16px"
    lineHeight: 1.6
    color: "{colors.primary}"
  body-strong:
    fontFamily: "'Kumbh Sans', sans-serif"
    fontWeight: 600
    fontSize: "{typography.body.fontSize}"
    lineHeight: "{typography.body.lineHeight}"
    color: "{colors.primary}"
  caption:
    fontFamily: "'Kumbh Sans', sans-serif"
    fontWeight: 500
    fontSize: "14px"
    lineHeight: 1.5
    color: "{colors.muted}"
  number:
    fontFamily: "'Kumbh Sans', sans-serif"
    fontWeight: 700
    fontSize: "clamp(40px, 5vw, 64px)"
    lineHeight: 1.0
    color: "{colors.primary}"
spacing:
  base: 8
  scale:
    xs: "4px"
    sm: "8px"
    md: "16px"
    lg: "24px"
    xl: "32px"
    2xl: "48px"
    3xl: "64px"
    4xl: "96px"
  section-gap: "{spacing.scale.4xl}"
  card-gap: "{spacing.scale.lg}"
  text-gap: "{spacing.scale.md}"
rounded:
  sm: "8px"
  md: "12px"
  lg: "16px"
  pill: "999px"
  circle: "50%"
components:
  button-primary:
    shape: "{rounded.pill}"
    background: "{colors.primary}"
    textColor: "{colors.ink-on-primary}"
    font: "{typography.body-strong.fontFamily}"
    padding: "{spacing.scale.sm} {spacing.scale.lg}"
    border: "1px solid {colors.primary}"
    hover-background: "{colors.primary}"
    hover-detail: "linea, flecha o textura sutil"
  button-secondary:
    shape: "{rounded.pill}"
    background: "{colors.background}"
    textColor: "{colors.primary}"
    border: "1px solid {colors.primary}"
    padding: "{spacing.scale.sm} {spacing.scale.lg}"
  card:
    background: "{colors.background}"
    texture: "paper-subtle"
    border: "1px solid {colors.border-subtle}"
    radius: "{rounded.md}"
    shadow: "0 1px 2px {colors.overlay}, 0 4px 16px {colors.overlay}"
    padding: "{spacing.scale.lg}"
  card-skill:
    extends: "{components.card}"
    usage: "Habilidades en reticula visual, no lista tradicional"
  card-contact:
    extends: "{components.card}"
    layout: "icono + nombre"
    radius: "{rounded.md}"
    usage: "Email, Instagram, LinkedIn, Behance, Telefono"
  nav-item:
    number-font: "{typography.number.fontFamily}"
    text-font: "{typography.body.fontFamily}"
    color: "{colors.primary}"
    active-style: "linea o subrayado en {colors.primary}"
    sections: ["01 Sobre mi", "02 Habilidades", "03 Herramientas", "04 Educacion", "05 Proyectos", "06 Contacto"]
  link:
    color: "{colors.primary}"
    decoration: "subrayado fino 1px"
    hover: "subrayado con pequeno desplazamiento o flecha"
  image-project:
    background: "{colors.surface}"
    radius: "{rounded.lg}"
    treatment: "fondo neutro, buena iluminacion, mockup cuidado, sin filtros"
  tool-item:
    font: "{typography.caption.fontFamily}"
    color: "{colors.primary}"
    layout: "logotipo + nombre"
---

## Overview

CV digital de Sofia Ramos Ferra, disenadora grafica.

Sistema que parte de la identidad personal: el logotipo funciona como firma personal manuscrita y es el punto de partida de toda la identidad, no un elemento aislado. El resto del sistema le da estructura para transmitir confianza y profesionalismo.

Personalidad objetivo: creativa, profesional, moderna y divertida, sin llegar a sentirse demasiado artistica, infantil, vintage o generica.

Idea central: hacer que la identidad personal y el trabajo como disenadora formen parte de una misma experiencia visual, cercana y personal pero organizada y funcional. Equilibrio entre estetica editorial y recursos espontaneos como collage, textura y numeros grandes.

Elementos siempre reconocibles: `{colors.primary}`, `{colors.background}`, tipografia display y `{typography.body.fontFamily}`, numeracion de secciones, lineas y marcos, textura de papel, collage y `{rounded.md}`.

## Colors

La identidad se construye con azul profundo y beige, mas neutros solo de apoyo. La variedad visual se consigue con composicion, imagen, textura y escala, no con mas croma.

- **Primary e identidad y contraste, `{colors.primary}`:** azul profundo #113051. Titulos, numeros grandes (`{typography.number}`), lineas, navegacion (`{components.nav-item}`), botones (`{components.button-primary}`) y bloques separadores entre secciones. Funciona tanto en pequenos detalles como en areas amplias.
- **Background y fondo principal, `{colors.background}`:** beige #F9F7EF, calido y cercano, siempre con textura de papel sutil pero visible. Aporta materialidad sin llevar la identidad a vintage.
- **Surface y apoyo, `{colors.surface}`:** blanco y neutros solo cuando sea necesario, por ejemplo fondos de foto de proyecto o mockups. No compiten con los dos colores principales.
- **Texto:** principal `{colors.ink}` sobre claro, invertido `{colors.ink-on-primary}` sobre `{colors.primary}`, secundario `{colors.muted}` para metadatos y captions como Nombre, Categoria, Ano y descripcion breve.
- **Lineas y bordes:** `{colors.line}` en 1px fino y delicado, `{colors.border-subtle}` para marcos de tarjeta (`{components.card}`).

Combinacion por defecto: texto `{colors.primary}` sobre `{colors.background}` con textura. Bloques invertidos con fondo `{colors.primary}` y texto `{colors.background}` como separadores entre secciones.

## Typography

Voz tipografica en dos familias con contraste moderado: los titulos tienen presencia pero no dominan, los proyectos son protagonistas.

- **Display, `{typography.display.fontFamily}`:** manuscrita, ligada al lettering del logotipo. Solo titulos principales de grandes secciones. No se usa en textos largos ni en interfaz. Token `{typography.display.fontSize}` con `{typography.display.lineHeight}` y color `{typography.display.color}`.
- **Funcional, `{typography.body.fontFamily}`:** Kumbh Sans para todo lo demas. Jerarquia por peso, tamano y color sin recurrir a Display:
  - `{typography.heading}` para titulos secundarios.
  - `{typography.subheading}` para subtitulos y categorias.
  - `{typography.body}` y `{typography.body-strong}` para parrafos y enfasis.
  - `{typography.caption}` en `{colors.muted}` para metadatos de proyecto con formato Nombre, Categoria, Ano y descripcion breve, y para etiquetas de herramientas.
  - `{typography.number}` para numeros estructurales 01 a 06 con funcion de orientacion, no decorativa.
- **Pesos Kumbh Sans:** 400, 500, 600 y 700 para diferenciar informacion, categorias y pequenos enfasis.
- **Portafolio de unas 20 obras en cuatro categorias:** Motion graphics, Identidad visual y Packaging, Editorial e Ilustracion. El texto es siempre breve y secundario frente a la imagen.

## Layout

Estructura ordenada pero dinamica, con espacio en blanco moderado que separa y crea pausas sin vaciar la pagina.

- **Reticula:** 12 columnas en escritorio como base para imagenes, textos, tarjetas (`{components.card}`) y collage. Los elementos pueden variar tamano, posicion y proporcion dentro de la reticula para una composicion editorial, sobre todo en Proyectos.
- **Espaciado:** escala en multiplos de `{spacing.base}px` con `{spacing.scale.xs}`, `{spacing.scale.sm}`, `{spacing.scale.md}`, `{spacing.scale.lg}`, `{spacing.scale.xl}`, `{spacing.scale.2xl}`, `{spacing.scale.3xl}` y `{spacing.scale.4xl}`. Se aplica a textos con `{spacing.text-gap}`, tarjetas con `{spacing.card-gap}` y secciones con `{spacing.section-gap}`.
- **Contenido en orden:** 1 Sobre mi como presentacion personal con interes en investigacion, organizacion, resolucion de problemas, narracion visual y estrategia, 2 Habilidades en tarjetas (`{components.card-skill}`) con Conceptualizacion, Investigacion, Resolucion de problemas, Composicion, Tipografia, Branding, Comunicacion visual, Storytelling, Organizacion, Atencion al detalle, Pensamiento creativo y estrategico, Trabajo en equipo y Presentacion de proyectos, 3 Herramientas con logotipo mas nombre (`{components.tool-item}`) para Illustrator, Photoshop, InDesign, After Effects, Figma, Procreate, Maya y HTML y CSS, 4 Educacion solo con universidad y carrera, 5 Proyectos en cuatro categorias, 6 Contacto con `{components.card-contact}`.
- **Adaptable:** en escritorio 12 columnas, al reducir el espacio la reticula se adapta y los elementos se reorganizan y cambian posicion y proporcion. No es solo un escalado. En movil se conservan `{colors.primary}`, `{colors.background}`, tipografias, numeracion, lineas y marcos, textura, collage y `{rounded.md}`.

## Elevation & Depth

Profundidad minima. La jerarquia se logra con color, escala, lineas y textura, no con elevacion.

- **Regla:** sombras muy sutiles y solo cuando ayuden a separar elementos, tipicamente `{components.card}`. Nada de sombras duras, largas o coloreadas.
- **Token usado:** sombra de tarjeta con `{colors.overlay}` sobre `{colors.background}` con textura.
- **Sin elevacion:** botones (`{components.button-primary}` y `{components.button-secondary}`) que cambian por color y detalle grafico como linea, flecha o textura, navegacion, imagenes de proyecto con fondo `{colors.surface}` plano y collage decorativo.
- **Orden visual:** primero fondo `{colors.background}` con textura, luego lineas y marcos `{colors.border-subtle}`, luego tarjetas `{components.card}` con sombra minima, y al frente botones capsula sin sombra.

## Shapes

Formas cercanas y amables que suavizan la reticula ordenada.

- **Radios:** tarjetas y contenedores con `{rounded.md}` ligeramente redondeadas, imagenes editoriales con `{rounded.lg}`, botones siempre con `{rounded.pill}` en forma capsula (`{components.button-primary.shape}`) para diferenciarse de tarjetas, `{rounded.circle}` solo para iconos si se necesita.
- **Lineas finas 1px en `{colors.primary}`:** separadores, subrayados de titulos y enlaces (`{components.link}`) y marcos delicados de tarjeta. Nunca gruesas ni pesadas.
- **Numeros grandes (`{typography.number}`):** 01 Sobre mi hasta 06 Contacto, estructurales y en `{colors.primary}`.
- **Textura de papel:** sobre `{colors.background}`, sutil pero visible en toda la pantalla.
- **Collage:** papeles, recortes y texturas, estrictamente decorativo y en dosis pequenas. Jamas sustituye ni compite con fotos de proyecto.

## Components

Todos heredan color, tipo, espaciado y radio de los tokens.

- **Botones con forma capsula `{rounded.pill}`:**
  - Primario `{components.button-primary}` con fondo `{colors.primary}`, texto `{colors.ink-on-primary}` y padding `{spacing.scale.sm} {spacing.scale.lg}`. En interaccion cambia de color y muestra un pequeno detalle grafico como linea, flecha o textura.
  - Secundario `{components.button-secondary}` con fondo `{colors.background}`, texto `{colors.primary}` y borde de 1px en `{colors.primary}`.
  - Interaccion sobria con pequenos momentos de sorpresa, sin saturar de animaciones.
- **Tarjetas `{components.card}`:** fondo `{colors.background}` con textura, borde de 1px en `{colors.border-subtle}`, radio `{rounded.md}`, sombra minima y padding `{spacing.scale.lg}`. Pueden incorporar marcos finos, textura, collage y esquinas ligeramente redondeadas. Variantes `{components.card-skill}` para habilidades en reticula visual y `{components.card-contact}` con icono mas nombre.
- **Navegacion `{components.nav-item}`:** no es menu tradicional. Numero grande (`{typography.number}`) mas etiqueta (`{typography.body}`) mas linea. Secciones 01 Sobre mi, 02 Habilidades, 03 Herramientas, 04 Educacion, 05 Proyectos y 06 Contacto. Estado activo con linea o subrayado en `{colors.primary}`.
- **Enlaces `{components.link}`:** color `{colors.primary}` con subrayado fino de 1px.
- **Imagenes de proyecto `{components.image-project}`:** tratamiento limpio y profesional con fondo `{colors.surface}`, radio `{rounded.lg}` y sin filtros, con fondos neutros, buena iluminacion y mockups cuidados. Acompanadas solo de Nombre, Categoria, Ano y descripcion breve en `{typography.caption}`.
- **Herramientas `{components.tool-item}`:** logotipo mas nombre en `{typography.caption}`, presentacion limpia sin tarjeta pesada.

## Do's and Don'ts

| Do | Don't |
|---|---|
| Manten la paleta en `{colors.primary}` y `{colors.background}`, usa `{colors.surface}` solo de apoyo. Diversifica con composicion, escala y textura. | No anadas mas colores principales ni degradados o neones. |
| Usa Display (`{typography.display.fontFamily}`) solo en grandes titulos de seccion. | No uses Handsome Pro en parrafos, botones, captions ni interfaz, ni la pongas a competir con Kumbh Sans. |
| Jerarquiza con Kumbh Sans desde `{typography.heading}` hasta `{typography.caption}` por peso, tamano y color. | No mezcles mas familias tipograficas. |
| Usa lineas y marcos finos de 1px (`{components.card}`, `{components.link}`). | No engroses lineas ni uses bordes pesados. |
| Usa textura de papel sutil sobre `{colors.background}` y collage en pequenas dosis decorativas. | No rellenes vacios con textura o collage, no dejes que compitan con fotos de proyecto. |
| Usa tarjetas con `{rounded.md}` y botones siempre con `{rounded.pill}`. | No uses botones rectangulares ni radios grandes o capsula en tarjetas. |
| Usa sombras minimas solo para separar (`{components.card}`). | No uses sombras duras, largas o en botones y navegacion. |
| Usa fotos de proyecto limpias (`{components.image-project}`) con fondo neutro, buena luz y mockup cuidado. | No apliques filtros, fondos recargados ni retoques que compitan con la obra. |
| Respeta reticula de 12 columnas y multiplos de `{spacing.base}px`, con espacio en blanco moderado. | No satures ni vacies, cada grafico debe tener funcion. |
| Conserva el logotipo y firma intacto y siempre legible. | No deformes, alteres colores, recontornees ni uses el logo como textura o fondo. |
| Manten reconocibles en movil `{colors.primary}`, `{colors.background}`, tipografias, numeracion, lineas, textura, collage y `{rounded.md}`. | No hagas del movil un simple escalado, reorganiza sin romper el sistema. |
| Manten tono cercano, personal y editorial, con proyectos primero y texto como contexto. | No suenes generico, infantil, vintage o excesivamente artistico. |
