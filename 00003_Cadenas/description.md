Hasta hora vimos como guardar caracteres, pero como hacemos si queremos guardar una palabra o una oración.<br>
Para poder utilizar cadenas en C, vamos a necesitar crear vectores de tipo char.<br>
Por lo tanto si queremos declarar una cadena podemos hacer lo siguiente:

``` c
char cadena[20] = "Hola mundo";
```
A tener en cuenta:

* Es una cadena con espacio para 20 caracteres
* Se están utilizando 11 caracteres del total de la cadena, pero si los contas los caracteres de "Hola mundo" solo vas a ver 10
* Lo anterior se debe a que todas las cadenas insertan un caracter especial para indicar el final de la línea, ese caracter suele mostrarse como \0

Y si quisieramos ingresar cadenas? La verdad es que se complica un poco, tratemos de utilizar scanf:

``` c
char cadena[20];
scanf("%s",cadena);
printf("La cadena ingresada es: %s", cadena)
```

Les proponemos que prueben esa porción de código en un compilador, después de algunos intentos van a llegar a esta conclusión:

> **No se pueden ingresar palabras con espacios**

Esto se debe a que en realidad scanf solo recibe entradas formateadas, es como el printf pero para ingresos. Para que quede más claro:

``` c
char cadena1[20];
scanf("%s %s",cadena1,cadena2);
printf("Las cadenas ingresadas son: %s %s", cadena1, cadena2);
```

De esa manera podríamos ingresar palabras con espacios, pero nos resulta impractico porque hay veces en las que queremos almacenar palabras con espacios en una única palabra, en la próxima lección vamos a explicarte como se resuelve este problema.
