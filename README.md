Torneos de eSports: UML
Autor

Nombre: Felix Ruiz de la Cuesta  
GitHub: github.com/felaks03

De qué va esto

Mi repositorio: https://github.com/felaks03/torneo-esports-uml.git  
Este proyecto es mi intento de montar un sistema para gestionar torneos de eSports, usando diagramas UML.
La idea era imaginar cómo se organizarían equipos, jugadores y torneos, y explicar quién hace qué y cómo encaja todo.

Los diagramas
Mis casos de uso
Me tocó hacer tres diagramas para enseñar cómo los usuarios (básicamente el administrador y los equipos) interactúan con el sistema.
  

Apuntar un equipo a un torneo: Esto deja que el administrador o el equipo diga "¡vamos a ese torneo!".
Pero primero hay que tener el equipo creado. Por eso puse un <<include>>, que conecta las dos cosas.

Meter un jugador en un equipo: Aquí el administrador coge a un jugador y lo añade a un equipo.

Mirar la lista de equipos y jugadores: Esto es para que el administrador o los equipos puedan ver quién está registrado.

El diagrama de clases
  

Aquí puse todas las piezas del sistema: Torneo, Equipo, Jugador, Partida y Premio. También definí cómo se conectan, como que un Torneo tiene varios Equipos (eso es agregación, porque un equipo puede estar fuera de un torneo), y que un Equipo está hecho de Jugadores (eso es composición, porque sin equipo, un jugador no pinta nada). Luego añadí unas clases de control (GestorTorneos, GestorEquipos, etc.) y una clase VistaPrincipal para que el usuario interactúe.

Los casos de uso los hice separados porque el proyecto pedía nombres específicos para cada archivo, y quería que quedara claro.
Para las clases, me imaginé cómo montaría este sistema si tuviera que programarlo de verdad.

Dividí todo en tres grupos:  

Las entidades (Torneo, Equipo, Jugador, etc.) son como los datos básicos.  
Las clases de control (GestorTorneos, GestorEquipos) son las que hacen el trabajo pesado, como registrar cosas o calcular resultados.  
La clase de interfaz (VistaPrincipal) es para que el usuario pueda meter datos o ver resultados.
