# 🎨 LECCIÓN 5 — Estilos y Diseño Simple
### Script de presentación
 
---

## 📍 Diapositiva 1 — Portada

Bienvenidos a la **Lección 5: Estilos y Diseño Simple**.

Hoy vamos a aprender a darle vida a nuestro HTML usando CSS. Veremos cómo aplicar colores, bordes y cómo centrar elementos como un profesional. ⚡
 
---

## 📍 Diapositiva 2 — ¿Qué vamos a aprender hoy?

En esta lección cubriremos cuatro temas principales:

1. **Colores de fondo y texto** — Usaremos `background-color` y `color` para transformar el aspecto de nuestros elementos.
2. **Bordes personalizados** — Le daremos personalidad a nuestras cajas con la propiedad `border`, controlando el grosor, el estilo y el color.
3. **Centrar contenido** — Veremos la diferencia entre `text-align: center` para texto, y `margin: 0 auto` para cajas completas.
4. **Práctica real** — Al final crearemos una tarjeta de oferta llamativa con todo lo aprendido.
---

## 📍 Diapositiva 3 — Propiedad CSS #1: Colores

Las dos propiedades más básicas para cambiar la apariencia de un elemento son:

- **`background-color`** → controla el color de fondo. Acepta nombres en inglés como `yellow`, valores hexadecimales como `#fffacd`, o RGB.
- **`color`** → controla el color del texto. Siempre debemos buscar buen contraste con el fondo.
  💡 **Tip:** Usa hexadecimales de 6 dígitos para mayor precisión. Por ejemplo, `#27ae60` es verde y `#d35400` es naranja.

---

## 📍 Diapositiva 4 — Bordes con personalidad

La propiedad `border` tiene tres partes que podemos controlar de forma independiente:

- 📏 **Grosor** → `1px`, `3px`, `5px`... mientras más grueso, más visible.
- ✏️ **Estilo** → `solid` (línea continua), `dashed` (guiones), `dotted` (puntos), `double` (doble línea).
- 🎨 **Color** → cualquier valor válido: nombre, hexadecimal o RGB.
  **Ejemplo completo:**
```css
border: 3px dashed #ff8c00;
```
Esto genera un borde punteado, naranja, de 3 píxeles.
 
---

## 📍 Diapositiva 5 — Centrar texto vs. centrar una caja

Este es el error más común entre principiantes. ¡No son lo mismo!

**`text-align: center`** → centra el *contenido de texto* dentro de un elemento.
```css
h1 {
  text-align: center;
}
```

**`margin: 0 auto`** → centra la *caja completa* en la pantalla. Requiere un `width` definido.
```css
.tarjeta {
  width: 350px;
  margin: 0 auto;
}
```

⚠️ **Importante:** Sin `width`, `margin: 0 auto` no funciona. El navegador necesita saber el ancho de la caja para poder calcular los márgenes automáticos a cada lado.
 
---

## 📍 Diapositiva 6 — Padding: el espacio interno

El **padding** es el espacio entre el contenido y el borde del elemento. Sin él, el texto queda pegado al borde y se ve mal.

```css
padding: 20px;           /* 20px en los cuatro lados */
padding: 10px 20px;      /* 10px arriba/abajo, 20px izquierda/derecha */
```

En botones, el padding los hace más grandes y fáciles de hacer clic. Siempre añádelo para dar respiro visual al contenido.
 
---

## 📍 Diapositiva 7 — Proyecto Final: Tarjeta de Oferta 🎯

Ahora vamos a poner en práctica todo lo aprendido creando una **tarjeta promocional llamativa**.

Seguiremos estos pasos en orden, y veremos cómo cada propiedad transforma el resultado:

1. **HTML base** — Escribimos la estructura.
2. **Centrar la caja** — Aplicamos `width` y `margin: 0 auto`.
3. **Colores y bordes** — Le damos personalidad visual.
4. **Estilizar el botón** — Creamos un botón de acción atractivo.
---

## 📍 Diapositiva 10 — Resumen ✅

Hoy aprendimos cuatro conceptos clave de CSS:

- **`background-color` y `color`** → controlan el fondo y el texto. Usar hexadecimales da más precisión.
- **`border` en 3 partes** → grosor + estilo + color. Ejemplo: `3px dashed #ff8c00`.
- **Dos técnicas para centrar** → `text-align: center` para texto, y `margin: 0 auto` + `width` para cajas.
- **`padding` da respiro visual** → sin padding, el contenido pega al borde. ¡Siempre añádelo!
---

*Fin de la Lección 5*
