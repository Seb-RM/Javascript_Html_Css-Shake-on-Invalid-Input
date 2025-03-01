# 🎯 Formulario con Animación de Validación en JavaScript

¡Bienvenido al repositorio del proyecto **Formulario con Animación de Validación en JavaScript**! Este proyecto fue desarrollado con el objetivo de practicar y reforzar conceptos básicos de JavaScript, CSS y HTML. A continuación, te explico en detalle cómo funciona y cómo puedes utilizarlo.

---

## 🚀 Descripción del Proyecto

Este proyecto consiste en un formulario simple que valida la entrada del usuario. Si el campo de texto está vacío al enviar el formulario, se activa una animación de "shake" (sacudida) y se muestra un mensaje de error. Si la entrada es válida, se muestra una alerta indicando que los datos son correctos.

### Características principales:
- **Validación de entrada**: Verifica si el campo de texto está vacío.
- **Animación de "shake"**: Una animación CSS que sacude el campo de texto cuando la entrada es inválida.
- **Mensaje de error**: Un mensaje de error que aparece temporalmente cuando la validación falla.
- **Diseño responsive**: El formulario está diseñado para verse bien en cualquier dispositivo.

---

## 🛠️ Tecnologías Utilizadas

- **HTML**: Estructura básica del formulario.
- **CSS**: Estilos y animaciones para el formulario y la validación.
- **JavaScript**: Lógica de validación y manipulación del DOM.

---

## 📂 Estructura del Proyecto

El proyecto consta de tres archivos principales:

1. **`index.html`**: Contiene la estructura del formulario.
2. **`style.css`**: Define los estilos y la animación de "shake".
3. **`script.js`**: Implementa la lógica de validación del formulario.

---

## 🎨 Diseño y Animación

El diseño del formulario es minimalista y moderno, con un enfoque en la usabilidad. La animación de "shake" se activa cuando el usuario intenta enviar el formulario sin ingresar datos. Esta animación se logra mediante keyframes en CSS:

```css
@keyframes shake {
    0% { transform: translateX(0); }
    25% { transform: translateX(-5px); }
    50% { transform: translateX(5px); }
    75% { transform: translateX(-5px); }
    100% { transform: translateX(0); }
}
````
