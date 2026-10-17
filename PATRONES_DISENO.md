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

### 3.2. Singleton

**¿Qué es?**

Singleton es un patrón de diseño creacional que busca garantizar que una clase tenga una única instancia y proporcionar un punto de acceso a ella cuando sea necesario.

**Aplicación en RescuePet**

En el diseño de RescuePet, se propone aplicar este patrón a la clase `SistemaRescate`, con el objetivo de centralizar el acceso a las funciones principales del sistema. De esta manera, los componentes que necesiten utilizar los servicios generales podrán acceder a una única instancia de esta clase.

**¿Por qué se eligió?**

Se propone Singleton para mantener organizado el acceso a las operaciones principales de RescuePet y evitar la creación de varias instancias de la clase encargada de coordinar el sistema.

**¿Qué problema resuelve?**

Este patrón ayuda a evitar que existan múltiples instancias de `SistemaRescate` cuando se requiere una única instancia compartida. Su aplicación debe definirse en el diseño y comprobarse si posteriormente se implementa el sistema mediante código.

### 3.3. Observer

**¿Qué es?**

Observer es un patrón de diseño de comportamiento que permite notificar automáticamente a los componentes interesados cuando ocurre un cambio en un objeto. De esta forma, los componentes pueden mantenerse informados sin depender directamente unos de otros.

**Aplicación en RescuePet**

En RescuePet, se propone utilizar Observer para notificar los cambios importantes en los casos de rescate. Por ejemplo, cuando el estado de un caso cambia de registrado a en proceso o resuelto, el sistema podría generar una notificación para los usuarios o responsables relacionados con ese caso.

**¿Por qué se eligió?**

Se eligió este patrón porque el sistema necesita mantener informados a los usuarios y responsables sobre las novedades de los rescates. Su utilización ayudaría a organizar las notificaciones y reducir la dependencia directa entre las clases involucradas.

**¿Qué problema resuelve?**

Observer ayuda a evitar que cada componente tenga que consultar constantemente si ocurrió algún cambio. En su lugar, los componentes interesados pueden recibir una notificación cuando se produce un evento relevante, lo que mejora la organización y la comunicación dentro del sistema.

### 3.4. MVC (Modelo-Vista-Controlador)

**¿Qué es?**

MVC es un patrón arquitectónico que divide una aplicación en tres partes: el Modelo, que gestiona los datos; la Vista, que presenta la información al usuario; y el Controlador, que recibe las acciones del usuario y coordina las operaciones correspondientes.

**Aplicación en RescuePet**

En el diseño de RescuePet, MVC puede utilizarse para separar la información de los animales, los casos de rescate y las adopciones de las pantallas que utilizarán los usuarios. El Controlador se encargaría de coordinar las acciones, como registrar un rescate, consultar un animal o gestionar una adopción.

**¿Por qué se eligió?**

Se propone este patrón porque RescuePet necesita organizar diferentes procesos y permitir que los usuarios interactúen con el sistema de manera clara. La separación de responsabilidades facilita la comprensión del diseño y los posibles cambios futuros.

**¿Qué problema resuelve?**

MVC ayuda a evitar que la presentación de la información, la gestión de los datos y la lógica de las operaciones estén mezcladas en una sola parte del sistema. Esto facilita el mantenimiento y la organización de sus componentes.
