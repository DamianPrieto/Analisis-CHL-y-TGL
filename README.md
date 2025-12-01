# Análisis de las concentraciones de Triglicéridos y Colesterol en estudiantes universitarios

Este estudio analiza una población estudiantil (periodo 2011-2025) con el objetivo de establecer valores de referencia para concentraciones de lípidos (Colesterol y Triglicéridos) en sujetos jóvenes aparentemente sanos.

## Metodología

Para garantizar la fiabilidad del estudio, se aplicaron los siguientes criterios de inclusión y exclusión:

### Criterios de Inclusión
* **Ayuno:** Mínimo de 8 horas.
* **IMC:** Intervalo de peso normal [18.5 - 24.9].
* **Historial Clínico:** Ausencia de enfermedades crónicas declaradas.

### Procesamiento de Datos y Limpieza
Se realizó un pre-procesamiento de datos para eliminar errores de captura y valores biológicamente implausibles. 
* **Filtrado de Outliers:** Se eliminaron registros de Triglicéridos > 400 mg/dL por considerarse patológicos (hipertrigliceridemia severa) o errores de medición, asegurando que la estadística descriptiva represente a la población "sana".

Posteriormente, se realizaron pruebas de normalidad (Gráficos Q-Q) y transformaciones logarítmicas para el análisis de distribuciones asimétricas.

## Resultados

### Análisis Descriptivo

**1. Colesterol (Distribución Normal)**
* **Media:** 160.24 mg/dL
* **Mediana:** 160.90 mg/dL
* **Desviación Estándar:** 54.33 mg/dL
* **Valor de Referencia (±2SD):** [51.59 - 268.89] mg/dL

**2. Triglicéridos (Distribución Log-Normal)**
Debido a la naturaleza asimétrica de los triglicéridos, se reportan los estadísticos recalculados tras la limpieza de outliers y transformación logarítmica inversa:

* **Media Real:** 143.62 mg/dL
* **Mediana Real:** 76.63 mg/dL (Valor más representativo de la población)
* **Moda Real:** 21.81 mg/dL
* **Desviación Estándar Real:** 227.66 mg/dL *
* **Intervalo de Referencia Robusto (Percentiles 2.5 - 97.5):** [8.56 - 221.91] mg/dL

> **Nota:** La desviación estándar de los triglicéridos es amplia debido a la asimetría positiva propia de esta variable biológica (skewness), por lo que se recomienda el uso de la **Mediana** y los **Percentiles** como valores de referencia clínica.

### Visualización y Normalidad

![Análisis de Normalidad](https://github.com/DamianPrieto/Analisis-CHL-y-TGL/raw/main/Imagenes/Q-Q%20TGL%20Y%20CHL%20NOV.png)

Como se observa en los gráficos Q-Q:
* **Colesterol:** Sigue una distribución normal teórica.
* **Triglicéridos:** Presentaban una distribución logarítmica. Se aplicó una transformación `np.log` para normalizar los datos y aplicar estadística paramétrica, confirmando la necesidad de métodos robustos.

#### Histogramas de Distribución

**Colesterol Total:**
![Distribución de CHL](https://github.com/DamianPrieto/Analisis-CHL-y-TGL/raw/main/Imagenes/CHL%20DISTRIBUCION.png)

**Triglicéridos:**
![Distribución de TGL](https://github.com/DamianPrieto/Analisis-CHL-y-TGL/raw/main/Imagenes/TGL%20DISTRIBUCION.png)

## Comparativa con Estándares Clínicos (NOM)

* **Colesterol:** La media poblacional (160 mg/dL) se encuentra dentro de los rangos deseables (<200 mg/dL).
* **Triglicéridos:** Tras el refinamiento de datos, la **mediana (76.63 mg/dL)** se ubica cómodamente dentro del rango normal (<150 mg/dL). Sin embargo, el límite superior del intervalo de referencia (221.91 mg/dL) sugiere que una fracción de la población estudiantil, aun con IMC normal, presenta niveles limítrofes o altos.

## Relevancia Clínica

El estudio demuestra que, aunque la mediana de la población universitaria es saludable, existe una dispersión significativa hacia valores altos en triglicéridos. Esto resalta la importancia de:
1.  No confiar únicamente en el IMC como indicador de salud metabólica.
2.  Considerar tamizajes de perfil lipídico incluso en adultos jóvenes aparentemente sanos.

## Habilidades Técnicas Demostradas

* **Data Science:** Limpieza de datos (Data Cleaning), detección de outliers, transformación de variables (Log-Transform).
* **Stack Tecnológico:** Python, Pandas, NumPy, Matplotlib, Seaborn, Statsmodels.
* **Bioestadística:** Interpretación de distribuciones normales vs. no paramétricas, cálculo de intervalos de referencia clínicos.
