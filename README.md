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
Además, el mensaje de error aparece con una transición suave y desaparece después de 0.5 segundos.

---

## 🖥️ Cómo Usar el Proyecto

1. **Clona el repositorio** :

```bash
git clone https://github.com/Seb-RM/Javascript_Html_Css-Shake-on-Invalid-Input.git`
```
2. **Abre el archivo** **`index.html`** en tu navegador.

3. **Prueba el formulario** :

- Deja el campo de texto vacío y haz clic en "Submit" para ver la animación de "shake" y el mensaje de error.

- Ingresa algún texto y haz clic en "Submit" para ver la alerta de entrada válida.

---

## 📝 Código Destacado

### HTML
El formulario tiene un campo de texto y un botón de envío. También incluye un mensaje de error oculto.

```html
<form action="" id="myForm">
    <div id="errorMessage" class="error-message">Invalid Input</div>
    <input type="text" id="inputField" placeholder="Enter your text" required>
    <button onclick="validateInput()" type="submit">Submit</button>
</form>
```

### CSS
Los estilos definen la apariencia del formulario y la animación de "shake".

```css
.shake {
    animation: shake 0.5s ease-in-out;
}
```
### JavaScript
La función **`validateInput()`** valida la entrada y controla la animación y el mensaje de error.

```javascript

function validateInput() {
    let inputField = document.getElementById("inputField");
    let inputValue = inputField.value.trim();
    const errorMessage = document.getElementById("errorMessage");

    if (inputValue === "") {
        inputField.classList.add("shake");
        errorMessage.style.visibility = "visible";

        setTimeout(() => {
            inputField.classList.remove("shake");
            errorMessage.style.visibility = "hidden";
        }, 500);
    } else {
        alert("Valid Inputs");
    }
}
```

---

## 🧠 Conceptos Trabajados
* Manipulación del DOM con JavaScript.

+ Uso de eventos y funciones en JavaScript.

- Animaciones CSS con @keyframes.

- Diseño responsive con unidades relativas como em y min().



