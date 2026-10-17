# Patrones de Diseño del Sistema RescuePet

## 1. Introducción

Los patrones de diseño son soluciones que ayudan a organizar mejor la estructura de un sistema informático. Permiten distribuir las responsabilidades entre las clases, facilitar el mantenimiento y hacer que el sistema pueda adaptarse a futuras necesidades.

En el sistema RescuePet, que está orientado al control de rescates y adopciones de animales, se proponen diferentes patrones de diseño para mejorar la organización de sus componentes y facilitar la gestión de los procesos principales.

## 2. Patrones de diseño seleccionados

Para el diseño del sistema RescuePet se consideran los siguientes patrones:

- **Factory Method:** permite organizar la creación de objetos relacionados con los animales.
- **Singleton:** permite controlar la existencia de una única instancia de una clase cuando el sistema lo necesita.
- **Observer:** permite notificar a los componentes o usuarios interesados cuando ocurre un cambio importante.
- **MVC (Modelo-Vista-Controlador):** permite separar la información del sistema, la interfaz y la lógica que controla las operaciones.

## 3. Documentación de los patrones

En los siguientes apartados se explicará cómo se aplica cada patrón en RescuePet, por qué fue seleccionado y qué problema ayuda a resolver.

### 3.1. Factory Method

**¿Qué es?**

Factory Method es un patrón de diseño creacional que permite organizar la creación de objetos sin que todas las partes del sistema tengan que encargarse directamente de ese proceso.

**Aplicación en RescuePet**

En RescuePet, este patrón se representa mediante la clase `AnimalFactory`, que se encarga de organizar la creación de objetos de tipo `Animal`. De esta forma, el sistema mantiene separado el proceso de creación de animales de las demás responsabilidades de las clases.

**¿Por qué se eligió?**

Se seleccionó este patrón porque el sistema necesita registrar y gestionar animales rescatados. Tener una clase dedicada a su creación permite mantener el diseño más organizado y facilita la incorporación de cambios en el futuro.

**¿Qué problema resuelve?**

Factory Method ayuda a evitar que la lógica de creación de objetos se repita en diferentes partes del sistema. Esto facilita el mantenimiento y permite que las responsabilidades estén mejor distribuidas entre las clases.
