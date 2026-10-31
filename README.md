
# SINCRONIZACION DE HILOS

## Materia: Sistemas Operativos

### Descripcion

En esta practica se realizo un programa en Python para trabajar con hilos. El ejercicio consiste en procesar 24 documentos utilizando cuatro trabajadores.

Los trabajadores utilizados son:

- Rosmery
- Neyda
- Maricel
- Alex

Cada trabajador tiene la tarea de procesar seis documentos.

### Objetivo

Realizar un ejercicio practico para conocer como trabajan los hilos y como se pueden organizar varias tareas dentro de un programa.

### Herramientas utilizadas

- Python
- Google Colab
- Libreria threading
- Libreria queue
- Libreria time
- Libreria random

### Desarrollo de la practica

El programa realiza las siguientes actividades:

1. Crear una cola con 24 documentos.
2. Crear cuatro hilos de ejecucion.
3. Asignar un trabajador a cada hilo.
4. Procesar seis documentos por trabajador.
5. Utilizar Lock para proteger los resultados compartidos.
6. Utilizar join para esperar que terminen los cuatro hilos.
7. Mostrar el resumen del trabajo realizado.

### Verificaciones realizadas

Se realizaron cuatro ejecuciones del programa para comprobar su funcionamiento.

En cada ejecucion se verifico lo siguiente:

- Que se procesen los 24 documentos.
- Que no existan documentos repetidos.
- Que no queden documentos pendientes.
- Que cada trabajador procese seis documentos.
- Que los cuatro hilos finalicen correctamente.
  1. ¿Por que queue.Queue es apropiada para compartir trabajos?
Porque permite repartir los 24 documentos entre los cuatro trabajadores sin que se repita el mismo documento. Cada uno va tomando un trabajo de la cola hasta terminar.
2. ¿Que protege Lock y que pasaria si se actualizara el resumen sin el?
Lock protege los resultados que comparten los trabajadores. Sin el podrian producirse errores cuando varios hilos intenten actualizar los datos al mismo tiempo.
3. ¿Que cambiarias si cada documento tuviera que guardarse en un archivo real?
Agregaria una parte para guardar cada documento en la computadora y controlaria que dos trabajadores 


### Evidencias

Se adjunta un archivo PDF con las cuatro capturas de las ejecuciones realizadas en Google Colab.
