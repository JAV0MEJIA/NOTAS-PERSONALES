# NOTAS PERSONALES DE DEUDAS
# JAVIER MEJIA
archivo = open("my_notes.txt", "w")


archivo.write("Nota 1: Recordar comprar la colacion de la guagua.\n")
archivo.write("Nota 2: Partido en el Ciclon a las 4 pm el sabado.\n")
archivo.write("Nota 3: Pagar la cuenta de Netflix Disney hasta el 16 d cada mes.\n")
archivo.write("Nota 4: Pagar el resto de deudas.\n")

# Cerrar el archivo después de escribir
archivo.close()

# Abrir el archivo en modo lectura
archivo = open("my_notes.txt", "r")

# Leer el contenido del archivo línea por línea
print("DEUDAS QUE PAGAR Y OTRAS NOTAS:")
while True:
    linea = archivo.readline()
    if not linea:  # Si no hay más líneas, salir del bucle
        break
    print(linea.strip())  # Eliminar el salto de línea

# Cerrar el archivo después de leer
archivo.close()

