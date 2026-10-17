# Sistema de Rescate y Adopción Animal - RescuePet

## 1. Análisis del problema

### 1.1 Descripción del problema

Los refugios animales necesitan una forma organizada de registrar los casos de rescate, almacenar información sobre los animales y coordinar el trabajo de voluntarios y veterinarios. Cuando estos procesos se realizan manualmente, puede existir pérdida de información, dificultades para asignar responsables y problemas para conocer el estado de cada animal.

Por esta razón, se propone diseñar RescuePet, un sistema de gestión que permita registrar animales rescatados, clasificarlos por especie, asignar responsables y realizar un seguimiento de su proceso de recuperación y adopción.

### 1.2 Actores principales

- **Ciudadano o reportante:** informa sobre animales que necesitan ayuda y proporciona los datos del lugar donde se encuentran.
- **Voluntario:** participa en las labores de rescate, cuidado y seguimiento de los animales.
- **Veterinario:** registra evaluaciones médicas, tratamientos y avances en la recuperación.
- **Administrador del refugio:** organiza los casos, asigna responsables y supervisa el funcionamiento del sistema.

### 1.3 Requerimientos funcionales

- RF01: Registrar nuevos casos de rescate animal.
- RF02: Clasificar los animales según su especie: perro, gato o fauna silvestre.
- RF03: Registrar los datos del animal y la ubicación del rescate.
- RF04: Asignar voluntarios o veterinarios responsables.
- RF05: Actualizar el estado del caso: Rescatado, En Tratamiento, Disponible para Adopción o Adoptado.
- RF06: Consultar el historial y los detalles de cada caso.
- RF07: Generar notificaciones para informar sobre nuevos rescates y asignaciones.

### 1.4 Requerimientos no funcionales

- RNF01: **Escalabilidad.** El sistema debe permitir incorporar nuevos usuarios y casos sin tener que rediseñar toda la solución.
- RNF02: **Mantenibilidad.** El diseño debe organizar las responsabilidades en componentes independientes y fáciles de modificar.
- RNF03: **Trazabilidad.** Los cambios del proyecto deben quedar registrados mediante Git y GitHub.
- RNF04: **Seguridad.** El acceso a las funciones administrativas debe estar controlado según el tipo de usuario.
- RNF05: **Usabilidad.** La interfaz debe ser clara y facilitar el registro y la consulta de casos.

### 1.5 Objetivo del sistema

Diseñar un sistema que facilite la gestión de rescates y adopciones mediante el registro organizado de animales, la asignación de responsables, el seguimiento de los casos y el uso de patrones de diseño de software.
