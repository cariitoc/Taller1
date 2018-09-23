Descripción del UML del taller uno -Ecosistemas de aplicaciones
-------------------------------------------------
Main
--------------------------------------------------
Atributos 
-------------------------
**Sue jugador1:** Variable para el jugador numero uno.
**Chris jugador2:** Variable para el jugador numero dos.

Metodos
-------------------
**Settings():void:** Metodo para definir el tamaño el lienzo.
**setUp():void:** Metodo para ejecutar el codigo.
**mousePressed():void:** Metodo para iniciar el juego haciendo click en el boton star.



Pantalla
-------------------
Atributos
-------------
**Pimage incio:** Variable para la pantalla de inicio.
**Pimage instrucciones:** Variable para la pantalla de instrucciones.
**Pimage juego:** Variable para la pantalla del juego.
**Pimage gano:** Variable para la pantalla que muestra si uno de los jugadores gano.
**Pimage perdio:** Variable para la pantalla que muestra si uno de los jugadores perdio.
**int tiempo:** Variable para le tiempo que se demora el juego en completarse, para ambos jugadores.
**PVector[] obj:** Variable para las posiciones de las variables.

Metodos
--------------
**Pantalla():** Constructor de la clase Pantalla.
**pintar():void:** Metodo
**ContabilizarTiempo():void:** Metodo
**perdio():** Metodo
**gano():** Metodo


Hacha
-------------------
Atributos
-------------
**Pimage hacha:** Variable para pintar el hacha.
**PVector[] obj:** Variable para la posicion del hacha.

Metodos
--------------
**Hacha():** Constructor de la clase Hacha.
**pintar():void:** Metodo para pintar el hacha.


Jugador
-------------------
Atributos
-------------
**PVector[] obj:** Variable para la poscion del hacha, es una variable tipo protected.
**int puntaje:** Variable para el puntaje del jugador, que se convertira despues en el tiempo, es una variable tipo protected.

Metodos
--------------
**Jugador():** Constructor de la clase Jugador.
**pintar():void:** Metodo para pintar a los jugadores, es un metodo sobreescribido ya que los hijos tendran su propio pintar.
**recoger():void:** Metodo  para recoger las hachas, es un metodo sobreescribido ya que los hijos tendran su propio pintar.
**vida():void:** Metodo para saber cuanta vida tiene el personaje , es un metodo sobreescribido ya que los hijos tendran su propio pintar.
**mover():void:** Metodo para el movimiento de los personajes,es un metodo sobreescribido ya que los hijos tendran su propio pintar.


Sue
-------------------
Atributos
-------------
**Pimage personaje1:** Variable para pintar al jugador 1.

Metodos
---------------
**Sue():** Constructor de la clase Sue.



Chris
-------------------
Atributos
-------------
**Pimage personaje2:** Variable para pintar al jugador 2.

Metodos
---------------
**Chris():** Constructor de la clase Chris.





Enemigo
-------------------
Atributos
-------------
**int daño:** Variable para el nivel de daño que los enemigos causan a los personajes, es una variable tipo protected.
**int mover:** Variable para el movimiento de los enemigos,es una variable tipo protected.
**PVector[] obj:** Variable para la posicion de los enemigos, es una variable tipo protected.

Metodos
--------------
**Enemigo():** Constructor de la clase Enemigo..
**pintar():void:** Metodo para pintar los enemigos, es un metodo sobreescribido ya que los hijos tendran su propio pintar.
**mover():void:** Metodo para mover a los enemigos, es un metodo sobreescribido ya que los hijos tendran su propio mover.
**daño():void:** Metodo para hacer daño a los jugadores, es un metodo sobreescribido ya que los hijos tendran su propio daño.



Fantasma
-------------------
Atributos
-------------
**Pimage fantasmas:** Variable para pintar a los fantasmas.


Metodos
---------------
**Fantasma():** Constructor de la clase Fantasma.




BolaPlasma
-------------------
Atributos
-------------
**Pimage plasma:** Variable para pintar las bolas de plasma

Metodos
---------------
**BolaPlasma():** Constructor de la clase BolaPlasma.


Sangre
-------------------
Atributos
-------------
**Pimage sangre:** Variable para pintar la sangre.

Metodos
---------------
**Sangre():** Constructor de la clase Sangre.



Servidor
------------------
Inteface MensajeObserver
-----------------
Atributos
---------------
**OnDataReceiver(Object):void** Aplica el patron observer.


ServerSingleton
--------------------
Atributos
----------------------
**ServerSocket serverSocket** Espera la  solicitud.

Metodos
--------------------
**ServerSingleton():** Constructor de clase ServerSingleton.
**getConstructor(): ServerSingleton** Se inicializa a si mismo si detecta que es un nulo 
**run(): void** Metodo para la recepcion y envio.
**setObserver(MensajeObservador): void** Metodo para gestionar el patron observer



TCPConection
----------------------
Atributos
-------------------------
**Socket socket:** Variable para comunicar.

Metodos
---------------------
**TCPConection()** 
**getConstructor() Comunication** 
**run(): void**
**serObservador(MensajeObservador): void**



Receptor
----------------------
Atributos
--------------------
**Socket socket;**

Metodos
---------------------
**Receptor();**
**run(): void**
**recibir():void**

