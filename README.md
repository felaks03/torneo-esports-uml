Sistema de Gestión de Torneos de eSports

Autor
Nombre: Felix Ruiz de la Cuesta
Perfil de GitHub: github.com/felask03

Descripción del Proyecto

Enlace al repositorio: https://github.com/felask03/torneo-esports-uml.git
Este proyecto modela un sistema de gestión de torneos de eSports utilizando diagramas UML para representar las interacciones y la estructura del sistema.

Diagramas UML
Diagramas de Casos de Uso


Registrar un Equipo: Permite al administrador crear un nuevo equipo en el sistema.
Inscribir Equipo en Torneo: Permite al administrador o equipo inscribir un equipo en un torneo, requiriendo que el equipo esté registrado primero (<<include>>).



Añadir Jugador a Equipo: Permite al administrador añadir un jugador a un equipo existente.


Ver Lista de Equipos y Jugadores: Permite al administrador o equipo consultar la lista de equipos y jugadores registrados.


Diagrama de Clases

Representa las clases principales (Torneo, Equipo, Jugador, Partida, Premio) y sus relaciones (agregación entre Torneo y Equipo, composición entre Equipo y Jugador). Incluye clases de control (GestorTorneos, GestorEquipos, GestorPartidas, GestorPremios) y de interfaz (VistaPrincipal).
