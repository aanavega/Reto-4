# Reto-4

A continuacion los programas planteados del reto correspondiente en el notebook de jupiter:

### Codigo numero 1
- Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.

```Python
# Leer un numero entero
numero : int
numero = int(input("Ingrese un numero entero: "))

# Determinar si el numero corresponde al codigo ASCII de una vocal minuscula
if numero == 97:
    print('El numero ' + str(numero) + ' corresponde a la vocal "a"' )
else:
    if numero == 101:
        print('El numero ' + str(numero) + ' corresponde a la vocal "e"')
    else:
        if numero == 105:
            print('El numero ' + str(numero) + ' corresponde a la vocal "i"')
        else:
            if numero == 111:
                print('El numero ' + str(numero) + ' corresponde a la vocal "o"')
            else:
                if numero ==117:
                    print('El numero ' + str(numero) + ' corresponde a la vocal "u"')
                else:
                    print('El numero ' + str(numero) + ' no corresponde ninguna vocal')

```

### Codigo numero 2
- Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.

```Python
# Definir una funcion 'es ascii par' y realizar la conversion correspondiente
def es_ascii_par(cadena):
    return len(cadena) == 1 and ord(cadena) % 2 == 0

# Leer una cadena de longitud 1
cadena = input("Ingresa una cadena de longitud 1: ")
resultado = es_ascii_par(cadena)

# Determinar si el coodigo ASCII de la primera letra es par
if resultado:
    print("El código ASCII de la primera letra es par.")
else:
    print("El código ASCII de la primera letra no es par.")
```

### Codigo numero 3
- Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.

```Python
# Definir una funcion 'es digito' y para evaluar si el valor que sera ingresado hace parte de la cadena
def es_digito(cadena):
    try:
        int(cadena)
        return True
    except ValueError:
        return False
    
# Leer un caracter
caracter = input("Escriba un caracter")

# Determinar si el caracter ingresado es un digito
if es_digito(caracter):
    print("El numero " + str(caracter) + " es un digito")
else:
    print("El numero " + str(caracter) +  "no es un digito")
```

### Codigo numero  4
- Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

    - Positivo: "El número x es positivo"
    -  Negativo: "El número x es negativo"
    - Cero (0): "El número x es el neutro para la suma"

```Python
# Leer un numero real
numero : float
numero = float(input("Ingrese un numero: ")) 

# Determinar si el numero es mayor, igual o menor que cero

if numero > 0:
  print("El numero "+str(numero)+" es positivo")
elif numero == 0:
  print("El número "+str(numero)+" es el neutro para la suma")
else:
  print("El numero "+str(numero)+" es negativo")
 ```

### Codigo numero 5
- Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.

```Python
# Leer 2 cooordenadas de punto y el radio de un circulo
x = int(input("Ingrese un numero en x para el punto a conocer: "))
y = int(input("Ingrese un numero en y para el punto a conocer: "))
a = int(input("Ingrese un numero en x para el centro del circulo: "))
b = int(input("Ingrese un numero en y para el centro del circulo: "))
r = int(input("Ingrese un numero para el radio del circulo: "))

# Se definen dos variables, el centro del circulo y el punto R2
C = (a, b)
R2 = (x, y)

# Determinamos si el punto R2 al circulo
if r**2 == (x - a)**2 + (y - b)**2:
    print("El punto R2 pertence al circulo")
else:
    print("El punto R2 no pertenece al circulo")
```

### Codigo numero 6
- Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.

  
```Python
#  Leer tres longitudes positivas
longitud1 = int(input("Ingrese un valor para cateto 1: "))
longitud2 = int(input("Ingrese un valor para cateto 2: "))
longitud3 = int(input("Ingrese un valor para la hipotenusa: "))

# Derminar si es posible construir el triangulo, a partir de las sumas de sus lados
if longitud1 + longitud2 > longitud3 and longitud2 + longitud3 > longitud1 and longitud3 + longitud1 > longitud2:
    print("Es posible construir el triangulo")
else:
    print("No es posible construir el triangulo")

```
