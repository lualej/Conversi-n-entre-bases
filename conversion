def base_a_decimal(numero, baseM):
    digitos = '0123456789ABCDEF'
    decimal_resultado = 0
    longitud = len(numero)

    for i, digito in enumerate(numero):
        valor = digitos.index(digito)
        decimal_resultado += valor * (baseM ** (longitud - i - 1))
    
    return decimal_resultado


def decimal_a_base(decimal_resultado, baseN):
    digitos = '0123456789ABCDEF'
    resultado = ""

    while decimal_resultado > 0:
        residuo = decimal_resultado % baseN
        resultado = digitos[residuo] + resultado
        decimal_resultado //= baseN
     
    return resultado

def decimal_a_binario(decimal_resultado):
    if baseM == 2:
      return numero
    
    if decimal_resultado == 0:
        return '0'
    
    binario_resultado = ""
    while decimal_resultado > 0:
        residuo = decimal_resultado % 2
        binario_resultado = str(residuo) + binario_resultado
        decimal_resultado //= 2
    
    return binario_resultado

def binario_a_ascii(binario_resultado):
    # Asegurarse de que binario_resultado solo contenga 0 y 1
    binario_resultado = binario_resultado.replace(" ", "")
    
    # Rellenar con ceros a la izquierda si la longitud no es múltiplo de 8
    while len(binario_resultado) % 8 != 0:
        binario_resultado = "0" + binario_resultado
    
    decodificado = ""
    
    for i in range(0, len(binario_resultado), 8):
        binario_grupo = binario_resultado[i:i+8]
        numero_decimal = int(binario_grupo, 2)
        letra = chr(numero_decimal)
        decodificado += letra
    
    return decodificado


# comienzo pidiendole al usuario que ingrese los datos que requerimos
print("Bienvenido al programa de conversion entre bases")
numero = input("Ingresa el numero que deseas convertir: ").upper()
baseM = int(input("Ingrese la base del numero ingresado anteriormente: "))
baseN = int(input("Ingrese la base a la que desea convertir el numero: "))

if baseM <= 1 or baseM > 16:
    print("La base ingresada es invalida(Recuerde: Debe ser una base entre 2 y 16)")
else:
    resultado = decimal_a_base(base_a_decimal(numero, baseM), baseN)
    print(f"El número en base {baseM} {numero} es equivalente a base {baseN}: {resultado}")

decimal_resultado = base_a_decimal(numero, baseM)
binario_resultado = decimal_a_binario(decimal_resultado)
print(f"El número en binario: {binario_resultado}")

binario_resultado = decimal_a_binario(decimal_resultado)
decodificado = binario_a_ascii(binario_resultado)

decodificado = binario_a_ascii(binario_resultado)
unicode_decodificado = decodificado.encode('utf-8').decode('unicode-escape')
print(f"El binario decodificado es: {unicode_decodificado}")
decodificado = binario_a_ascii(binario_resultado)

