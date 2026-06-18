# 📹 GUION DE VIDEO - LECCIÓN 3: Construyendo Contenido Web con HTML

**Duración:** 10-12 minutos  
**Público:** Estudiantes de secundaria (12-17 años)  
**Herramientas:** CodePen (editor en línea)  
**Objetivo Final:** Que el estudiante pueda construir una página con títulos, párrafos, listas, imágenes y enlaces

---

## 🎬 INTRODUCCIÓN (0:00 - 0:30)

**MOSTRAR EN PANTALLA:**
- Título: "Lección 3: Construyendo Contenido Web"
- Ejemplo final de portafolio completo

**QUÉ DECIR:**
"¡Hola! En la lección anterior aprendimos la estructura básica de HTML. Hoy vamos a aprender a **llenar esa estructura con contenido real**.

Imagina que estás construyendo una casa:
- Lección anterior = Las vigas y estructura
- Hoy = Las paredes, puertas, ventanas y decoración

Al final de este video, podrás crear **tu propia página de portafolio profesional** con títulos, textos, imágenes y enlaces. ¡Vamos allá!"

---

## 1️⃣ TÍTULOS Y SUBTÍTULOS (0:30 - 2:30)

### DEMOSTRACIÓN EN CODEPEN

**MOSTRAR EN PANTALLA:**
- Abrir CodePen
- Ir a la sección HTML
- Escribir paso a paso:

```html
<h1>Mi Portafolio de Proyectos Web</h1>
<h2>Proyectos Personales</h2>
<h3>Proyecto #1: Sistema de Notas</h3>
```

**QUÉ DECIR (mientras escribes):**

"Los títulos en HTML se crean con las etiquetas `<h1>` a `<h6>`.

- `<h1>` es el **más grande e importante**. Úsalo solo una vez, para el título principal.
- `<h2>` es para **secciones grandes**
- `<h3>` a `<h6>` para **subsecciones cada vez más pequeñas**

Fíjate cómo cada uno es más pequeño que el anterior. Esto ayuda a que tu página sea **ordenada y fácil de leer**.

[PAUSA]

Cosa importante: Google y otros buscadores leen estos títulos para entender de qué trata tu página. Así que ¡úsalos bien!"

**MOSTRAR EN VIVO:**
- El resultado en el navegador
- Cómo se ve cada h1, h2, h3

---

## 2️⃣ PÁRRAFOS (2:30 - 3:30)

### DEMOSTRACIÓN EN CODEPEN

**MOSTRAR EN PANTALLA:**
- Agregar debajo del código anterior:

```html
<p>
  Soy un desarrollador web apasionado por crear experiencias digitales innovadoras.
  Llevo 2 años aprendiendo HTML, CSS y JavaScript.
</p>
```

**QUÉ DECIR:**

"Los párrafos se crean con `<p>`. Es la etiqueta más común para escribir texto.

Mira algo importante: [APUNTAR] aunque yo escribí el texto en varias líneas aquí en el editor, [MOSTRAR RESULTADO] en el navegador sale todo junto en una sola línea.

Eso es porque **HTML ignora los espacios y saltos de línea**. Solo lee la etiqueta `<p>` y ya. Más adelante con CSS haremos que el texto tenga más espacio si queremos.

Regla de oro: cada bloque de texto importante va en su propio párrafo `<p>`."

**MOSTRAR EN VIVO:**
- Cómo se ve el párrafo en el navegador
- Explicar que no importan los espacios en blanco

---

## 3️⃣ LISTAS (3:30 - 5:30)

### DEMOSTRACIÓN A: LISTA SIN ORDEN

**MOSTRAR EN PANTALLA:**
- Agregar código:

```html
<h2>Lenguajes que Domino</h2>
<ul>
  <li>HTML - Estructura</li>
  <li>CSS - Diseño</li>
  <li>JavaScript - Interactividad</li>
</ul>
```

**QUÉ DECIR:**

"Las listas son perfectas para **agrupar elementos relacionados**.

Hay dos tipos:
- **Lista sin orden (`<ul>`)**: Usa viñetas. Se llama 'unordered list'. Úsala cuando el orden no importa.
- **Lista ordenada (`<ol>`)**: Usa números. Se llama 'ordered list'. Úsala cuando el orden SÍ importa.

Cada elemento de la lista va dentro de un `<li>` (list item).

[MOSTRAR EN NAVEGADOR] Mira cómo aparece con viñetas automáticamente. No tuvimos que escribirlas, HTML lo hizo solo."

### DEMOSTRACIÓN B: LISTA ORDENADA

**MOSTRAR EN PANTALLA:**
- Agregar código:

```html
<h2>Pasos para Crear una Página Web</h2>
<ol>
  <li>Aprende HTML</li>
  <li>Domina CSS</li>
  <li>Entiende JavaScript</li>
</ol>
```

**QUÉ DECIR:**

"Ahora esta es una lista **ordenada**, porque el orden sí importa. Estamos diciendo:
'Primero aprende HTML, luego CSS, luego JavaScript.'

[MOSTRAR EN NAVEGADOR] Automáticamente aparece con números del 1 al 3. Genial, ¿verdad?

Consejo: Si cambias el orden en tu código, los números se actualizan solos. No tienes que reescribirlos."

---

## 4️⃣ IMÁGENES (5:30 - 7:00)

### DEMOSTRACIÓN EN CODEPEN

**MOSTRAR EN PANTALLA:**
- Agregar código:

```html
<h2>Mi Foto de Perfil</h2>
<img 
  src="https://via.placeholder.com/300?text=Mi+Foto" 
  alt="Foto de perfil de un desarrollador"
/>
```

**QUÉ DECIR:**

"Ahora toca las imágenes. La etiqueta es `<img>` y es **diferente a las otras** porque NO tiene etiqueta de cierre. Solo tiene una barra diagonal al final.

La etiqueta `<img>` tiene dos atributos importantes:

1. **`src`** = la dirección donde está la imagen. Puede ser:
   - Una URL de Internet (como lo hice aquí)
   - Un archivo de tu computadora
   
2. **`alt`** = texto alternativo. Si la imagen no carga, esto aparece. Además, es muy importante para personas con visión limitada.

[APUNTAR] Mira que el `alt` debe describir BIEN qué hay en la imagen. No solo escribas 'foto'. Sé específico.

[MOSTRAR EN NAVEGADOR] Aquí vemos la imagen. Es de un servicio que genera imágenes de relleno para practicar.

Opcionalmente, puedes agregar `width` y `height` para cambiar el tamaño:

```html
<img 
  src="..." 
  alt="..." 
  width="250" 
  height="250"
/>
```

Eso dice: 'Muestra esta imagen a 250 píxeles de ancho y 250 de alto'."

---

## 5️⃣ ENLACES (7:00 - 8:30)

### DEMOSTRACIÓN EN CODEPEN

**MOSTRAR EN PANTALLA:**
- Agregar código:

```html
<h2>Sígueme en Línea</h2>
<p>
  Mira mis proyectos en GitHub:
  <a href="https://github.com" target="_blank">Mi perfil en GitHub</a>
</p>

<ul>
  <li>
    <a href="https://www.linkedin.com" target="_blank">LinkedIn</a>
  </li>
  <li>
    <a href="https://www.twitter.com" target="_blank">Twitter</a>
  </li>
</ul>
```

**QUÉ DECIR:**

"Los enlaces se crean con `<a>` (de 'anchor', ancla). Conectan tu página con otros sitios.

Tiene principalmente dos atributos:

1. **`href`** = la dirección web a donde va el enlace. Siempre empieza con `http://` o `https://`

2. **`target="_blank"`** = esto hace que el enlace abra en una **nueva pestaña**, en lugar de reemplazar la página actual. Es muy útil cuando no quieres que el usuario se vaya de tu sitio.

[MOSTRAR EN NAVEGADOR] Ves que el texto del enlace aparece en azul y subrayado. Eso es lo normal en un navegador.

[HACER CLIC EN EL ENLACE] Si hago clic... [PAUSA] se abre en una nueva pestaña. Perfecto, ¿verdad?

Bonus: Puedes agregar un atributo `title` para que aparezca un mensaje cuando pasas el cursor:

```html
<a href="https://github.com" target="_blank" title="Visita GitHub">GitHub</a>
```

Cuando pasas el cursor lentamente encima, aparece el texto del `title`."

---

## 6️⃣ JUNTANDO TODO (8:30 - 10:00)

### MOSTRAR EJEMPLO COMPLETO

**MOSTRAR EN PANTALLA:**
- Mostrar el archivo `completed-examples/lesson3.html` completo
- O recorrer un portafolio similar en CodePen

**QUÉ DECIR:**

"Ahora que ya conoces todos los elementos, vamos a juntarlos en una página completa.

[RECORRER EL CÓDIGO mientras hablas]

Mira la estructura:
- Un título principal con `<h1>`
- Párrafos describiendo al desarrollador
- Listas de habilidades y pasos
- Una imagen del perfil
- Enlaces a redes sociales
- Más listas de proyectos con enlaces

[MOSTRAR EN NAVEGADOR] Y así se ve cuando se renderiza. Parece una página real, ¿verdad?

Lo importante es que **cada elemento tiene su propósito**:
- Los títulos organizan
- Los párrafos explican
- Las listas agrupan información relacionada
- Las imágenes comunican visualmente
- Los enlaces conectan

Cuando combines todo esto, logras crear una **página informativa y bien estructurada**."

---

## 7️⃣ ERRORES COMUNES (10:00 - 10:45)

**MOSTRAR EN PANTALLA:**
- Pantalla con lista de errores
- Ejemplos de código incorrecto vs. correcto

**QUÉ DECIR:**

"Antes de terminar, vamos a ver los **errores más comunes** que cometen los principiantes:

❌ **Error 1:** Usar `<h1>` varias veces en la misma página
✅ **Correcto:** Solo un `<h1>` por página. Usa `<h2>` y `<h3>` para lo demás.

❌ **Error 2:** Olvidar el atributo `alt` en las imágenes
✅ **Correcto:** Siempre escribe `alt="descripción clara"`

❌ **Error 3:** URLs rotas en los enlaces
✅ **Correcto:** Prueba siempre que tus enlaces funcionen antes de entregar

❌ **Error 4:** No abrir enlaces externos en nueva pestaña
✅ **Correcto:** Usa `target="_blank"` para no perder el visitante

❌ **Error 5:** Listas desordenadas cuando necesitas orden
✅ **Correcto:** Piensa si el orden importa: sí = `<ol>`, no = `<ul>`"

---

## 8️⃣ DESAFÍO / LLAMADA A LA ACCIÓN (10:45 - 11:00)

**MOSTRAR EN PANTALLA:**
- Diapositiva de desafío
- Enlace a CodePen con starter file

**QUÉ DECIR:**

"Ahora te toca a ti. **Tu desafío es:**

1. Abre el editor en línea (enlace en la descripción)
2. Crea tu propia página de portafolio
3. Incluye:
   - Tu nombre en `<h1>`
   - Un párrafo sobre ti
   - Tus 3 habilidades en una lista `<ul>`
   - Una foto tuya (o placeholder)
   - Enlaces a 2 redes sociales en una lista `<ul>`

[PAUSA]

¿Necesitas ayuda? En la descripción del video encontrarás:
- El código de ejemplo completo
- Un editor precargado para practicar
- Los apuntes de la lección

¡Comparte tu resultado en los comentarios! Me encantaría ver tu portafolio. 

En la próxima lección aprenderemos CSS para hacer que todo esto se vea **hermoso**. Colores, tipografía, espacios... 

¡Nos vemos! 👋"

---

## 🎥 NOTAS TÉCNICAS PARA GRABAR

### Lo que necesitas
- Screen recorder (OBS, ScreenFlow, etc.)
- Micrófono decente
- Editor en línea: **CodePen** (https://codepen.io/)
- Tema oscuro o claro consistente

### Tips de grabación
- Habla claro y pausado (estudiantes de 12-17 años)
- Haz zoom en el código (24pt font mínimo)
- Pausa entre secciones
- Sintetiza: no leas todo lo que está en pantalla
- Muestra el resultado en el navegador después de cada cambio
- Sé entusiasta pero natural

### Estructura del código en CodePen
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Mi Portafolio</title>
</head>
<body>
    <!-- TODO: Completar según lo que enseñas -->
</body>
</html>
```

### Duración estimada por sección
- Intro: 30s
- Títulos: 2m
- Párrafos: 1m
- Listas: 2m
- Imágenes: 1.5m
- Enlaces: 1.5m
- Ejemplo completo: 1.5m
- Errores: 45s
- Desafío: 15s

**TOTAL: ~12 minutos**

