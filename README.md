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

# OPERADORES LÓGICOS
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

# USANDO FUNCIONES PARA NO REPETIR CÓDIGO
def ** nombre_funcion():
desarrollo de la funcion.

Los nombres de las funciones se escriben siempre en minusculas, nunca con numeros y siempre se separan con guion bajo.
Parametros: variables que voy a tener disponibles para usarla dentro de la función.

def conversacion (opcion):
    opcion = str(opcion)
    print('Hola')
    print('Elijiste la opcion ' + opcion)
    print('adios')

opcion = int(input('Elije una opcion (1, 2, 3: '))

if (opcion == 1):
    conversacion(opcion)
elif(opcion == 2):
    conversacion(opcion)
elif (opcion == 3):
    conversacion(opcion)
else: 
    print('Elijiste una opcion invalida')
    
    REDUCIENDO CÓDIGO
    
    def conversacion(opt):
    print('Hola')
    print('Como estas')
    print(f'Elegiste la opcion {opt}')
    print('Adios')

opcion = int(input('Elige una opción (1,2,3): '))

conversacion(opcion)

REDUCIENDO CÓDIGO EJEMPLO "CONVERSOR DE MONEDA PAISES":
*** EN VISUAL ***
def conversor (tipo_cambio, valor_dolar):
    soles = input("¿Cuánto dinero en moneda " + tipo_cambio + " tienes?: ") 
    soles= float(soles)
    dolares = soles/valor_dolar
    dolares=round(dolares,2)
    dolares=str(dolares)
    print("Tienes $" + dolares + " dolares")

    
menu = """
Bienvenido al conversor de monedas multipais

1- Moneda Mexicana
2-Soles Peruanos
3-Moneda Argentina

Elige una opción: 

"""
# de derecha a izquierda: llamo a la funcion input, le paso la variable menu para que la imprima y reciba el número que el usuario escogió, lo convierto a int y lo guardo en la variable 'opcion'
opcion = int(input(menu))

if opcion == 1: #moneda mexicana
    conversor("mexicana", 3877.8)
	
	
elif opcion == 2: #moneda peruana
	conversor("peruana",3.8)
	
elif opcion == 3: #moneda peruana
	conversor("argentina",24)
else:  #el usuario escribió algo diferente
	print('Escribe una opción correcta: ')

****EN CONSOLA***
λ py conversor.py

Bienvenido al conversor de monedas multipais

1- Moneda Mexicana
2-Soles Peruanos
3-Moneda Argentina

Elige una opción:

1
¿cuanto dinero en moneda mexicana tienes?: 100
Tienes $0.03 dolares
_______________________________________________
λ py conversor.py

Bienvenido al conversor de monedas multipais

1- Moneda Mexicana
2-Soles Peruanos
3-Moneda Argentina

Elige una opción:

2
¿cuanto dinero en moneda peruanos tienes?: 100
Tienes $26.32 dolares

# CADENAS DE CARACTERES (TEXTO).

nombre=input("¿Cuál es tu nombre?: ")

*** FUNCIÓN upper **
Función ligada al objeto específico
nombre.upper()

*** FUNCIÓN capitalize **
Primera letra en Mayúscula
nombre.capitalize()

*** se ejecuta el método nombre y se guarda dentro de la variable nombre
nombre=nombre.capitalize()

*** FUNCIÓN para quitar espacio **
Elimina los espacios sobrantes
nombre=nombre.strip()

*** FUNCIÓN lower **
Transforma la palabra en minúscula
nombre=nombre.lower()

*** FUNCIÓN replace **
Reemplaza letras 
nombre=nombre.replace()


** FUNCIÓN un caracter/letra***
accede a la cadena de caracteres
nombre[1]
letra =nombre[1]

** FUNCIÓN len **
Cuenta los caracteres de la palabra o cadena
len(nombre)
>>>7
len(letra)
>>>1

# SLICES (REBANADA)

ombre = "Francisco"
nombre
"Francisco"
nombre[0 : 3) 
// Arranca desde el primer índice hasta llegar antes del 3° índice.
"Fra"
nombre[:3] 
//Va desde el principio hasta antes de llegar del 3° índice. Cómo no hay ningún parámetro en el primer lugar, se interpreta que arranca desde el principio.
"Fra"
nombre[1:7] 
//Arranca desde el índice 1 hasta llegar antes del 7.
"rancis"
nombre[1:7:2] 
//Arranca desde el índice 1 hasta llegar antes del 7, pero pasos de 2 en 2, ya que eso es lo que nos indica el 3! parámetro, el cual es 2.
nombre[1::3] 
//Arranca desde el índice 1 hasta el final del string (al no haber ningún 2° parámetro, significa que va hasta el final), pero en pasos de 3 en 3.
"rcc"
nombre[::-1]  
//Al no haber parámetro en los 2 primeros lugares, se interpreta que se arranca desde el inicio hasta el final, pero en pasos de 1 en 1 con la palabra al revés, porque es -1.
"ocsicnarF"



