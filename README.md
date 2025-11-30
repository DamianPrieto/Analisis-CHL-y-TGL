# Analisis de las concentraciones de Trigliceridos y Colesterol en estudiantes universitarios

En este estudio se utilizo una poblacion de estudiantes desde el 2011 hasta el 2025, con el objetivo de encontrar valores de referencias de las concentraciones de lipidos (Colesterol y Trigliceridos).

# Metodologia 

Se filtraron los datos para excluir los estudiantes que no cumplieran con los siguietnes requisitos:
- Un ayuno minimo de 8 horas
- IMC en un intervalo de [18.5 - 24.9]
- No tenga enfermedades

Posterior a esto se realizaron distintas pruebas estadisticas como lo son graficas Q-Q y metodos no parametricos para un mejor tratamiento de los datos y así encontrar los valores de referencia de la poblacion estudiada.

# Resultados

Los resultados principales que se encontraron fueron los siguientes
- Para colesterol
Media: 160.24
Desviación estándar: 54.33
Mediana: 160.90
Moda: 146.4
- Para trigliceridos
Media: 226.50
Mediana: 104.08
Moda: 21.98
Desviación estándar: 437.78

![Comparativa de graficas Q-Q](Imagenes/Q-Q TGL Y CHL NOV.png)

En esta imagen se puede observar que para la distribucion de trigliceridos, se obtuvo una distribucion logaritmica, por lo cual su tratamiento podría ser utilizando una conversion de datos a escala logaritmica y si la desviasion estandar es muy grande considerar utilizar metodos parametricos
En cambio, para el colesterol se encontro una distribucion normal, por lo cual se utilizaran los tratamientos normales sin ninguna conversion


