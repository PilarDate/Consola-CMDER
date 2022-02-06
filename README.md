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


# PRIMER PROGRAMA CON PHYTON
// EN VISUAL CODE CREAR UN ARCHIVO py conversor.py ESCRIBIR EL SGTE. CÓDIGO:

soles = input(" ¿cuantos soles tienes?: ") 
soles= float(soles)
valor_dolar=3.8
dolares = soles/valor_dolar
dolares=round(dolares,2)
dolares=str(dolares)
print("Tienes $" + dolares + " dolares")

// RESPUESTA EN CMDER
λ py conversor.py
 ¿cuantos soles tienes?: 500
Tienes $131.58 dolares

# UTILIZANDO CONDICIONALES
 EN VISUAL CODE CREAR UN ARCHIVO py conversor.py ESCRIBIR EL SGTE. CÓDIGO:
edad=int(input("Escribe tu edad: "))
if edad >17:
    print('joven estudiando en la U o trabajando')
else:
    print('joven estudiando secundaria- primaria-inicial-prekinder')

// RESPUESTA EN CMDER
λ py condicionales.py
Escribe tu edad: 42
joven estudiando en la U o trabajando

λ py condicionales.py
Escribe tu edad: 11
joven estudiando secundaria- primaria-inicial-prekinder

//*** OTRO EJEMPLO
// EN VISUAL CODE CREAR UN ARCHIVO py conversor.py ESCRIBIR EL SGTE. CÓDIGO:
numero =int(input("Escribe un numero: "))
if numero > 5:
    print('Es mayor a 5')
elif numero == 5:
    print('Es igual a 5')
else:
    print('Es menor a 5')
    
// RESPUESTA EN CMDER    
λ py condicionales.py
Escribe un numero: 5
Es igual a 5

λ py condicionales.py
Escribe un numero: 6
Es mayor a 5

λ py condicionales.py
Escribe un numero: 2
Es menor a 5

# PROGRAMA DE CONVERSOR DOLARES DE 3 PAÍSES *****

// EN VISUAL CODE CREAR UN ARCHIVO py conversor.py ESCRIBIR EL SGTE. CÓDIGO:
menu = """
Bienvenido al conversor de monedas multipais

1-Pesos Mexicanos
2-Soles Perduanos
3-Pesos Argentinos

Elige una opción: 

"""
opcion = int(input(menu))

if opcion == 1: #pesos mexicanos
	#pregunto al usuario la cantidad a convertir
	pesos = input('¿Cuántos pesos mexicanos tienes?: ')
	#convierto a float para mejor manejo de datos
	pesos = float(pesos)
	#escribo el valor del dolar en pesos mexicanos
	tipo_de_cambio = 21.5
 
elif opcion == 2: #soles peruanos
	#pregunto al usuario la cantidad a convertir
	pesos = input('¿Cuántos soles peruanos tienes?: ')
	#convierto a float para mejor manejo de datos
	pesos = float(pesos)
	#escribo el valor del dolar en soles peruanos
	tipo_de_cambio = 4
 
elif opcion == 3: #soles peruanos
	#pregunto al usuario la cantidad a convertir
	pesos = input('¿Cuántos pesos argentinos tienes?: ')
	#convierto a float para mejor manejo de datos
	pesos = float(pesos)
	#escribo el valor del dolar en pesos argentinos
	tipo_de_cambio = 452
 
else:  #el usuario escribió algo diferente
	print('Escribe una opción correcta: ')

#hago la conversión
dolares = pesos / tipo_de_cambio
#redondeo los dólares a dos decimales
dolares = round(dolares, 2)
#convierto el float de dolares a un string
dolares = str(dolares)

#imprimo el valor de la conversion. Se pueden sumar (concatenar) strings con '+'
print('Tienes $' + dolares +' dólares')

λ py condicionales.py

// RESPUESTA EN CMDER

Bienvenido al conversor de monedas multipais
1-Pesos Mexicanos
2-Soles Perduanos
3-Pesos Argentinos

Elige una opción:

2
¿Cuántos soles peruanos tienes?: 100
Tienes $25.0 dólares
