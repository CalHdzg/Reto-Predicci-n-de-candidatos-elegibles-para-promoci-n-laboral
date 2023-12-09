Reto | Predicción de candidatos elegibles para promoción laboral


Introducción:

Con el desarrollo del reto integrarás todos los conocimientos adquiridos, cumpliendo los
siguientes objetivos:
● Genera informes automáticos para describir los datos con técnicas estadísticas y de
visualización.
● Aplica técnicas de preprocesamiento y transformación previo a la ejecución de
autoaprendizajes.
● Utiliza plataformas de AutoML para seleccionar, evaluar y optimizar modelos.
“El 80% del éxito se basa simplemente en insistir.”
- Woody Allen.


Indicaciones:

Para cualquier profesionista una promoción laboral representa un reconocimiento al esfuerzo,
capacidades y a la lealtad. Normalmente, los nuevos cargos implican mayores
responsabilidades, y retos de crecimiento profesional, pero para la empresa también es una
oportunidad importante, para cubrir determinadas vacantes con empleados que conocen la
empresa y así evitan el proceso de reclutamiento y capacitación de nuevos candidatos.
Para las grandes compañías, la identificación de los empleados adecuados para la promoción
y su preparación es un proceso complejo y hay muchos retrasos en la transición a nuevos
roles, esto ha dado origen al análisis de ciertos datos para identificar a los candidatos
elegibles en un punto de control en particular y así acelerar el ciclo de promoción.
Tu labor será generar un modelo para predecir si un empleado será promovido o no después
del proceso de evaluación, teniendo como entradas atributos en torno al rendimiento pasado
y actual del empleado junto con la demografía.
Columna Descripción
employee_id ID único para el empleado
department Departamento de empleado


Pasos:

1. Genera una libreta en Google Colab para el reto, cuya estructura esté basada en los
análisis solicitados. Descarga el archivo: EmployeePromotion.csv y guarda, en un
dataframe (info), todos sus registros.
2. Realiza un análisis exploratorio de datos con la plataforma de AutoEDA YData
Profiling. En la sección de Overview incluye una pestaña Dataset con la descripción del
conjunto de datos y tu nombre como autor. En una pestaña Variables coloca el
significado de las columnas.
3. Con la plataforma SweetViz divide el conjunto utilizando la variable gender como
booleana para comparar las características de los subconjuntos resultantes.
4. Elimina los registros con información faltante (NaN) y la columna employee_id por
no tener aportación en la predicción.

● Obtención de un modelo de ML con TPOT:

6. Codifica las variables categóricas de info con LabelEncoder.
7. Divide la matriz en conjuntos de entrenamiento y prueba (80:20), utilizando el
parámetro random_state=1 para garantizar reproducibilidad.
8. Observa la distribución de la variable objetivo is_promoted. En caso de que las
clases estén desbalanceadas, realiza over_sampling con el método SMOTE().
9. Ejecuta el autoaprendizaje utilizando el parámetro random_state y la métrica
accuracy.

● Obtención de un modelo de machine learning con PyCaret:

11. Divide la matriz en conjuntos de entrenamiento y prueba (80:20), utilizando el
parámetro random_state=1 para garantizar reproducibilidad.
12. Ejecuta el autoaprendizaje con parámetros equivalentes a los que usaste en TPOT y
optimiza el mejor modelo con la métrica accuracy.
13. Utiliza evaluate_model() para mostrar la interfaz de usuario con detalles del
modelo optimizado.
14. Verifica las métricas con el conjunto de prueba.
