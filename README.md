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
