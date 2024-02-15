#Suarez Canche Isaac Moises  3SB

calificaciones = []

for i in range(100):
    fila_de_calificaciones = []
    for a in range(6):
        fila_de_calificaciones.append(float(input(f"Calificación de Alumno {i + 1} en la materia {a + 1}: ")))
    calificaciones.append(fila_de_calificaciones)

print("\nTabla de Calificaciones:")

print("{:<10} {:<10} {:<10} {:<10} {:<10} {:<10} {:<10}".format(" ", "Materia 1", "Materia 2", "Materia 3", "Materia 4", "Materia 5", "Materia 6"))

for i in range(len(calificaciones)):
    print("{:<10} {:<10} {:<10} {:<10} {:<10} {:<10} {:<10}".format(f"Alumno {i + 1}", *calificaciones[i]))

alumno_a_buscar = 95
materia_a_buscar = 5

fila_alumno = alumno_a_buscar - 1
calificacion_de_la_materia_a_buscar = calificaciones[fila_alumno][materia_a_buscar - 1]

print(f"\nEl alumno {alumno_a_buscar} tiene una calificación de {calificacion_de_la_materia_a_buscar} en la materia {materia_a_buscar}.")

# CONCLUSION:
#Al ejecutar mi programa de forma base, me di cuenta que el codigo funcionaba bien, sin embargo, el apartado del diseño hacia que este luzca como un arreglo unidimensional, lo cual no era muy estetico, por lo cual se decidio usar un arreglo tipo matriz (bidimensional) el cual hizo que este adoptara la forma de una tabla, en cuanto a la funcion del programa he de decir que me gustó ya que facilito bastante el hecho de añadir los datos y que estos estuviesen ordenados y que fuese rapido el resultado de este. La forma mas rápida que busque para que se ejecute el programa fue poniendo las materias en la parte superior, mientras que los alumnos en la parte izquierda de la matriz.
