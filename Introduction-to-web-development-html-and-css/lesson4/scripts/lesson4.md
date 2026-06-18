# Lección 4: Introducción a CSS (Estilizando componentes)

**Objetivo:** Comprender cómo CSS transforma el HTML plano en un diseño atractivo visualmente. Aprenderás a usar selectores de etiquetas y de clases para modificar el color, el fondo y el espaciado interno/externo.

---

## El Superpoder de CSS

Mientras que el HTML construye los "huesos" de nuestra página web, **CSS** se encarga de la ropa, el peinado y el estilo. Pasaremos de una estructura aburrida a una tarjeta interactiva y moderna.

### Las tres maneras de añadir CSS:
1. **En línea:** Usando el atributo `style` (no recomendado para proyectos grandes).
2. **Interno:** Dentro de etiquetas `<style>` en el archivo HTML.
3. **Externo:** En un archivo `.css` independiente conectado por un `<link>`.

---

## Anatomía de una Regla CSS
Para cambiar un diseño necesitas tres cosas: un **Selector**, una **Propiedad** y un **Valor**.

```css
.clase-o-etiqueta {
  propiedad: valor;
}