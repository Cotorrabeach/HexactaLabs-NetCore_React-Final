# HexactaLabs-.NETCore_React

Hexacta 2020

**Bienvenido a los Hexacta Labs**

Agenda:
* _Initial_: Presentación de la aplicación básica, pasos para correrla localmente y planteo de la primer actividad: Backend con .NetCore.
* _Level 1_: Se nivelará presentando una aplicación con las actividades de la etapa inicial completas. Planteo de la segunda actividad: Frontend con ReactJS.
* _Level 2_: Se presenta la aplicación con las actividades anteriores completas. Planteo de la tercera actividad: FullStack development.
* __Final: Se presenta la aplicación completa. Planteo de la actividad final.__

## [Readme General](https://github.com/lnapoliHX/HexactaLabs-NetCore_React-Initial/blob/master/README.md)

## [Documentación](https://github.com/lnapoliHX/HexactaLabs-NetCore_React-Initial/blob/master/Docs/index.md)


## ¿Qué aprendimos?
*Initial: creación de un backend para un frontend existente.*  

Aprendimos conceptos de DTO, Inyección de Dependencias, Mapping entre Dto y Entity, buenas prácticas de documentación con Swagger, N-Layer architecture ó "slices horizontales". 

*Level 1: creación de un frontend para un backend existente.* 

Aprendimos componetizar un frontend con React, mantener un estado general con Redux, realizar validaciones en frontend con Redux-Form, routing, separation of concerns, trabajar con una arquitectura existente en este caso utilizamos "duck typing" y "slices verticales" o "separación en módulos. 

*Level 2: end-to-end, creación desde el frontend hasta la base de datos.*

Aplicar aquí todo el conocimiento para desarrollar frontend y backend.

Sobre [Vertical/Horizontal Slices](https://jimmybogard.com/vertical-slice-architecture/)  
Sobre [Separation of Concerns](https://en.wikipedia.org/wiki/Separation_of_concerns)  

# Actividad Final
Para el trabajo final disponemos de una versión de la Stock Web completa con el manejo CRUD de todas las entidades tanto de backend como de frontend.
Este ejercicio final propone el modelado e implementación de un carrito de compra, para el que se necesita:

* Agregar en la tabla de productos la opción de _agregar producto al carrito_ con un botón y un campo de cantidad.
* Los productos cuyo stock sea 0 no deben habilitar la opción para agregar al carrito.
* Una nueva sección en el sitio debe mostrar el detalle del carrito con una tabla donde se muestren los productos seleccionados, la cantidad y el precio unitario. En la sección inferior de la pantalla se debe mostrar el precio total a pagar y un botón de checkout.
* Al presionar el botón para realizar la compra, el sistema debe chequear el stock disponible en ese momento para cada producto seleccionado. Si hay stock para un producto en particular, se debe actualizar la cantidad de existencias restando la cantidad que el usuario seleccionó.
* Aquellos productos que no tienen suficiente stock al momento de realizar la compra no deben ser actualizados.
* Al finalizar la compra el sistema debe mostrar al usuario una nueva página donde se muestre el detalle de qué productos pudieron reservarse y el precio total de la compra. Tener en cuenta que este precio puede ser distinto al precio que se mostró en la página anterior por falta de stock.

## Tips:
- El carrito:
    - no es necesario mantenerlo en backend
    - al recargar la página (al presionar F5) el carrito se siga manteniendo.
    - realizar validaciones en backend para comprobar la existencia del producto (puede ocurrir que haya tenido stock en el momento que lo agregó al carrito, pero no al momento de finalizar la compra)
- Al finalizar la compra, debería almacenarse la misma en backend.  
