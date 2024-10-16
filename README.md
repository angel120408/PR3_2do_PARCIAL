# Codigo #1 De la Pr3 Por Ramirez Torres Angel Manuel De 3°W
- Guardar en una variable el diccionario {'Euro':'€', 'Dollar':'$', 'Yen':'¥'}, 
El usuario debe meter una divisa y debe mostrar el símbolo o un mensaje de que la divisa no está en el diccionario.


print(" ")# Sirve para que no se vea amontonado el codigo 
print("Ramirez Torres Angel Manuel 3°W")#Nombre del alumno
print("Numer de control: 1206")#numero de control
print("-INSTRUCCIONES-")#Nos muestra a continuacion las instrucciones
print("Guardar en una variable el diccionario {'Euro':'€', 'Dollar':'$', 'Yen':'¥'}, ")
print("El usuario debe meter una divisa y debe mostrar el símbolo o un mensaje de que la divisa no está en el diccionario.")
print(" ")# Sirve para que no se vea amontonado el codigo 

def obtener_simbolo(divisa):
    # Diccionario que mapea nombres de divisas a sus símbolos
    divisas = {'Euro': '€', 'Dollar': '$', 'Yen': '¥'}
    
    # Retorna el símbolo correspondiente a la divisa ingresada
    # Si la divisa no está en el diccionario, retorna un mensaje de error
    return divisas.get(divisa, "La divisa no está en el diccionario.")
print("NOTA: INGRESA LA DIVISA TAL CUAL ESTA ESCRITA")
print(" ")
# Solicitar al usuario que ingrese una divisa
entrada = input("Introduce una divisa (Euro, Dollar, Yen): ")

# Llamar a la función y almacenar el resultado
resultado = obtener_simbolo(entrada)

# Mostrar el resultado al usuario
print(resultado)


![image](https://github.com/user-attachments/assets/8c8446d3-5bbb-451a-8a6c-689fe3c3e778)
![image](https://github.com/user-attachments/assets/20043a42-e26a-4a64-9e76-0b5689021039)


# Codigo #2 De la Pr3 Por Ramirez Torres Angel Manuel De 3°W
- Preguntar al usuario nombre, edad, dirección y teléfono y lo guarde en un diccionario. Después debe mostrar por pantalla el mensaje <nombre> tiene <edad> años, vive en <dirección> y su número de teléfono es <teléfono>

print(" ")# Sirve para que no se vea amontonado el codigo 
print("Ramirez Torres Angel Manuel 3°W")#Nombre del alumno
print("Numer de control: 1206")#numero de control
print("-INSTRUCCIONES-")#Nos muestra a continuacion las instrucciones
print("Preguntar al usuario nombre, edad, dirección y teléfono y lo guarde en un diccionario. ")
print("Después debe mostrar por pantalla el mensaje ")
print("<nombre> ")
print("tiene <edad> años, ")
print("vive en <dirección> ")
print("y su número de teléfono es <teléfono>")
print(" ")# Sirve para que no se vea amontonado el codigo 

class Usuario:
    def __init__(self, nombre, edad, direccion, telefono):
        # Inicializar los atributos del usuario con la información proporcionada
        self.nombre = nombre      # Nombre del usuario
        self.edad = edad          # Edad del usuario
        self.direccion = direccion  # Dirección del usuario
        self.telefono = telefono    # Número de teléfono del usuario

    def mostrar_info(self):
        # Retornar una cadena para describir la información del usuario 
        return (f"{self.nombre} tiene {self.edad} años,\n"  #nombre y edad
                f"vive en {self.direccion} y su número de teléfono es {self.telefono}.")  #dirección y teléfono

# Solicitar la información al usuario
nombre = input("Introduce tu nombre: ")        # Pregunta por el nombre
edad = input("Introduce tu edad: ")            # Pregunta por la edad
direccion = input("Introduce tu dirección: ")   # Pregunta por la dirección
telefono = input("Introduce tu número de teléfono: ")  # Pregunta por el número de teléfono

usuario = Usuario(nombre, edad, direccion, telefono)

# Mostrar la información del usuario 
print(usuario.mostrar_info())  # Imprime la información del usuario 


![image](https://github.com/user-attachments/assets/c252d6ab-c6f8-4c68-8e4e-f29aab69788b)
![image](https://github.com/user-attachments/assets/6697f629-ffe1-4d6c-8458-f47dd46e31fa)



# Codigo #3 De la Pr3 Por Ramirez Torres Angel Manuel De 3°W
- Guardar en un diccionario precios de las frutas en una matriz, luego preguntar al usuario por fruta, un número de kilos mostrar el precio de ese número de kilos de fruta.

print(" ")# Sirve para que no se vea amontonado el codigo 
print("Ramirez Torres Angel Manuel 3°W")#Nombre del alumno
print("Numer de control: 1206")#numero de control
print("-INSTRUCCIONES-")#Nos muestra a continuacion las instrucciones
print("Guardar en un diccionario precios de las frutas en una matriz, luego preguntar al usuario por ")
print("fruta,")
print("un número de kilos")
print("mostrar el precio de ese número de kilos de fruta.")
print("Si no está la fruta no está en el diccionario debe mostrar un mensaje informando eso mismo")
print(" ")# Sirve para que no se vea amontonado el codigo 


def calcular_precio(fruta, kilos):

    # Diccionario que contiene los precios de las frutas por kilo
    precios_frutas = {
        'manzana': 3.0,  # Precio por kilo de manzana
        'plátano': 2.5,  # Precio por kilo de plátano
        'naranja': 4.0,  # Precio por kilo de naranja
        'fresa': 5.0     # Precio por kilo de fresa
    }

    # Verificar si la fruta ingresada por el usuario está en el diccionario de precios
    if fruta in precios_frutas:
        # Si la fruta está disponible, calcular el precio total
        precio_total = precios_frutas[fruta] * kilos
        # Da un mensaje de la cantidad de kilos y el precio total
        return f"El precio de {kilos} kilos de {fruta} es: ${precio_total:.2f}"
    else:
        # Si la fruta no está en el diccionario, da un mensaje de error
        return "La fruta no está en el diccionario."

# Solicitar el nombre de la fruta
fruta = input("Introduce el nombre de la fruta (manzana, plátano, naranja, fresa): ")

# Solicitar el número de kilos que desea comprar
kilos = float(input("Introduce el número de kilos: "))

#calcular el precio y almacenar el resultado
resultado = calcular_precio(fruta, kilos)

print(" ")
# Mostrar el resultado al usuario en la consola
print(resultado) 


![image](https://github.com/user-attachments/assets/44eadcc8-b118-4b00-8003-a5073216974e)
![image](https://github.com/user-attachments/assets/d9260553-e574-4e2d-9813-16253f358e42)
![image](https://github.com/user-attachments/assets/d9b4f234-12fc-4d23-b5eb-3984035d0d0d)
![image](https://github.com/user-attachments/assets/ed76a3a0-49bb-4969-8726-813ae3128af3)


