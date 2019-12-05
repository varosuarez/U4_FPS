
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
 