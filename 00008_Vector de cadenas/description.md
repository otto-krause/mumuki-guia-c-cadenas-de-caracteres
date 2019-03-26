¿Que pasaría si quisiéramos tener un vector de cadenas? <br>
Se complica un poco imaginarlo ¿No?<br>

La solución a esto es agregando una dimensión más a nuestros vectores, algo que más adelante conoceremos como **matrices**. Por ahora solo analizá el siguiente código:

``` c
char nombres[10][30];
for(int i=0; i<10; i++)
{
  printf("Ingrese un nombre: ");
  gets(nombres[i]);
}
```
Este código va a ingresar los nombres de 10 alumnos, con un máximo de 30 caracteres por nombre.<br>
A tener en cuenta:

* La primer dimensión del vector indica cuantas cadenas habrá.
* La segunda dimensión del vector indica cuantos caracteres tendrá cada cadena.
* Cuando llamamos a gets, vamos a usar solamente la primera dimesión para indicar en cuál cadena guardar el ingreso.
* Si quisieramos mostrar una cadena en específico se debe indicar con la primer posición, por ejemplo: puts(nombres[3]), mostraría por pantalla la tercer cadena en el vector de strings.