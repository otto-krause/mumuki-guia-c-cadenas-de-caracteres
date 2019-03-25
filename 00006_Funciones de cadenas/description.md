Existen algunas funciones de cadenas para facilitarnos las cosas un poco, para ello vas a tener que importar las bibliotecas **string.h** y **ctype.h**. Primero te las explicamos y después te mostramos algunos ejemplos:

* **strcpy**: Copia una cadena.
* **strcmp**: Compara dos cadenas, si son iguales devuelve 0, si la primara es más larga que la segunda devuelve 1 y si la segunda es más larga que la primera, devuelve -1.
* **strcat**: Concatena dos cadenas, es decir, las junta en una nueva cadena.
* **toupper**: Recibe un caracter y devuelve su versión en mayúscula. Si ya está en mayúscula, lo devuelve como está.
* **tolower**: Recibe un caracter y devuelve su versión en minúscula. Si ya está en minúscula, lo devuelve como está.


**STRCPY**

``` c
#include <stdio.h>
#include <string.h>

int main ()
{
  char cadena1[]="hola";
  char cadena2[40];
  //El primer parametro es el destino, y el segundo el origen.
  strcpy (cadena2,cadena1);
  printf ("cadena1: %s\cadena2: %s\n",cadena1,cadena2);
  return 0;
}
```
**STRCMP**

``` c
#include <stdio.h>
#include <string.h>

int main ()
{
  char clave[] = "manzana";
  char respuesta[80];
  do {
     printf ("Cual es mi fruta favorita? ");
     gets(aux);
  } while (strcmp (clave,respuesta) != 0);
  puts ("Respuesta correcta!");
  return 0;
}
```

**STRCAT**

``` c
#include <stdio.h>
#include <string.h>

int main ()
{
  char str[80];
  strcpy (str,"estas ");
  strcat (str,"cadenas ");
  strcat (str,"estan ");
  strcat (str,"concatenadas");
  puts (str);
  return 0;
}
```

Para toupper y tolower su funcionamiento es el más simple:

``` c
=> toupper('a')
ム A

=> tolower('B')
ム b
```

No olvidar utilizar ctype.h para estas dos últimas