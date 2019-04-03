# castanedaPerdomo_Taller1

##Documentación

###1. Eclipse

###1.1 Estación

Esta clase es la que se va a encargar de crear un objeto de tipo Estación que se va a pintar y hacer los cambios en su tamaño cuando se unda
**Métodos:**
+Estacion(int, int, int): es el constructor de la clase, recibe parametros para su posición y el tipo de objeto que se va a crear
+run(): aquí se va a hacer el cambio temporal del tamaño de la imagen al ser presionado
+pintar(): pinta la imagen dependiendo del onjeto que sea
+undido(): es el metodo que se llama cuando se queira hacer el cambio de la imagen

###1.2 Main

Es donde ocurre toda la validación de la secuencia dpeendiendo de lo que recibe de Android
**Métodos:**
+Main(Strin[])
+setup(): se inicializan todas las variables
+settings(): se establece el tamaño del lienzo
+draw(): se pinta lo que debe ir en cada pantalla
+comparar(): se encarga de comprar lo que viene de Android con la secuencia que está creada en eclipse
+agregarPaso(): se encarga de crear un paso nuevo aleatorio a la secuencia
+recorrerSecuencia(): es el que se encarga de recorrer y mostrar la secuencia guardada en eclipse para mostrarle al usuario la que debe seguir

###1.3 Comunicacion
Recibe la información que viene de Android
**Métodos:**
+Recibir(): recibe la comunicación de Androir
+Enviar(): envía a Android


###2. Android

###2.1 MainActivity

Esta será la primera pantalla que se le muestre al usuario, tendrá un botón de play que inicie el juego; un EditText para poner el IP, un TextView que muestra el mejor puntaje y botón de ayuda que lleva a la pantalla de instrucciones. También tiene una referencia a Comunicación para notificarle a eclipse que cambie de pantalla.

###2.2 Juego

Esta ya es la pantalla de juego que tendra cuatro botones cada uno con una estación. Tiene un TextView que muestra el puntaje y otro que muestra el tiempo y tiene una referencia a Comunicación para recibir los mensajes de android en caso de equivocarse y para notificarle que debe cambiar de pantalla.

###2.3 Perder
Esta es la pantalla que se muestra en caso de que el usuario se equivoque en la secuencia. tiene un TextView donde muestra el puntaje que tuvo seguido de otro TextView que muestra el mejor puntaje hasta ahora. También tiene dos botones: unos para reiniciar y el otro para ir a la pantalla de inicio. Y por último una referencia a Comunicacion para notificar a eclipse que debe cambiar de pantalla.

###2.4 Ayuda
Esta pantalla muestra las instrucciones de juego. Las instrucciones están incluidas en la imagen de fondo y solo tien eun botón de play. Cuenta con una referencia a Comunicación para notificar a eclipse el cambio de pantalla.

### 2.5 Comunicacion
Esta clase se encarga de crear la comunicación con eclipse y de enviar y recibir información del mismo.
