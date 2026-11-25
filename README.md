# Centrar ventanas emergentes

Userscript para Violentmonkey en Firefox que intenta centrar los cuadros de diálogo que aparecen dentro de una página web. También puede ayudar cuando un diálogo queda fuera del área visible, como los pop-ups de extensiones.

## Instalación

- Instala Violentmonkey en Firefox.
- Abre su panel y selecciona **Crear un nuevo script**.
- Pega el código del archivo `centrar-ventanas-emergentes.user.js`.
- Guarda el script y recarga la página donde aparece el cuadro de diálogo.

## Funcionamiento

El script busca diálogos mediante atributos y selectores habituales, como `role="dialog"`, `aria-modal="true"` y `dialog[open]`. Fuerza su posición al centro de la ventana y vuelve a aplicar los estilos cuando la página agrega o modifica elementos.

## Alcance y límites

Actúa sobre elementos dentro de las páginas web. No puede controlar los paneles que Firefox dibuja en su propia interfaz, como los que se abren desde un botón de la barra de herramientas.

Tampoco puede garantizar el centrado de elementos dentro de iframes de otro origen o de raíces Shadow DOM cerradas. En algunas páginas, forzar la posición puede alterar el diseño del diálogo.

## Datos

- Autor: Baalgarthem
- Versión: 1.0.0
- Gestor de usuarioscripts: Violentmonkey
- Navegador objetivo: Firefox
