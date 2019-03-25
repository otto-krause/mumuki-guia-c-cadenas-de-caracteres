Ahora vamos a ver dos funciones que nos van a servir para guardar caracteres, veamos el siguiente código:

``` c
#include<stdio.h>
#include<conio.h>
 
void main()
{
    printf("Ingrese un caracter:");
    char a = getch();
    printf("El caracter ingresado fue %c",a);
    printf("El codigo ASCII de ese caracter es %d",a);
    
    printf("Ingrese un caracter:");
    char b = getchar();
    printf("El caracter ingresado fue %c",b);
    printf("El codigo ASCII de ese caracter es %d",b);
}

```

Probá el código en tu compilador, analizalo y elegí las opciones correctas
