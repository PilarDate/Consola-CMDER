# Consola-CMDER
//Usando CONSOLA CMDER 
comandos básicos para consola:
Ctrl + L = Limpiar pantalla
CD = Change Directory
… = Carpeta padre
CD… = Cambiar de directorio a la carpeta padre
Alt + 92 =
ls = list
mkdir = Make directory
touch = para crear archivos

¤////#
input("Ingresa un dato:")

//sumar números:
primero determinar entero
>>> dato1 =input("Ingresa un dato:")
Ingresa un dato:1
>>>
>>> dato2 =input("Ingresa un dato:")
Ingresa un dato:2
>>> dato1 =int(dato1)
>>> dato2 =int(dato2)
>>> dato1+dato2
3

OPERADORES LÓGICOS
and para comparar si dos valores son verdaderos.
-or para comparar si dos valores son falsos.
-not para invertir el valor booleano.
-== Compara dos valores y te dice si son iguales o no.
-!= Compara dos valores y te dice sin son diferentes o no.
-> Compara si es mayor que otro valor.
-< Compara si es menor que otro valor.
>= igual o mayor que el valor a comparar.
<= igual o menor que el valor a comparar.
Seguro que muchos lo podéis explicar mucho mas claro. Un saludo!

EJEMPLO:
pepe_estudia = True
>>> ana_trabaja = True
>>> ana_duerme = True
>>> ana_estudia and pepe_trabaja and ana_duerme
True
>>> ana_estudia and pepe_trabaja andnot(ana_duerme)
False
>>> ana_come = False
>>> ana_come or ana_duerme
True
>>> not(ana_come) ornot(ana_duerme) ornot(ana_estudia)
True
// En este caso sigue dando True porque ana_come = False y al agregarle un not su valor es True.
Pero si hago lo siguiente,todos los valores son False:
>>> ana_come ornot(ana_duerme) ornot(ana_estudia)
False

OTRO EJEMPLO:

AND
true and true = true
true and false = false
false and true = false
false and false = false
OR
true or true = true
true or false = true
false or true = true
false or false = false

