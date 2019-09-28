# Tarea-3
Guía de ejercicios en clase
#Ejercicio 1
Luego de ingresar el comando "listaDeNumeros[5]" lo que nos arrojaba la posición numero 5 de nuestra lista de numeros, dando como resultado el numero 1, reemplazamos el número 5 por el 0, es decir le damos la orden de buscar la posición 0, dando como resultado "list()". ¿Por qué nos dio este resultado? esto se debe a que a la posición 0 no se le atribuye ningún valor de la lista previamente creada.
Al buscar "listaDeNumeros[-5]" lo que R nos arroja es una nueva lista, esta lista es igual excepto por una pequeña diferencia, el numero 1, ubicado en la posición 5 de la lista no esta, esto quiere decir que cuando reemplazamos el 5 por un numero negativo llamamos una lista que suprime la posición que posimos en negativo, como en este caso que suprimio la quinta posición.
Si colocamos un valor que excede los números que posee la lista, en este caso "listaDeNumeros[14]" lo que nos entrega "null" lo que quiere decir "nulo" es decir que no se encuentra la posición a la que estamos llamando, ya que se encuentra fuera de los parametros de la lista.

#Ejercicio 2
Ejecutamos Comando 1:
unlist(listaDeNumeros[5]) 
if(listaDeNumeros[5]+1>0){
  print("se cumple")
}
Observación, R nos arroja un error.
Ejecutamos Comando 2:
if(unlist(listaDeNumeros[5])+1>0){
  print("se cumple")
}
Observación: "se cumple"
Conclusión:El comando 1 posee la el comando "unlist" fuera del condicional "if", es por esto que nos arroja un error, porque en la función condicional solo llamamos a la posición 5  para sumarla y una posición no es necesariamente un número, es por esto que R nos entrega un error. En el caso del comando 2, dentro de la función condicional se encuentra el comando "unlist" este extrae la posición 5 en su formato natural, en este caso como valor, ya que la posición 5 en la lista tiene el valor de 1, es por esto que se puede sumar, porque el programa lo reconoce como un valor y por ende lo puede sumar con otro valor, en este caso 1+1=2 y al ser 2>0, la condicion se cumple.
Finalmente el comando "unlist" nos ayuda a extraer el valor para que el programa lo reconozca como tal y popdamos utilizarlo como número.

#Ejercicio 3
Al ejecutar el comando "listaDeNumeros[5] <- 12" lo que hacemos es asignar el valor 12 a la posición número 5, lo que quiere decir que reemplazamos el 1 por un 12. Este cambio lo observamos simplemente revisando la lista "View(listaDeNumeros)". 

#Ejercicio 4
Al ejecutar "length(nombre_variable)" R nos arroja un error, este dice que no encuenta "nombre_variable" y esto es evidente ya que no estamos usando este, es por esto que se hace necesario cambiarlo por "listaDeNumeros" que es la lista que estamos utilizando, al ejecutarlo encuentra la lista y nos entrega el numero de posiciones que este posee.

#Ejercicio5
Ejecutamos: "valorInicial <- 5" y "valorFinal <- 20"
Observación: Para visualizar los cambios ejecutamos "valorInicial : valorFinal" ahora podemos observar que se genero una secuenca de menor a mayor con 15 valores, partiendo del 5 y terminando en el 20.
Ejecutamos: "valorInicial <- 20" y "valorFinal <- 5"
Observación: Para visualizar los cambios ejecutamos "valorInicial : valorFinal" ahora podemos observar que se genero una secuenca de mayor a menor con 15 valores, partiendo del 20 y terminando en el 5.
Ejecutamos: "length(listaDeNumeros) : valorFinal"
Observación: Se genera una secuencia de mayor a menor desde el 11 hasta el 5, esto sucede porque "length(listaDeNumeros)" es el número de posiciones que tiene la lista, al ser este número 11 y además colocarla como punto de partida da com resultado la secuencia anteriormente descrita. 
Ejecutamos: "valorInicial : length(listaDeNumeros)"
Observación: Se genera una secuencia de mayor a menor desde el 20 hasta el 11, esto sucede porque "length(listaDeNumeros)" es el número de posiciones que tiene la lista, al ser este número 11 y además colocarla como punto en el cual finaliza, da com resultado la secuencia anteriormente descrita. 
Ejecutamos: "valorInicial <- 20" y "valorFinal <- 20" 
Observación: Para visualizar los cambios ejecutamos "valorInicial : valorFinal" ahora podemos observar que solo aparece el valor 20, en este caso al iniciar en 20 y finalizar en 20 no se genera una secuancia ya que una secuaencia "es la creación ordenada de números" y ahora solo tenemos un número.

#Ejercicio 6














