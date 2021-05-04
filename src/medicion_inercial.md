


La seguridad en el sistema es sumamente importante.

Existe un modo de fallo que puede ocurrir cuando el vehiculo esta en una curva.

Es posible que las llantas atras pueden deslizar

a) por exceso de velocidad
b) por exceso de aceleración
c) por frenado

En cualquier caso se considera que lo más seguro es que el sistema 4x4 se debe desconectar.

Se deja como proyecto de investigación la posibilidad de corrección del deslizo activo por parte de las llantas traseras.

Para detectar el caso de la perdida de tracción es necesario sensar la atitude, posicion, velocidad y aceleración del carro.

# 




# Unidad de medición inercial

Se propone utilizar 2 sensores IMU, uno en la parte adelante del vehiculo y uno trasero.



# Filtro Kalman

Para (Sensor Fusion)



# Filtro Kalman Extendido

Integración de GPS requiere Extendido... 

An algorithm for fusing low-cost triaxial MEMS gyroscope and accelerometer measurements.
https://crates.io/crates/dcmimu

A DCM Based Attitude Estimation Algorithm for Low-Cost MEMS IMUs

> To be able to use these low-cost MEMS sensors with precision in all situations, a novel attitude estimation algorithm is proposed for fusing triaxial gyroscope and accelerometer measurements. An extended Kalman filter is implemented to estimate attitude in direction cosine matrix (DCM) formation and to calibrate gyroscope biases online.



 Navigation filter based on an Error State Kalman Filter (ESKF) 
https://crates.io/crates/eskf


An Error State Kalman Filter is a navigation filter based on regular Kalman filters, more specifically Extended Kalman Filters, that model the "error state" of the system instead of modelling the movement of the system explicitly.

The navigation filter is used to track position, velocity and orientation of an object which is sensing its state through an Inertial Measurement Unit (IMU) and some means of observing the true state of the filter such as GPS, LIDAR or visual odometry.

Quaternion kinematics for the error-state Kalman filter
https://github.com/nordmoen/eskf-rs/blob/HEAD/docs/Error_State_Kalman_Filter.pdf


# AHRS attitude and heading reference system

https://x-io.co.uk/open-source-imu-and-ahrs-algorithms/


The AHRS sensor fusion algorithm to combines gyroscope, accelerometer, and magnetometer measurements into a single measurement of orientation relative to the Earth (NWU convention).

The algorithm provides the measurement of orientation as a quaternion. The library includes functions for converting this quaternion to a rotation matrix and Euler angles.

The algorithm also provides a measurement of linear acceleration and Earth acceleration. Linear acceleration is equal to the accelerometer measurement with the 1 g of gravity removed. Earth acceleration is a measurement of linear acceleration in the Earth coordinate frame.

Fuente https://github.com/xioTechnologies/Fusion

Paper https://ieeexplore.ieee.org/document/4608934

https://www.x-io.co.uk/res/doc/madgwick_internal_report.pdf

A Rust port of Madgwick's AHRS algorithm
https://crates.io/crates/ahrs



# ADAS

Se puede detectar que las condiciones se estan aproximando a perder tracción y avisar al conductor.
