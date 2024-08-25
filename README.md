# Rendimiento de estudiantes de secundaria
# Abstract
## Resumen

Este conjunto de datos contiene información de más de 2000 estudiantes de secundaria; en él se detallan sus hábitos de estudio, las actividades extracurriculares que realizan, el desempeño académico y el compromiso de sus padres, entre otras. 

El rendimiento académico se mide a través del GPA (Grade Point Average según sus siglas en inglés) y está influenciado por la información detallada al principio. 

Se clasifica a los estudiantes en cinco categorías basadas en su GPA: 
* 0 para 'A' (GPA ≥ 3.5)
* 1 para 'B' (3.0 ≤ GPA < 3.5)
* 2 para 'C' (2.5 ≤ GPA < 3.0)
* 3 para 'D' (2.0 ≤ GPA < 2.5)
* 4 para 'F' (GPA < 2.0)

## Hipótesis

***Hipótesis 1 - Influencia del apoyo parental en el éxito académico:*** 
Los estudiantes que reciben un mayor apoyo de sus padres, tienden a obtener un GPA significativamente más alto. O sea, el apoyo parental tiene una influencia positiva en el éxito académico de los estudiantes de secundaria.

***Hipótesis 2 - Impacto de la participación en actividades extracurriculares en el rendimiento académico:***
Los estudiantes que participan en actividades extracurriculares (como ser deportes o música) tienen un mejor rendimiento académico (GPA) en comparación con aquellos que no participan de tales actividades.

***Hipótesis 3 - Incidencia del nivel educativo de los padres en la cantidad de faltas de los estudiantes:***
Los estudiantes cuyos padres tienen un mayor nivel educativo tienden a tener menos ausencias.

## Objetivos

* Analizar las relaciones entre variables socioeconómicas y educativas (como apoyo parental, nivel educativo de los padres, participación en actividades extracurriculares) y su influencia en el rendimiento académico (GPA) y la asistencia escolar.
* Determinar los factores clave que afectan positivamente o negativamente el éxito académico de los estudiantes, para identificar áreas de mejora y oportunidades de intervención.
* Crear modelos estadísticos que puedan predecir el rendimiento académico y la asistencia escolar en función de las variables analizadas, con el fin de proporcionar herramientas para la toma de decisiones en el ámbito educativo.

## Impacto

* Mejora de Políticas Educativas
* Desarrollo de Programas de Intervención
* Optimización de Recursos Educativos

## Conclusiones preliminares

* La edad promedio de los estudiantes es de aproximadamente 16.47 años, con un rango de entre 15 y 18 años.
* La distribución de género está casi equilibrada, con un promedio cercano a 0.51 (donde 0 y 1 representan los dos géneros codificados en el dataset).
* La mayoría de los estudiantes son caucásicos (caucásico = 0), ya que tanto la mediana como el primer cuartil están en 0.
* El nivel educativo promedio de los padres está alrededor de 1.75, en una escala de 0 a 4. La mediana es 2, lo que sugiere que muchos padres tienen un nivel educativo intermedio.
* El apoyo parental promedio es 2.12, en una escala de 0 a 4, lo que indica un nivel moderado de apoyo parental entre los estudiantes.
* Los estudiantes dedican un promedio de aproximadamente 9.77 horas a la semana al estudio, con un rango que varía desde casi 0 horas hasta casi 20 horas.
* El número de ausencias promedio es de 14.54 días, con un rango entre 0 y 29 días. Esto sugiere que algunos estudiantes tienen una asistencia muy irregular.
* Aproximadamente el 38% de los estudiantes participan en alguna actividad extracurricular: 30% de los estudiantes participan en deportes, 20% de los estudiantes participan en actividades relacionadas con la música y 15.7% de los estudiantes participan en actividades de voluntariado.
* El promedio de calificaciones (GPA) es de 1.91 en una escala de 0 a 4. La desviación estándar del GPA es relativamente alta (0.92), lo que indica una considerable variabilidad en el rendimiento académico entre los estudiantes. 
* Tambien se observa en la columna de GradeClass que la mediana es 4 (F).

# Gráficos

Se realizan distintos tipos de gráficos que permiten una mejor comprensión y análisis del dataset y de esta forma poder identificar patrones, tendencias y relaciones entre variables

- ***Gráfico de líneas:*** Relación entre el Apoyo Parental y el GPA (Matplotlib)
- ***Boxplot:*** Distribución del GPA según el Nivel de Apoyo Parental (Seaborn)
- ***Gráfico de barras:*** Distribución de Participación en Actividades Extracurriculares (Seaborn)
- ***Gráfico de líneas mejorado:*** Media del GPA por Actividad Extracurricular (Matplotlib)
- ***Histograma:*** Distribución de las Faltas por Nivel Educativo de los Padres (Matplotlib)
- ***Gráfico de puntos:*** Relación entre Faltas, GPA y Nivel Educativo de los Padres (Seaborn)
- ***Mapa de Calor de Correlaciones***(Seaborn)

# Insights relevantes

***Hipótesis 1: Influencia del Apoyo Parental en el Éxito Académico:***
La correlación entre el apoyo parental y el GPA es positiva pero débil, con un valor de 0.19, lo que indica que, aunque el apoyo parental influye en el rendimiento académico, su impacto es limitado. Un aumento máximo en el apoyo parental solo mejora el GPA en 0.6 puntos, lo que sugiere que otros factores juegan un papel más significativo en el éxito académico de los estudiantes. Por lo tanto, aunque el apoyo parental es beneficioso, no es suficiente por sí solo para lograr un rendimiento académico elevado. 

***Hipótesis 2: Impacto de la Participación en Actividades Extracurriculares en el Rendimiento Académico***
La participación en actividades extracurriculares muestra una correlación muy débil con el GPA. Aunque los estudiantes que participan en música tienen una media de GPA ligeramente superior (2.02) en comparación con los que no participan en ninguna actividad (1.84), la diferencia no es lo suficientemente significativa como para sugerir que la participación en actividades extracurriculares mejora sustancialmente el rendimiento académico. La hipótesis de que la participación en actividades extracurriculares impacta significativamente en el rendimiento académico no es fuertemente respaldada por estos datos.
Hay que considerar que hay un número significativo de estudiantes que no participan en ninguna actividad, esto podría sugerir que hay barreras que impiden su participación, como falta de interés, acceso limitado, o carga académica. Este dato podría ser útil para las instituciones educativas al diseñar programas que fomenten una mayor participación.

***Hipótesis 3: Incidencia del Nivel Educativo de los Padres en la Cantidad de Faltas***
La media de ausencias es alta, lo que podría correlacionarse con el bajo rendimiento académico observado, pero no parece estar fuertemente influenciado por el nivel educativo de los padres. Como pasa con las otras hipótesis, tiene cierta influencia pero no es determinante
