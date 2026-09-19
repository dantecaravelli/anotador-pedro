# Tantos de Pedro

Contador de puntos para jugar al Pedro, el juego de cartas. Una sola página web, sin instalar nada: se abre en el celular y se anota ahí mismo en la mesa.

## Cómo se juega al Pedro

De 3 a 6 jugadores. Cada uno recibe cuatro cartas y al principio puede mirar dos. Por turnos se van robando cartas del mazo y cambiándolas por las propias, con el objetivo de quedarse con la menor suma posible.

Cuando alguien cree que tiene la suma más baja, canta **Pedro** y todos muestran:

- Si al que cantó le salió, suma **0**.
- Si alguien le ganó, suma lo mismo que el jugador que más puntos hizo en esa ronda.
- El resto suma lo que le quedó en la mano.

Pierde el primero que llega a **100 puntos**. Ese queda afuera y los demás siguen jugando hasta que queda uno solo: ese gana.

## Qué hace la página

- Se arma la partida eligiendo de 3 a 6 jugadores y sus nombres.
- Cada ronda se carga lo que sumó cada uno y la tabla se ordena sola: el que menos tiene va primero.
- Marca en dorado al que pasa los 70 y en rojo al que pasa los 90, para ver de una mirada quién está por salir.
- Al llegar a 100 el jugador queda tachado como *afuera* y deja de pedir puntos, pero sigue en la tabla.
- Se puede sumar un jugador con la partida empezada: entra con 10 puntos más que el que peor va.
- Deshacer la última ronda, por si se cargó mal un número.
- Historial completo de todas las rondas.
- Ayuda opcional: si se marca quién cantó Pedro, la página calcula sola qué le corresponde.
- La partida queda guardada en el navegador, así que se puede cerrar la pestaña sin perder la tabla.

## Cómo se usa

Abrir `index.html`. Nada más: es un solo archivo, no necesita servidor ni instalación.

## Cómo está hecho

HTML, CSS y JavaScript a mano, sin librerías. Los datos de la partida se guardan en el `localStorage` del navegador, o sea que viven en ese teléfono o computadora y no se comparten entre dispositivos.
