
# Change Log

Añado este archivo para llevar la cuenta de lo que se va haciendo, como extensión de los commits
 
 
## [1.0.2] - 04/12/2019
  
Añadido el spawn de enemigos
 
### Añadido
 
 - Blueprint **Mob Generator**. Genera enemigos cada *t* segundos hasta llegar a un tope. Cada generador tiene un contador individual de los enemigos generados. Cuenta con *HP* propia, la cual se regenera cada 2 segs.
 
### Modificado
  
- Blueprint **Enemy**. Añadida una referencia al generador que lo spawneó. Añadido justo antes del *DestroyActor* el decremento al contador de éste generador.
- Eliminado el enemigo por defecto del nivel. Únicamente aparecen por los spawners.
 
### Arreglado
 
 
 ## [1.0.5] - 11/12/2019
  
Añadido fade in y fade out del HUD cuando se hace focus con el click izquierdo y los contadores para enemigos y generadores.
 
### Añadido
 
 - Animaciones y eventos entre el **HUD** y **FirstPersonCharacter** para el efecto de focus.
 - Contador de enemigos y de generadores en el **HUD**.
 
### Modificado
  
- Blueprint **FirstPersonCharacter**. Añadidas variables para llevar el conteo de generadores y enemigos.
- Blueprint **Enemy**. Añadida suma y resta de las variables del nivel (guardadas en el jugador, no hay forma fácil de acceder a las variables si se ponen como variables de nivel) cuando se crea y se destruye.
- Blueprint **Mob Generator**. Añadida suma y resta de las variables del nivel cuando se crea y se destruye.
 
### Arreglado
 