# 🎨 LECCIÓN 5 — Estilos y Diseño Simple
### Script de presentación
 
---
Bienvenidos a la **Lección 5: Estilos y Diseño Simple**.
 
Hoy vamos a aprender a darle vida a nuestro HTML usando CSS. Veremos cómo aplicar colores, bordes y cómo centrar elementos como un profesional. ⚡
 
---
 
## ¿Qué vamos a aprender hoy?
 
En esta lección cubriremos cuatro temas principales:
 
1. **Colores de fondo y texto** — Usaremos `background-color` y `color` para transformar el aspecto de nuestros elementos.
2. **Bordes personalizados** — Le daremos personalidad a nuestras cajas con la propiedad `border`, controlando el grosor, el estilo y el color.
3. **Centrar contenido** — Veremos la diferencia entre `text-align: center` para texto, y `margin: 0 auto` para cajas completas.
4. **Práctica real** — Al final crearemos una tarjeta de oferta llamativa con todo lo aprendido.
---
 
## Propiedad CSS #1: Colores
 
Las dos propiedades más básicas para cambiar la apariencia de un elemento son:
 
- **`background-color`** → controla el color de fondo. Acepta nombres en inglés como `yellow`, valores hexadecimales como `#fffacd`, o RGB.
- **`color`** → controla el color del texto. Siempre debemos buscar buen contraste con el fondo.
💡 **Tip:** Usa hexadecimales de 6 dígitos para mayor precisión. Por ejemplo, `#27ae60` es verde y `#d35400` es naranja.
 
---
 
##  Bordes con personalidad
 
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
 
## Centrar texto vs. centrar una caja
 
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
 
## Padding: el espacio interno
 
El **padding** es el espacio entre el contenido y el borde del elemento. Sin él, el texto queda pegado al borde y se ve mal.
 
```css
padding: 20px;           /* 20px en los cuatro lados */
padding: 10px 20px;      /* 10px arriba/abajo, 20px izquierda/derecha */
```
 
En botones, el padding los hace más grandes y fáciles de hacer clic. Siempre añádelo para dar respiro visual al contenido.
 
---
 
Bien, ahora vamos a ver cómo todo esto funciona junto en un ejemplo real. Tenemos dos archivos: el HTML y el CSS. Los voy a explicar parte por parte.
 
---
 
### 🗂️ El HTML
 
```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lección 5 - Estilo Simple</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="header">
    <h1>Mi primera página con estilo</h1>
    <p>Aprendiendo CSS básico 🎨</p>
  </header>
  <div class="card">
    <h2>¡Hola!</h2>
    <p>Este es un ejemplo de cómo aplicar colores, bordes y centrado.</p>
  </div>
  <div class="card">
    <h2>¿Qué aprendimos?</h2>
    <p>Podemos cambiar colores, centrar texto y también centrar cajas con CSS.</p>
  </div>
</body>
</html>
```
 
Aquí tenemos la estructura base. Fíjense en tres cosas importantes:
 
- El `<link rel="stylesheet" href="styles.css">` en el `<head>` es lo que conecta nuestro HTML con el archivo CSS. Sin esta línea, no habría estilos.
- Tenemos un `<header>` con la clase `header` — esa clase es la que vamos a usar desde el CSS para aplicarle estilos.
- Debajo hay dos `<div>` con la clase `card`. Ambos comparten la misma clase, así que los dos van a recibir exactamente los mismos estilos automáticamente.
---
 
### 🎨 El CSS
 
```css
/* Fondo general de la página */
body {
  background-color: #f2f6ff;
  font-family: Arial, sans-serif;
  margin: 0;
}
```
 
Empezamos con el `body` — esto afecta a toda la página. Le damos un fondo azul muy suave con `#f2f6ff`, definimos la fuente como Arial, y con `margin: 0` eliminamos el espacio blanco que los navegadores añaden por defecto alrededor de todo.
 
```css
/* Encabezado */
.header {
  background-color: #4a90e2;
  color: white;
  text-align: center;
  padding: 20px;
}
```
 
Aquí estilizamos el encabezado. Usamos `background-color` para darle ese azul más fuerte, `color: white` para que el texto sea legible — buen contraste —, `text-align: center` para centrar el texto dentro del header, y `padding: 20px` para que el contenido no quede pegado al borde.
 
```css
/* Tarjetas */
.card {
  background-color: white;
  width: 60%;
  margin: 20px auto;
  padding: 20px;
  border: 2px solid #4a90e2;
  border-radius: 10px;
}
```
 
Esta es la parte más importante. Aquí aplicamos todo lo que vimos en la lección:
 
- `width: 60%` — le damos un ancho fijo. Sin esto, lo que viene a continuación no funcionaría.
- `margin: 20px auto` — los `20px` son el espacio arriba y abajo, y el `auto` centra la caja horizontalmente. Esto es exactamente lo que vimos con `margin: 0 auto`, pero con un poco de espacio vertical.
- `padding: 20px` — espacio interno para que el texto respire.
- `border: 2px solid #4a90e2` — borde sólido azul de 2px.
- `border-radius: 10px` — esto es nuevo y es un regalo: redondea las esquinas de la caja. Cuanto mayor el número, más redondeadas.
```css
/* Títulos y párrafos dentro de las tarjetas */
.card h2 {
  color: #4a90e2;
  text-align: center;
}
 
.card p {
  color: #333;
  text-align: center;
}
```
 
Por último, estilizamos los elementos dentro de las tarjetas. `.card h2` significa "los `h2` que están dentro de un elemento con clase `card`" — esto se llama selector descendente. El color `#333` es un gris oscuro, más suave que el negro puro, que es más agradable de leer.
 
---
 
## Resumen ✅
 
Hoy aprendimos cuatro conceptos clave de CSS:
 
- **`background-color` y `color`** → controlan el fondo y el texto. Usar hexadecimales da más precisión.
- **`border` en 3 partes** → grosor + estilo + color. Ejemplo: `3px dashed #ff8c00`.
- **Dos técnicas para centrar** → `text-align: center` para texto, y `margin: 0 auto` + `width` para cajas.
- **`padding` da respiro visual** → sin padding, el contenido pega al borde. ¡Siempre añádelo!
---
 
*Fin de la Lección 5*
