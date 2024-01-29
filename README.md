# RiesgoRelativo

# Contexto

Riesgo relativo bancario 

En el contexto reciente, la disminución de las tasas de interés en el mercado ha desencadenado un aumento notable en la demanda de solicitudes de crédito. Los clientes ven una oportunidad favorable para financiar compras importantes o consolidar deudas existentes, lo que ha llevado a una afluencia de solicitudes de préstamo en el banco “Super Caja”. El equipo de análisis de crédito del banco está enfrentando una carga de trabajo abrumadora debido al análisis manual requerido para cada solicitud de préstamo de clientes individuales. Esta metodología manual ha resultado en un proceso ineficiente y demorado, lo que ha afectado negativamente la eficacia y la rapidez con la que se procesan las solicitudes de préstamo. La situación se vuelve más crítica debido a la creciente preocupación por la tasa de incumplimiento (default), un problema que está afectando cada vez más a la industria financiera, aumentando la presión sobre los bancos para identificar y mitigar los riesgos asociados con el crédito.

Con el fin de abordar este desafío, la propuesta es la automatización del proceso de análisis utilizando técnicas avanzadas de análisis de datos, con el objetivo de mejorar la eficiencia, la precisión y la rapidez en la evaluación de las solicitudes de crédito. Además, el banco ya tiene una métrica para identificar a los clientes con pagos atrasados, lo que podría ser una herramienta valiosa para integrar en la clasificación de riesgo dentro del nuevo sistema automatizado.

El objetivo del análisis es armar un score crediticio a partir de un análisis de datos y la evaluación del riesgo relativo que pueda clasificar a los solicitantes en diferentes categorías de riesgo basadas en su probabilidad de incumplimiento. Esta clasificación permitirá al banco tomar decisiones informadas sobre a quién otorgar crédito, reduciendo así el riesgo de préstamos no reembolsables. Además, la integración de la métrica existente de pagos atrasados fortalecerá la capacidad del modelo para identificar riesgos, lo que en última instancia contribuirá a la solidez financiera y la eficiencia operativa del banco.

# Base de Datos

Se cuenta con una base de datos con las siguientes caracteristicas:
- 4 tablas llamadas User Info, Loans Outstanding, Loans Details y Default.
- Volumen de 36000 y 305335 lineas.
- Cuentan con 16 variables en total.

# Proceso de Limpieza y Preparación

Durante el proceso de limpieza se eliminaron las lineas con valores nulos en variables importantes como user_id y loan_id.
Para los datos nulos o fuera de alcance estos fueron eliminados, sujetos al limite de no borrar mas de un 1% del total de datos.
Se dejaron las variables de texto sin caracteres especiales o numeros donde no corresponda.

# Análisis Exploratorio 

A continuación se muestra el analisis exploratorio de los datos.

![image](https://github.com/FeerOT/RiesgoRelativo/assets/150949526/d38f7aeb-8b62-4b6a-9209-c7a8d2f1fa20)

![image](https://github.com/FeerOT/RiesgoRelativo/assets/150949526/02a12eae-8948-4cdb-8ed1-e563702d67f6)

![image](https://github.com/FeerOT/RiesgoRelativo/assets/150949526/4cff1150-2ca6-4f38-aa29-82ea109eed98)

# Técnicas de Análisis Utilizadas

Durante el proceso de analisis se utilizaron las siguientes tecnicas: 
- Calculo de Riesgo Relativo
- Validación de Hipotesis
- Segmentación
- Regresión Logistica
- Correlación

# Resultados y Conclusiones

Los principales resultados y conclusiones obtenidos fueron:
- Se identificaron patrones de comportamiento
- Se identificaron cuartiles de riesgos
- Se establecieron recomendaciones para la el banco sobre garantias, tolerancias, etc.

# Herramientas
https://console.cloud.google.com/bigquery?project=riesgo-relativo-406716&ws=!1m0
