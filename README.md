# Proyecto-2
A continuación, los dos programas correspondientes al módulo 2 del curso 

Ambos códigos estan hechos con estructuras de control if, elif, else y while
En el caso del primero esta encapsulado en un while, a diferencia del segundo que solo lo utiliza para verificar que no se ingrese un valor igual a cero.
A lo largo de este segundo módulo del bootcamp, he comprendido mejor el funcionamiento de pyhton y sus diferentes estructuras. Por otro lado he conocido otras de sus muchas herramientas como lo son los diccionarios, listas, conjuntos y demás estructuras que fácilitan la creación, edición y gestión de datos.

Adjunto el link al archivo python: C:\Users\Monse\OneDrive\Documentos\Python\MONSERRAT_MAZA_proyectoM2.py

Adjunto el código con los respectivos comentarios que lo describen:
#Reto 1
#El siguiente programa mide la longitud de la frase ingresada

#A continuación,se encapsula el código dentro de un bucle while para permitir múltiples intentos hasta que se ingrese una frase con la longitud correcta
while True:    
 frase = input("Ingrese una frase: ") #Se declara la variable frase
 longitud_frase = len(frase)
 print("La longitud de la frase es:", longitud_frase)
#La frase que el programa detectará coomo correcta tendrá una longitud entre 4 y 8 letras
 if longitud_frase < 4:
    print(f"Hacen falta letras.Solo hay {longitud_frase} letras.")
 elif longitud_frase > 8:
    print(f"Sobran letras.Tiene {longitud_frase} letras.")
#Al tener una palabra con longitud entre 4 y 8 letras, el else se encargará 
#de mostrar el mensaje de éxito y finalizar el programa
 else:
    print(f"La longitud de la frase es correcta, tiene {longitud_frase} letras.")
    print("La palabra correcta fue ingresada, fin del programa.")
    break 
 
 #Reto 2
#Encuentra a que cuadrante pertenecen las coordenadas ingresadas
#Se solicita al usuario que ingrese las coordenadas x e y
x = float(input("Ingrese la coordenada x: "))
while x==0: #asegura que "x" no sea igual a 0
    print("Error: La coordenada 'x' no puede ser cero. Inténtelo de nuevo.")
    x = float(input("Ingrese la coordenada x: "))
y = float(input("Ingrese la coordenada y: "))
while y==0: #asegura que "y" no sea igual a 0
    print("Error: La coordenada 'y' no puede ser cero. Inténtelo de nuevo.")
    y = float(input("Ingrese la coordenada y: "))
#Se determina a que cuadrante pertenecen las coordenadas ingresadas
if x > 0 and y > 0:
    print("El punto se encuentra en el cuadrante I.")
elif x < 0 and y > 0:
    print("El punto se encuentra en el cuadrante II.")
elif x < 0 and y < 0:
    print("El punto se encuentra en el cuadrante III.")
elif x > 0 and y < 0:
    print("El punto se encuentra en el cuadrante IV.")
else:
    print("Las coordenadas están en el origen o en uno de los ejes.")
