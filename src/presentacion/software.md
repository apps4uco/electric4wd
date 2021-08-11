# Software

Los software mencionados son en varios fases de desarrollo. Y son más pruebas de concepto y exploraciones que productos terminados.

# car_bus

Software para probar simulación de comunicación via un bus de datos en Rust

El objetivo es simular la red CAN del vehiculo. Los ECU son simulados corriendo en hilos diferentes, enviando mensaje via un bus de datos.

Prototipo sencillo

# car_cali

Sofware para probar el uso de Unidades de Medida en UOM en un aplicativo.

Para evitar problemas como el Mars Climate Orbiter
|
# car-can

Software para convertir trazas CAN en formato CSV en imagenes png a blanco y negro y a color

# car_carla

Software para cargar el conjunto de datos Carla y Audi en formato json a Parquet para procesar más rapido.

Carla es un simulador para desarrollar vehiculos autonomos.

# car-diagnostics

Software para graficar los datos del vehiculo en "tiempo real" y offline.


#car_diagrams

Software para mostrar diagramas de simulación del vehiculo en formato svg

# car_imu

Software para demostrar el funcionamiento de librerias de medición inercial escritos en Rust. Attitude and Heading Reference System (AHRS).

Se implementa los algoritmos de

* Madgwick <https://github.com/xioTechnologies/Fusion>
S. Madgwick, An Efficient Orientation Filter for Inertial and Inertial/Magnetic Sensor Arrays; Technical Report; Report x-io and University of Bristol: Bristol, UK, 30 April 2010.
* Mahony - S. Mahony, T. Hamel, J.-M. Pflimlin, Nonlinear complementary filters on the special orthogonal group.  Auto. Control IEEE Transac., 53, 1203-1218, 2008
* Heikki Hyyti and Arto Visala, "A DCM Based Attitude Estimation Algorithm for Low-Cost MEMS IMUs," International Journal of Navigation and Observation, vol. 2015, Article ID 503814, 18 pages, 2015. <https://www.hindawi.com/journals/ijno/2015/503814/>
* Error State Kalman Filter

Comparison of Attitude and Heading Reference Systems using Foot Mounted MIMU Sensor Data: Basic, Madgwick and Mahony
<http://www.cs.ndsu.nodak.edu/~siludwig/Publish/papers/SPIE20181.pdf>

Para investigar: Los resultados de las librerias no son iguales.


# car_lvgl

Principios de un prototipo para mostrar la interfaz del vehiculo con la libreria LVGL (apto para microcontroladores)

Se encontró que la implementación de la libreria en Rust esta incompleta y no soporta imagenes entre otras cosas.

# car_model_glider

Modelo de vehiculo sencillo "Glider" combinado con el EPA Drivecycle Prueba, y un bucle PID.

El objetivo es poder simular la respuesta del carro basado en las pruebas EPA.

Pasos futuros: modelar el motor y la bateria y determinar el estado de carga y corrientes picos.

# car_physics

Actualmente es un demo del motor de fisica rapier, para modelar masas, y uniones articuladas.

El objetivo es utilizar el motor de fisica rapier para modelar el movimiento del carro y poder medir y visualizar los resultados.

# car_physx

nvim /opt/git/PhysX/physx/snippets/snippetvehiclecontactmod/SnippetVehicleContactModRender.cpp

nvim /opt/git/PhysX/physx/snippets/snippetvehicle4w/SnippetVehicle4W.cpp

cd /opt/git/PhysX/physx/compiler/linux-release/sdk_snippets_bin

make

cd /opt/git/PhysX/physx/bin/linux.clang/release

./SnippetVehicleContactMod_64

Project es el comienzo para utilizar Nvidia Physx para simular un vehiculo y visualisación en 3d utilizando Rust.

# car-webui

Software para mostrar datos del carro en un tablero web actualizado en tiempo real, desde un servidor web, utilizando svg.

# infotainment

Un demo de un LCD/LED tablero. Apto para utilizar desde un microcontrollador (en Rust).

# rtos

Implementación de unos componentes del carro utilizando FreeRTOS.

La simulación corre sobre Linux, pero la propuesta es utilizar el mismo sistema sobre microcontroladores.
