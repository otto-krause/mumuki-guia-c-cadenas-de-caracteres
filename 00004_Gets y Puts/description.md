Para resolver el problema anterior existe una función que nos va a ayudar, el nombre de la función es **gets**.

``` c
#include <stdio.h>
#include <stdlib.h>
int main() {
    char frase[50];
    printf ("escriba una frase") ;
    gets(frase);
    puts("La frase ingresada fue:");
    puts(frase);
    return 0;
}
```

gets nos soluciona el problema que teníamos con scanf, además te presentamos la función puts, que recibe una cadena de caracteres cualquiera y la muestra por pantalla.
