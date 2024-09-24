# daniel-arguijo_3-w
PR_EN CLASE "NUMERO SECRETO 

(" ") 
("jose daniel arguijo torres 3-w")
(" ")

import random
# Generar un número aleatorio entre 1 y 100
numero_secreto = random.randint(1, 100)#indica el numero secreto 

# Inicializar variables
intentos = 0#tenemos oportunidad de muchos intentos 
adivinado = False#adivinar el numero correcto 

print("¡Bienvenido al juego de adivinanza!")#nos da la bienvenida al programa 
print("He seleccionado un número entre 1 y 100. ¡Intenta adivinarlo!")#seleccionar un numero para adivinar el correcto 

while not adivinado:
    try:
        # Pedir al usuario que ingrese un número
        guess = int(input("Introduce tu número: "))#poder introducir el primer numero 
        intentos += 1 

        if guess < numero_secreto:#adivinar el numero secreto 
            print("Demasiado bajo. Intenta de nuevo.")#intentar de nuevo el escoger el numero 
        elif guess > numero_secreto:#poder introducir el primer numero
            print("Demasiado alto. Intenta de nuevo.")#intentar de nuevo el escoger el numero 
        else:#programa finalizado 
            adivinado = True
            print(f"¡Felicidades! Adivinaste el número {numero_secreto} en {intentos} intentos.")#te felicita por adivinar el numero corecto 
    except ValueError:
        print("Por favor, introduce un número válido.")#el numero fue valido 

        
![image](https://github.com/user-attachments/assets/c76af22e-1b58-4dd5-988d-6336cd764249)
