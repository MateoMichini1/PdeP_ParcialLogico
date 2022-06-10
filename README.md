# Metaparcial

Los parciales son difíciles de crear, todos los años hay que tener temas nuevos y frescos. Este año usaremos las mentes de nuestros estudiantes para que hagan un programa que nos pueda crear parciales para futuros años.

![Market](metaparcial.jpg)

Los parciales tienen que tener un Tema Copado, que despierte el interés de estudiantes y les familiarice un poco al modelo. 
Los parciales tienen una lista de puntos que se deberán resolver, que suelen ser entre 7 y 10 puntos. Cada uno de esos puntos evalúa algún tema... y si o si tienen que ser evaluados todos los temas, como por ejemplo primer orden.

Nota. Tener en cuenta que todos los predicados deben ser totalmente inversibles, salvo que se aclare lo contrario.
```Prolog
% parcial(Tema, [Puntos]).
temaCopado(chocobos).
temaCopado(inversiones).
temaCopado(harryPotter).
temaCopado(carpinchos).
temaCopado(bidones).
temaCopado(piratas).
temaCopado(tierraMedia).
temaCopado(kraken).

punto(primerOrden).
punto(ordenSuperior).
punto(polimorfismo).
punto(listas).
punto(relleno).
punto(modelado).
punto(diagramado).
```
Se pide:

1. Hacer **parcialEvalua/2** que relaciona un parcial con un punto que evalúa. No requiere ser inversible para el parcial.

2. Hacer **esParcialListo/1** que resulta verdadero para un parcial que cumple todas las reglas de los parciales (tiene entre 7 y 10 puntos, tiene un tema copado y evalúa todos los puntos al menos una vez). 
No requiere ser inversible para el parcial.

3. Hacer **puntosInventados/1**, que genera una lista de puntos de cantidad válida.

4. Hacer **nuevoParcial/1**, que debe generar un parcial nuevo que esté listo.

5. Ya que nos están haciendo los parciales, vamos a tratar de predecir quienes van a aprobar. Agregar a la base de conocimiento un predicado que relacione el nombre de un estudiante y un punto que sabe, con ejemplos.

6. Hacer **aprueba/2**, que relaciona a un estudiante con un parcial, siempre y cuando sepa todos los temas que este último abarca.
No requiere ser inversible para el parcial.

7. Hacer una consulta que unifique la variable Aprobados con una lista de todos los estudiantes que aprueban este parcial:
```
parcial(chocobos, [primerOrden, primerOrden, ordenSuperior, polimorfismo, listas, relleno, modelado, diagramado]). 
```
**Nota:** No definir un nuevo predicado.

8. Saber si un parcial es sólo para elegidos, que es cuando sólo un alumno puede aprobarlo.
No requiere ser inversible para el parcial.