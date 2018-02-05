# matlab-visual-servo
matlab visual servo (legacy code)

# Copyright: (C) RoboticsLab @ 2013 Universidad Carlos III de Madrid
# Authors: Alvaro Martínez Estradé, Juan G. Victores
# CopyPolicy: Released under the terms of the LGPLv2.1 or later, see LGPL.TXT

* distancia: Calcula la distancia euclídea entre dos puntos (en 2D).
* ordenacion: Ordena 4 puntos en el orden de la toolbox (aprox. Fig 3.4).
* radtodeg: Radianes a grados.
* recseg1: Regsec para 1ª iteración (cuenta con etiquetado correcto).
* recseg: Coge de colorSegmentor los 4 puntos, comprueba si etiquetado bien, y llama ordenación si está bien.
* traj: Coge las posiciones de los motores y los apila en ua matriz.
* velocidad: Recibe las coordenadas destino, las actuales, halla el error, calcula la jacobiana visual,
halla la velocidad con la pinv, lo pasa a grados, aplica las ganancias, y envía las velocidades al robot.
Además devuelve el error.
* viss (main): Inicializa todo, implementa el bucle y comprueba errores y convergencias con tolerancias. También plots.

