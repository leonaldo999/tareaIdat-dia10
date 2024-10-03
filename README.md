# [![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=30F714&background=703BE2BE&center=true&vCenter=true&width=435&lines=Dia+10+tarea;Estilos+de+texto+CSS;Sesion+02+CSS;IDAT+frontEnd)](https://git.io/typing-svg)

## PROPIEDADES

- [](#)
  - [PROPIEDADES](#propiedades)
    - [COLOR EN EL TEXTO (color)](#color-en-el-texto-color)
    - [TAMAÑO DE TEXTO (font-size)](#tamaño-de-texto-font-size)
    - [PESO DE TIPOGRAFIA (font-weight)](#peso-de-tipografia-font-weight)
    - [RECETEADOR DEL ESTILO](#receteador-del-estilo)
    - [GOOGLE fonts @font-face (font-family)](#google-fonts-font-face-font-family)
      - [Formas de llamado](#formas-de-llamado)
    - [TRANSFORMACION DE TEXTO (text-transform)](#transformacion-de-texto-text-transform)
      - [Valores posibles de (font-family)](#valores-posibles-de-font-family)
    - [Alinear Texto (text-align)](#alinear-texto-text-align)
      - [Valores posibles de text-align](#valores-posibles-de-text-align)
    - [Estilos de texto (font-style)](#estilos-de-texto-font-style)
      - [Valores posibles de font-style](#valores-posibles-de-font-style)
    - [Decoración de Texto (text-decoration)](#decoración-de-texto-text-decoration)
      - [Valores posibles de text-decoration](#valores-posibles-de-text-decoration)
    - [Espaciado entre letras (Letter-Spacing)](#espaciado-entre-letras-letter-spacing)
      - [Valores posibles de letter-spacing](#valores-posibles-de-letter-spacing)
    - [Espaciado entre palabras (word-spacing)](#espaciado-entre-palabras-word-spacing)
      - [Valores posibles de word-spacing](#valores-posibles-de-word-spacing)

---

[</br>](html)

### COLOR EN EL TEXTO (color)

 >El color de texto en CSS se establece utilizando la propiedad color. Esta propiedad permite definir el color del texto en un elemento HTML. Por ejemplo, para establecer el color del texto en rojo, se puede utilizar el siguiente código:

- color: #FF0000;
- color: rgb(255, 0, 0);
- color: hsl(0, 100%, 50%);
- color: hwb(0, 0%, 0%);

 >A continuación, te presento un breve resumen de los diferentes valores que se pueden asignar a la propiedad color en CSS:

- color: red; (predefinido)
- color: #000000 (hexadecimal)
- color: rgb(0, 128, 0) (RGB)
- color:  rgba(0, 128, 0, 0.5) (RGBA)

```html
<h2>Color en texto</h2>
```

```css
h2 {
    color: #ff0000;
  }
```

---

[</br>](html)

### TAMAÑO DE TEXTO (font-size)

 >El tamaño de fuente en CSS se establece utilizando la propiedad font-size. Esta propiedad permite definir el tamaño de la fuente en un elemento HTML. Por ejemplo, para establecer el tamaño de la fuente en 26 píxeles, se puede utilizar el siguiente código:

```html
<h2>TAMAÑO DE TEXTO (font-size)</h2>
```

```css
h2 {
  font-size: 26px;
}
```

 > **NOTA**
 >
 >Un px es la unidad de medida para los tamanos
 >
 >1. px: Unidad absoluta o unidad de medida
 >2. em: Unidad del ancestro, si no se especifica tamaño al padre x defaullt 16px
 >3. rem: Unidad de etiqueta HTML

```css
/* em: Unidad del ancestro, si no se especifica tamaño al padre x defaullt 16px */
section {
  font-size: 10px;
}

h2 {
  color: red;
  font-size: 4em;
} 

/* rem: Unidad de etiqueta HTML*/
html {
  font-size: 10px;
}

h2 {
  color: red;
  font-size: 4rem;
}  
```

---

[</br>](html)

### PESO DE TIPOGRAFIA (font-weight)

> El peso de la fuente en CSS se establece utilizando la propiedad font-weight. Esta propiedad permite definir el grosor o peso de la fuente en un elemento HTML. Por ejemplo, para establecer el peso de la fuente en negrita, se puede utilizar el siguiente código:

```html
<h2>PESO DE TIPOGRAFIA (font-weight)</h2>
```

```css
h2 {
  font-weight: 800;
}
```

> **VALORES POSIBLES DE FONT-WEIGHT**
>
>- 100-300: fuentes delgadas (_lighter_)
>- 400: fuente normal (_normal_)
>- 500-700: fuentes seminegritas (_bolder_)
>- 800-900: fuentes negritas (_bold_)

---

[</br>](html)

### RECETEADOR DEL ESTILO

 >Una alternativa moderna y compatible con HTML5 a los restablecimientos de CSS. Normalize.css hace que los navegadores representen todos los elementos de manera más uniforme y acorde con los estándares modernos.

```html
  <a href="https://necolas.github.io/normalize.css/">Normalizar.css</a>
```

### GOOGLE fonts @font-face (font-family)

 > [**Google Fonts**](https://fonts.google.com/)
 >
 >Es una colección de fuentes de código abierto que se pueden utilizar de forma gratuita en sitios web y productos. Permite a los desarrolladores y diseñadores agregar personalidad y rendimiento a sus proyectos a través de una amplia variedad de fuentes de alta calidad.
 ---

#### Formas de llamado

>1. **@import**: Importa carga las fuentes de Google Fonts en tu proyecto.

```html
p {
  font-family: "Roboto",serif;
  font-weight: 500;
}
```

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');
```

>2. **@font-face**: Utiliza la propiedad @font-face para cargar fuentes de Google de manera local

```html
<h2>Google fonts - @font-face (font-family)</h2>
```

```css
@font-face {
  font-family: "Roboto Condensed", sans-serif;
  src: url(../estio-texto/fonts/RobotoCondensed-Italic-VariableFont_wght.ttf);
  font-weight: normal;
  font-style: italic;
}

h2 {
  color: red;
  font-family: "Roboto Condensed", Arial, Helvetica, sans-serif;
  font-weight: 700;
}
```

---

[</br>](html)

### TRANSFORMACION DE TEXTO (text-transform)

 >La propiedad **text-transform** en CSS se utiliza para controlar la forma en que se muestra el texto en un elemento HTML. Esta propiedad permite transformar el texto en mayúsculas, minúsculas, título o dejarlo sin cambios.

#### Valores posibles de (font-family)

- **none**: No aplica ninguna transformación al texto.
- **capitalize**: Convierte la primera letra de cada palabra en mayúscula y el resto en minúscula.
- **uppercase**: Convierte todo el texto en mayúscula.
- **lowercase**: Convierte todo el texto en minúscula.
- **inherit**: Hereda el valor de la propiedad - text-transform del elemento padre.

>- _EJEMPLOS_

```css
/* Dejar el texto sin cambios: */
span {
  text-transform: none;
}

/* Convierte la primera letra de cada palabra en mayúscula: */
p {
  text-transform: capitalize;
}

/* Convierte todo el texto en mayúscula: */
h1 {
  text-transform: uppercase;
}

/* Convierte todo el texto en minúscula. */
h2 {
  text-transform: lowercase;
}

/* Hereda el valor de la propiedad - text-transform del elemento padre */
h2 {
  text-transform: inherit;
}
```

 ---

[</br>](html)

### Alinear Texto (text-align)

 >La propiedad **text-align** en CSS se utiliza para controlar la alineación horizontal del texto dentro de un elemento HTML. Esta propiedad permite alinear el texto a la izquierda, derecha, centro o justificarlo.

#### Valores posibles de text-align

- **left**: Alinea el texto a la izquierda del elemento.
- **right**: Alinea el texto a la derecha del elemento.
- **center**: Alinea el texto en el centro del elemento.
- **justify**: Justifica el texto, es decir, ajusta el espacio entre las palabras para que el texto se extienda desde la izquierda hasta la derecha del elemento.
- **inherit**: Hereda el valor de la propiedad text-align del elemento padre.

>- _EJEMPLOS_

```CSS
/* Alinea el texto a la izquierda del elemento. */
text-align: left;

/* Alinea el texto a la derecha del elemento. */
text-align: right;

/* Alinea el texto en el centro del elemento. */
text-align: center;

/* Justifica el texto. */
text-align: justify;

/*  Hereda el valor de la propiedad text-align del elemento padre. */
text-align: inherit;
```

 ---

[</br>](html)

### Estilos de texto (font-style)

 > La propiedad **font-style** en CSS se utiliza para definir el estilo de fuente de un elemento HTML, como si es normal, cursiva o oblicua

#### Valores posibles de font-style

- **normal**: Establece el estilo de fuente en normal (no cursiva ni oblicua).
- **italic**: Establece el estilo de fuente en cursiva.
- **oblique**: Establece el estilo de fuente en oblicua (similar a cursiva, pero con una inclinación más pronunciada).

>- _EJEMPLO_

```css
/* Establece el estilo de fuente en normal. */
font-style: normal;

/* Establece el estilo de fuente en cursiva. */
font-style: italic;

/* Establece el estilo de fuente en oblicua. */
font-style: oblique;
```

>Nota:
>
> Es importante tener en cuenta que la propiedad font-style solo funciona si la fuente utilizada tiene una variante cursiva o oblicua disponible. De lo contrario, el navegador no podrá aplicar el estilo de fuente deseado.

 ---

[</br>](html)

### Decoración de Texto (text-decoration)

 >La propiedad **text-decoration** en CSS se utiliza para agregar decoraciones al texto, como subrayados, tachados o sobrelineados.

#### Valores posibles de text-decoration

- **none**: No aplica ninguna decoración al texto.
- **underline**: Agrega un subrayado al texto.
- **overline**: Agrega un sobrelineado al texto.
- **line-through**: Agrega un tachado al texto.
- **inherit**: Hereda el valor de la propiedad text-decoration del elemento padre.

>- EJEMPLO:

```css
/* No aplica ninguna decoración al texto. */
text-decoration: none;

/* Agrega un subrayado al texto. */
text-decoration: underline;

/* Agrega un sobrelineado al texto. */
text-decoration: overline;

/* Agrega un tachado al texto. */
text-decoration: line-through;

/* Hereda el valor de la propiedad text-decoration del elemento padre. */
text-decoration: inherit;
```

 ---

[</br>](html)

### Espaciado entre letras (Letter-Spacing)

 > La propiedad letter-spacing en CSS se utiliza para controlar el espacio entre letras en un texto. Esta propiedad permite aumentar o disminuir el espacio entre letras para mejorar la legibilidad o crear un efecto visual específico.

#### Valores posibles de letter-spacing

- normal: Establece el espacio entre letras en su valor predeterminado.
- length: Establece el espacio entre letras en un valor específico, como px, em, %, etc.
- inherit: Hereda el valor de la propiedad letter-spacing del elemento padre.

>- _EJEMPLOS_:

```css
/* Establece el espacio entre letras en su valor predeterminado. */
letter-spacing: normal;

/* Establece el espacio entre letras en un valor específico, como px, em, %, etc. */
letter-spacing: 10px;

/* Hereda el valor de la propiedad letter-spacing del elemento padre. */
letter-spacing: inherit;
```

> **Nota**:
>
> Es importante tener en cuenta que la propiedad letter-spacing solo se aplica al texto y no a los elementos en sí. Además, algunos navegadores pueden tener comportamientos diferentes al aplicar esta propiedad.

 ---

[</br>](html)

### Espaciado entre palabras (word-spacing)

 >La propiedad **word-spacing** en CSS se utiliza para controlar el espacio entre palabras en un texto. Esta propiedad permite aumentar o disminuir el espacio entre palabras para mejorar la legibilidad o crear un efecto visual específico.

#### Valores posibles de word-spacing

- **normal**: Establece el espacio entre palabras en su valor predeterminado.

- **length**: Establece el espacio entre palabras en un valor específico, como px, em, %, etc.

- **inherit**: Hereda el valor de la propiedad word-spacing del elemento padre.

```css
/* Establece el espacio entre palabras en su valor predeterminado. */
word-spacing: normal;

/*  Establece el espacio entre palabras en un valor específico, como px, em, %, etc. */
word-spacing: 8px;

/* Hereda el valor de la propiedad word-spacing del elemento padre. */
word-spacing: inherit;
```

> **Nota**:
>
> Es importante tener en cuenta que la propiedad word-spacing solo se aplica al texto y no a los elementos en sí. Además, algunos navegadores pueden tener comportamientos diferentes al aplicar esta propiedad.

 ---

[</br>](html)

<!-- 
# TAREA

  Actualizar el repositorio con lo visto en la 2da parte
  1) Explicar los conceptos con ejemplos
  2) (Agregar una nueva tipografia de google fonts, usando font-face)
-->