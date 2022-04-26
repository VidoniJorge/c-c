# c-c

# Estructura de datos
## Basic types

* Aritmeticos 
  * **int** 2 o 4 Bytes permite tener numeros negativos y positivos
      * 2 Bytes -32,768 to 32,757
      * 4 bytes -2,147,483,648 to 2,147,483
  * **unsigned int** 2 o 4 bytes no nos permite tener datos negativos
      * 2 Bytes 0 to 65.535
      * 4 bytes 0 to 4,294,967,295
  * **short** 2 Bytes: -32,768 to 32,767
  * **unsigned short** 2 Bytes: 0 to 65,535
  * **long** 8 Bytes: -9223372036854775808 to 9223372036854775807
  * **unsigned long** 8 Bytes 0 to 18446744073709551615
* Florante
  * **float** 4 Bytes 1.2E-38 to 3.4E+386 ( 6 decimal places)
  * **double** 8 Bytes 2.3E-308 to1.7E+30815 (15 decimal places)
  * **long double** 10 Bytes 3.4E-4932 to 1.1E+493219 (19 decimal places)

## Void
Especifica que no hay valor disponible. Se utiliza en 3 escenarios:
* Para especificar el tipo de dato que retorna una funcion. void fun(){}
* Para especificar que la funcion no acepta parametros. int fun(void){}
* Para indicarle a un puntero que no nos importa el tipo de dato al que apunta.

## ENUM

``` c
enum designElements{
 ITALICS = 1;
 BOLD = 2;
 STRIKE = 3;
}
```

``` c
#include <stdio.h>

enum weekDays{Sunday, Monday, Tusday, Wednesday, Thursday, Friday, Saturday};

int main() {
 enum weekDays today;
 today = Sunday;
 printf("Day %d", today+1);
 return 0;
}
```

``` c
#include <stdio.h>

enum deck{
 club = 0,
 diamond = 5,
 hearts = 10,
 spades = 15,
} card;

int main() {
 card = spades;
 printf("Card value %d",card);
 return 0;
}
```




