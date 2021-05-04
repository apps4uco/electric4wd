# Lenguaje de Programación


## C / C++

C fue inventado en 1970 y es uno de los lenguajes más comunes en sistemas operativos, y actualmente la mayoria de firmware para sistemas embebidas esta escrito en C.

<!-- muchos otros lenguajes de programación estan implementados en C. -->

Más del 70% de los parches para Windows son por errores de seguridad en la memoria.
[Fuente](https://vandal.elespanol.com/noticia/w3123/mas-del-70-de-los-parches-para-windows-son-por-errores-de-seguridad-en-la-memoria)

Aproximadamente el 70% de todos los errores de seguridad graves en la base del código de Chrome son errores de administración de memoria, según dijeron los ingenieros de Google esta semana.
[Fuente](https://unaaldia.hispasec.com/2020/05/chrome-alrededor-del-70-de-los-errores-graves-son-problemas-de-seguridad-relacionados-con-la-administracion-de-la-memoria.html)

Problemas de memoria incluyen:


* Null Pointer
* Wild Pointer
* Dangling Pointer
* Double Free
* Use after free
* Using Uninitialized Memory
* Buffer Overflow
* Memory Leaks
* Data Races

## Rust

Un lenguaje que empodera a todos
para construir software fiable y eficiente. 

fast, reliable, productive: pick thre

### ¿Por qué Rust?

Rust fue diseñado para evitar los problemas de memoria que C y C++ tienen, mencionados anteriormente, y al mismo tiempo tener el mismo rendimiento.


<https://www.rust-lang.org/es/>

<https://www.rust-lang.org/es/what/embedded>


### Rendimiento

Rust es rápido como el rayo y eficiente con la memoria: sin runtime ni colector de basura, puede sustentar servicios de rendimiento crítico, ejecutarse en dispositivos embebidos, e integrarse con otros lenguajes fácilmente.


### Fiabilidad

El rico sistema de tipos de Rust y su modelo de propiedad (ownership) garantizan seguridad de memoria y seguridad de hilos, y te permiten eliminar muchas clases de bugs en tiempo de compilación.


### Productividad

Rust tiene una documentación genial, un compilador accesible con mensajes de error útiles, y herramientas de primera: gestor de paquetes y de proyecto integrado, soporte avanzado multi-editor con autocompletado e inspecciones de tipos, auto-formateador, etc.

## Rust en Sistemas Embebidas

Aunque todavia no es común encontrar firmware escrito en Rust, tiene ventajas de seguridad y facilidad de desarrollo.

### Análisis estático potente

Aplica la configuración de pins y periféricos en tiempo de compilación. Garantiza que los recursos no son usados accidentalmente por otras partes de tu aplicación. 


### Memoria flexible

La gestión dinámica de memoria es opcional. Usa un gestor de memoria global y estructuras de datos dinámicas. O prescinde del heap y asigna espacio para todo estáticamente. 


### Concurrencia sin miedo

Rust previene el estado compartido accidentalmente entre hilos. Usa concurrencia con el enfoque que desees, y siempre tendrás las fuertes garantías de Rust. 

### Interoperabilidad

Integra Rust en tu código C ya existente o aprovecha uno de los SDKs disponibles para escribir una aplicación en Rust. 

### Portabilidad

Escribe una biblioteca o driver una sola vez, y úsala en múltiples sistemas, desde pequeños microcontroladores hasta potentes placas integradas. 

### Impulsado por la comunidad

Como parte del proyecto open source Rust, el soporte para sistemas embebidos está respaldado por una comunidad open source ejemplar, con apoyo de socios comerciales. 



> Rust nos permite desplegar software más correcto y más rápidamente de lo que imaginábamos. Gracias a Rust podemos dar la seguridad de memoria por sentada, mientras que otros beneficios de un lenguaje de coste cero con un sistema de tipos sofisticado nos ayudan a desarrollar software mantenible. Rust hace felices a nuestros clientes, así como a nuestros ingenieros.


Marc Brinkmann, CEO, 49nord


### Empresas utilizando Rust en Produción

Mozilla Firefox 

<https://www.rust-lang.org/production/users>
