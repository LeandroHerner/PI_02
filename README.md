# Análisis de Siniestros Viales en Buenos Aires

**Alumno:** HERNER LEANDRO GABRIEL

## Introducción
El presente proyecto aborda el análisis de datos vinculados a la problemática de los siniestros viales en la Ciudad Autónoma de Buenos Aires. Se parte de datos proporcionados por el Observatorio de Movilidad y Seguridad Vial de la Secretaría de Transporte de la Ciudad Autónoma de Buenos Aires comprendidos entre los años 2016 y 2021. El dataset proporcionado consta de un archivo en formato xlsx que contiene las hojas ‘Hechos’ y ‘Víctimas’, con sus respectivos diccionarios de datos. Se utilizan como indicadores los datos de mortalidad vinculados a siniestros viales a fin de comprender, identificar patrones y generar información que sea de utilidad para el desarrollo y aplicación de estrategias preventivas, que permitan mejorar la seguridad vial y la vida de los habitantes de la ciudad. Estos mismos datos también se utilizan para evaluar el impacto de las medidas implementadas.

## Exploratory Data Analysis (EDA)

Aquí se analiza el dataset para buscar datos faltantes, repetidos, errores, problemas de codificación, etc. Una vez que se tiene el dataset limpio y completo, se procede a buscar relaciones entre las columnas que puedan aportar información de interés. Algunas de las relaciones que se pensaron útiles y se exploraron a fin de identificar posibles tendencias fueron:
- Víctimas de Siniestros Viales por Comuna.
- Distribución de tipo de víctima (peatón, moto, auto, etc.) por Comuna.
- Distribución de siniestros por tipos de Calle (Avenida, Autopista, Calle).
- Total de siniestros viales por Año.
- Distribución de Siniestros por Edades.
- Distribución de víctimas en siniestros según rol (conductor, pasajero, peatón, ciclista).
- Distribución de víctimas según tipo de movilidad (moto, auto, peatón, bicicleta).
- Distribución de víctimas por género.
- Frecuencia de Siniestros Viales por Dirección.
- Distribución por rango etario y rol de la víctima.
- Distribución de siniestros según día de la semana.

## Dashboard en Power BI

### Portada

![Screenshot](/ruta/al/portada.png)

### Página 1 - Análisis Geográfico/Temporal

En esta página se muestra un análisis de las víctimas fatales de siniestros viales realizado por año por ubicación geográfica según comuna. En el margen izquierdo se dispone de un tablero interactivo que permite seleccionar un año o rango de años a la vez que una comuna o rango de comunas. De esta manera, es posible cruzar datos temporales y espaciales para su visualización y análisis. Los elementos visuales utilizados incluyen:
- Tarjeta de víctimas Totales.
- Mapa de siniestros viales por comuna.
- Gráfico de barras de víctimas por comuna.
- Gráfico de barras de víctimas según día de la semana.
- Gráfico de dona de víctimas por tipo de calle.

![Screenshot](/ruta/al/screenshot.png)

### Página 2 - KPI 1

En esta página se realiza un análisis de los datos en función del KPI número 1: ‘Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior.’ Se incluye un gráfico de barras que permite visualizar las víctimas totales por semestre desde el año 2016 hasta el año 2021 y una tabla interactiva que permite visualizar las métricas por cada semestre. Las métricas por semestre incluyen:
- Tasa de homicidios por siniestros viales por semestre.
- Variación porcentual de la tasa de homicidios por siniestros viales con respecto al semestre anterior. (Se indica en esta métrica si se alcanza el KPI objetivo y se señala cuántos puntos por arriba o por abajo del mismo se encuentra la métrica).

![Screenshot](/ruta/al/screenshot2.png)

### Página 3 - KPI 2

En esta página se realiza un análisis de los datos en función del KPI número 2: ‘Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.’ Se incluye un gráfico de barras que permite visualizar las víctimas totales por año de accidentes de moto desde el año 2016 hasta el año 2021 y una tabla interactiva que permite visualizar las métricas anuales. Las métricas anuales incluyen:
- Variación porcentual de accidentes mortales en moto con respecto al año anterior (Se indica en esta métrica si se alcanza el KPI objetivo y se señala cuántos puntos por arriba o por abajo del mismo se encuentra la métrica).

![Screenshot](/ruta/al/screenshot3.png)

### Página 4 - KPI 3

En esta página se realiza un análisis de los datos en función del KPI número 3: ‘Reducir en un 10% la media mensual de accidentes mortales de peatones, en CABA, con respecto al año anterior.’ Este KPI es de elaboración propia y surge a raíz de identificar en el EDA que los peatones constituyen un gran porcentaje de las víctimas fatales involucradas en siniestros viales y, por tanto, resulta relevante entender estos hechos a fin de proponer estrategias que contribuyan a mantener seguros a los habitantes de la ciudad que deciden movilizarse a pie. A continuación, se incluyen dos gráficos realizados en el EDA que fueron el puntapié para la generación de este KPI:

![Screenshot](/ruta/al/screenshot4a.png)

![Screenshot](/ruta/al/screenshot4b.png)

A fin de analizar los siniestros viales que involucran peatones, en primera instancia, se filtró a las víctimas totales (peatones) por año. Este dato se incluye en la página del dashboard en un gráfico de barras que incluye los años comprendidos entre el año 2016 y el año 2021. Se utilizó como indicador la media mensual de accidentes fatales de peatones. Dicha métrica se calculó como: Víctimas totales para un año dado / 12 meses. En el dashboard se incluye una tabla interactiva que permite visualizar este indicador para cada año. Finalmente, se incluye la variación porcentual de accidentes mortales de peatones con respecto al año anterior (Se indica en esta métrica si se alcanza el KPI objetivo y se señala cuántos puntos por arriba o por abajo del mismo se encuentra la métrica).

![Screenshot](/ruta/al/screenshot4c.png)
