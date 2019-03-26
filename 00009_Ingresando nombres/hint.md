Suponiendo que por ejemplo el vector nombres[10][20] vale "juan" en la posición tres, si accediéramos a cada caracter obtendríamos algo así:

``` c
nombres[3][0] => vale 'j'
nombres[3][1] => vale 'u'
nombres[3][2] => vale 'a'
nombres[3][3] => vale 'n'
nombres[3][4] => vale null
.
.
//Sigue hasta 20
.
.
nombres[3][20] => vale null
```

Lo único que deberíamos hacer sería convertir cada caracter a mayúsculas. ¿Te acordás de **toupper**?