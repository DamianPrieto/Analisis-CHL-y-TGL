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

![Analisís de Normalidad](https://github.com/Daitiki/Analisis-CHL-y-TGL/blob/a9111fb7beb4c716004cdaac2b2b331134429575/Imagenes/Q-Q%20TGL%20Y%20CHL%20NOV.png)

En esta imagen se puede observar que para la distribucion de trigliceridos, se obtuvo una distribucion logaritmica, por lo cual su tratamiento podría ser utilizando una conversion de datos a escala logaritmica y si la desviasion estandar es muy grande considerar utilizar metodos parametricos
En cambio, para el colesterol se encontro una distribucion normal, por lo cual se utilizaran los tratamientos normales sin ninguna conversion

Para el analisís de colesterol se obtuvo el siguiente histograma.
![Distribusion de CHL](https://github.com/Daitiki/Analisis-CHL-y-TGL/blob/ab5f66dca739a323448d08414a8bac57ac0c3c95/Imagenes/CHL%20DISTRIBUCION.png)

Obteniendo un valor de referencia de: [**51.59 - 268.89**]

Para el analisís de trigliceridos se obtuvo el siguietne histograma.
![Distribusion de CHL](Imagenes/TGL%20DISTRIBUCION.png)

Utilizando un metodo no parametrico se obtuvo un valor de referencia de: [**8.56 - 221.91**]

### Comparativa con Estándares Clínicos:
- **Colesterol**: Dentro de rangos normales (NOM: <200 mg/dL deseable)
- **Triglicéridos**: **Valor promedio elevado** (NOM: <150 mg/dL normal)

##  Relevancia Clínica

Los niveles elevados de triglicéridos en población universitaria aparentemente sana sugieren:
- Posibles factores de riesgo cardiovascular tempranos
- Necesidad de programas de prevención en población joven
- Importancia de establecer valores de referencia específicos por población

## Habilidades Demostradas

- **Programación**: Python, Pandas, Matplotlib
- **Estadística Médica**: Transformaciones, intervalos de referencia, análisis de distribución
- **Visualización**: Gráficos Q-Q, histogramas, análisis de normalidad
- **Interpretación Clínica**: Contextualización de hallazgos biomédicos
