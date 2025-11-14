# Memoria-y-Planificadores

Al finalizar esta actividad se obtuvo una descripción del funcionamiento de los procesos de usuario en términos del procesador y de la memoria consumida.

## Insumos necesarios para el TP
Para realizar esta actividad fue necesario repasar las teóricas de planificadores y administración de memoria.

## Enunciado del Mini TP
Hace poco la materia SOR se compró un Raspberry pi, el cual tiene un procesador ARM v8, 1.2 Ghz, 4 núcleos y 1 Gb de Ram. Para instalar el sistema operativo le compró una tarjeta micro sd, 32 gb clase 10 marca Lexar. Instaló Ubuntu mate, pero no quedó muy conforme. Decide consultarle a sus amigos de SOR2 y ellos le aconsejan instalar Raspbian Buster Lite (de 32 bits).
Una vez instalado el S.O. comprueba el estado de los procesos con htop y ve lo siguiente:

Apa1rentemente el sistema operativo consume 54.1 MB, averigua también que Raspbian hace paginación de a 8KB. Decide compilar un programa en C con funciones recursivas y nota que cuando ejecuta en la consola
root@raspi02:~# ./ejecutable_A   este consume 128.05 MB. 

## Memoria
Responder:

a) ¿Cuántos bits necesito para dar un número de página del proceso ejecutable_A (el de las funciones recursivas)?

b) ¿Cuántos bits necesito para el desplazamiento dentro de un frame? 

c) ¿Cuántas páginas se asignan al proceso ejecutable_A? 

d) ¿Hay fragmentación? Justificar.


## Planificador
Supongamos que el sistema ejecuta 2 procesos de las siguientes características:
PROCESO 1 : Ejecuta 20 unidades de tiempo, luego efectúa una E/S sobre disco, luego ejecuta 10 unidades de tiempo. y termina.
PROCESO 2 : Ejecuta 60 unidades de tiempo y termina.
El método de selección de la cola de listos es el Round Robin asignándole a cada proceso un quantum de 20 unidades de tiempo. Una operación de E/S sobre disco tarda el equivalente 30 unidades de tiempo. 
Suponer que ambos procesos llegan al mismo tiempo a la cola de listos y que el planificador decide ejecutarlos y planificarlos sobre el mismo núcleo.

Observación: tiempo de conmutación de tarea (context switch) de 0.5 unidades de tiempo

Representar la planificación en un diagrama de Gantt e informar el tiempo de retorno de ambos procesos por separado. Puede realizar la planificación en una planilla de cálculo. Justificar su planificación con el seguimiento paso por paso de Round Robin.
