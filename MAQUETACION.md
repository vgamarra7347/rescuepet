# Maquetación HTML5 Semántica - RescuePet

## 1. Descripción de la actividad
Se desarrolló la estructura base de la interfaz de usuario del sistema **RescuePet** utilizando exclusivamente etiquetas semánticas de HTML5, sin aplicar hojas de estilo (CSS), priorizando la accesibilidad, el orden lógico del contenido y la estructura estándar web.

## 2. Estructura de vistas implementadas
* **`index.html`:** Página principal que presenta el sistema, su propósito y las últimas novedades o jornadas de adopción mediante etiquetas `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` y `<footer>`.
* **`reportar.html`:** Vista que contiene un formulario interactivo con validaciones nativas de HTML5 (`required`, tipos de entrada específicos como `tel` y selecciones) para registrar animales en situación de calle.
* **`rescates.html`:** Vista de consulta que organiza el historial y estado actual de los casos gestionados mediante tablas semánticas (`<table>`, `<thead>`, `<tbody>`).

## 3. Control de versiones (Gitflow)
El desarrollo se realizó de forma aislada en la rama `feature/maquetacion-html` y posteriormente fue integrado a la rama `develop` para mantener la trazabilidad del proyecto.