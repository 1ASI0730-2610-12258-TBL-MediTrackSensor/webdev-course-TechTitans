# Lección 3: Construyendo Contenido Web con HTML

**Objetivo:**  
Dominar las etiquetas HTML esenciales como **títulos, textos, listas, fotos y hipervínculos** para armar una página web estructurada, clara y visualmente organizada.

---

## Introducción

Ahora que ya conoces cómo se arma el esqueleto de una página HTML, es momento de aprender a **llenarla de contenido**. HTML te proporciona diferentes etiquetas que te permiten mostrar información de múltiples formas: con títulos de distintos tamaños, bloques de texto, listados, galería de imágenes y conexiones a otros sitios.

> 💡 Imagina que estás construyendo un edificio: ya tienes las vigas y la estructura básica, ahora vamos a colocar las paredes, puertas, ventanas y decoración.

---

## Títulos y Subtítulos (`<h1>` a `<h6>`)

Los títulos sirven para **jerarquizar la información** en tu página. Van desde `<h1>` (el más importante) hasta `<h6>` (el menos importante).

```html
<h1>Mi Portafolio de Proyectos Web</h1>
<h2>Proyectos Personales</h2>
<h3>Proyecto #1: Sistema de Notas</h3>
```

| Etiqueta        | Uso                                                                        |
| :-------------- | :------------------------------------------------------------------------- |
| `<h1>`          | Título principal de la página. Usarlo una sola vez por página.             |
| `<h2>`          | Títulos de secciones principales.                                          |
| `<h3>` a `<h6>` | Subniveles para subsecciones y detalles adicionales.                       |

**Consejo:** Los buscadores como Google leen los títulos para entender qué trata tu página, así que úsalos con cuidado.

---

## Párrafos (`<p>`)

Un párrafo es un bloque de texto. HTML los utiliza para agrupar información y hacer que sea legible.

```html
<p>
  Soy un desarrollador web apasionado por crear experiencias digitales innovadoras.
  Llevo 2 años aprendiendo HTML, CSS y JavaScript.
</p>
```

**Nota:** HTML ignora los espacios y saltos de línea que escribas. El párrafo siempre se mostrará en una línea hasta que agregues CSS para modificarlo.

---

## Listas: Organizando Información (`<ul>`, `<ol>`, `<li>`)

Las listas permiten mostrar grupos de elementos de forma clara y ordenada.

### Lista sin Orden (`<ul>`)

Usa viñetas (puntos) cuando el orden no importa.

```html
<ul>
  <li>HTML - Estructura del sitio</li>
  <li>CSS - Diseño y colores</li>
  <li>JavaScript - Interactividad</li>
</ul>
```

Se vería así en el navegador:
- HTML - Estructura del sitio
- CSS - Diseño y colores
- JavaScript - Interactividad

### Lista Ordenada (`<ol>`)

Usa números cuando el orden tiene importancia (como en pasos o tutoriales).

```html
<ol>
  <li>Escribe tu primer código HTML</li>
  <li>Añade estilos con CSS</li>
  <li>Haz tu página interactiva con JavaScript</li>
</ol>
```

Se vería así:
1. Escribe tu primer código HTML
2. Añade estilos con CSS
3. Haz tu página interactiva con JavaScript

---

## Imágenes (`<img>`)

La etiqueta `<img>` inserta fotos, gráficos o cualquier imagen en tu página.

```html
<img src="https://via.placeholder.com/300" alt="Foto de perfil del desarrollador" />
```

| Atributo           | Descripción                                                                  |
| :----------------- | :--------------------------------------------------------------------------- |
| `src`              | La dirección o ubicación de la imagen (URL o ruta local).                    |
| `alt`              | Texto descriptivo (importante para personas con visión limitada).            |
| `width` / `height` | Ancho y alto de la imagen en píxeles (opcional).                             |

**Ejemplo con tamaño:**
```html
<img src="proyecto.png" alt="Captura de pantalla del proyecto" width="400" height="300" />
```

**Consejo:** Usa el atributo `alt` siempre. Ayuda con la accesibilidad y si la imagen no carga, el usuario sabrá qué debería haber allí.

---

## Enlaces (`<a>`)

Los enlaces (o hipervínculos) conectan tu página con otros sitios o recursos en la web.

```html
<a href="https://www.github.com" target="_blank">Mi perfil en GitHub</a>
```

| Atributo          | Descripción                                                 |
| :---------------- | :---------------------------------------------------------- |
| `href`            | La dirección web hacia donde apunta el enlace.              |
| `target="_blank"` | Abre el enlace en una **nueva pestaña** del navegador.       |
| `title`           | Texto que aparece cuando pasas el cursor sobre el enlace.   |

**Ejemplo completo:**
```html
<a href="https://www.linkedin.com/in/miusuario" 
   target="_blank" 
   title="Visita mi perfil de LinkedIn">
  Conéctate conmigo en LinkedIn
</a>
```

---

## Juntándolo Todo: Un Ejemplo Completo

Veamos cómo combinar todas estas etiquetas para crear una página de presentación:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Mi Portafolio - Juan Developer</title>
</head>
<body>
    <h1>Juan García - Desarrollador Web</h1>
    
    <img src="mi-foto.jpg" alt="Foto de perfil" width="150" height="150" />
    
    <h2>Sobre mí</h2>
    <p>
        Soy estudiante de ingeniería de software con pasión por crear 
        sitios web increíbles. Especializado en HTML, CSS y JavaScript.
    </p>
    
    <h2>Habilidades</h2>
    <ul>
        <li>Diseño responsivo</li>
        <li>HTML5 semántico</li>
        <li>CSS3 moderno</li>
    </ul>
    
    <h2>Mis Proyectos</h2>
    <ol>
        <li>
            <a href="https://ejemplo1.com" target="_blank">Blog Personal</a>
            - Mi primer proyecto con HTML y CSS
        </li>
        <li>
            <a href="https://ejemplo2.com" target="_blank">Tienda Online</a>
            - Proyecto más complejo con carrito
        </li>
    </ol>
    
    <h2>Contacto</h2>
    <p>
        Puedes encontrarme en:
        <a href="https://www.twitter.com" target="_blank" title="Mi Twitter">Twitter</a> |
        <a href="https://www.instagram.com" target="_blank" title="Mi Instagram">Instagram</a>
    </p>
</body>
</html>
```

---

## Consejos Finales

✅ **Usa títulos para organizar** - Cada sección debe tener un título  
✅ **Mantén los párrafos cortos** - Facilita la lectura en celulares  
✅ **Agrega descripciones en tus imágenes** - No olvides el atributo `alt`  
✅ **Prueba tus enlaces** - Asegúrate de que todas las URLs sean correctas  
✅ **Abre enlaces externos en nueva pestaña** - Usa `target="_blank"`

---

## Errores Comunes a Evitar

❌ **No usar `<h1>` varias veces** - Solo debe haber un `<h1>` por página  
❌ **Dejar imágenes sin `alt`** - Es importante para la accesibilidad  
❌ **Saltar niveles de títulos** - Usa `<h2>` después de `<h1>`, no `<h4>`  
❌ **URLs rotas en enlaces** - Siempre verifica que los enlaces funcionen  

---

## Próxima Lección

¡Perfecto! Ya sabes cómo estructurar contenido. En la siguiente lección aprenderás a **hacer que se vea bonito** con CSS: colores, tipografía, espacios y mucho más. 🎨
