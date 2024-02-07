# 🇮🇹 Studio della pandemia di COVID-19 in Italia😷

![](https://img.shields.io/badge/python-3.10+-sucess?style=for-the-badge&logo=python)![](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)![](https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white)![](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

> [!NOTE]
> [![Static Badge](https://img.shields.io/badge/build-Analisis_COVID_19-brightgreen?logo=deepnote&label=Presentación%20ejecutiva%20en%20deepnote.com&color=%23AFEEEE&style=for-the-badge)](https://deepnote.com/@lucel-dasilva/Analisis-COVID-19-56551004-f932-4da5-b5ad-7bb31d32774e)


## Objetivo 👈
Analizar los datos relacionados con el COVID-19 y presentar insights a través de visualizaciones que respondan a las siguientes preguntas clave de __`Ministero della Salute`__, la entidad gubernamental responsable de la gestión de la salud en Italia


## Conociendo a los datos 🗺️

Del dataframe de __World Health Organization__
| Columna | Tipo de Dato |Descripción | 
| :---: | :---: | :---| 
| `Date_reported` | datetime64[ns] | Fecha del reporte |
| `Country_code` | String | Código identificatorio universal del país |
| `Country` | String | Nombre oficial del país |
| `New_cases` | Integer | Casos nuevos por registro |
| `Cumulative_cases` | Integer | Casos acumulados a partir del registro anterior con el actual |
| `New_deaths` | Integer | Nuevas muertes por registro |
| `Cumulative_deaths` | Integer | Muertes acumuladas a partir del registro anterior con el actual |
| `lethality_rate` | Float | Porcentaje entre `Cumulative_deaths` y `Cumulative_cases` |

Del dataframe de __United Nations__
| Columna | Tipo de Dato |Descripción | 
| :---: | :---: | :--- | 
| `Country_code` | String | Código identificatorio universal del país |
| `Total_Population` | Integer | Población total del país |
| `Male_Population` | Integer | Población masculina del país |
| `Female_Population` | Integer | Población femenina del país |
| `Population_Density` | Integer | Densidad poblacional del país |
| `Life_Expectancy` | Float | Esperanza de vida del país |

## Problema de Negocio 

Una entidad gubernamental responsable de la gestión de la salud de Italia (pais seleccionado) enfrenta el desafío de comprender y analizar la propagación del COVID-19 para tomar decisiones informadas y eficaces en la gestión de la pandemia.
Para ello, se analizan los datos relacionados con el COVID-19 y se presentan insights a través de visualizaciones que respondan a las siguientes preguntas clave:

Preguntas

1. ¿Cómo ha evolucionado el COVID-19 en Alemania en comparación con el impacto observado a nivel mundial?

2. ¿Cuál ha sido la evolución de los nuevos casos diarios reportados de COVID-19 en Alemania a lo largo del tiempo?

3. ¿Cuál es la evolución del índice de letalidad del COVID-19 en el país, comparado con los países con los índices históricos más elevados?

4. Desde una perspectiva demográfica, ¿cuáles son las características que tienen un mayor impacto en el índice de letalidad en un país?

## Resultados
1. ¿Cómo ha evolucionado el Covid-19 en el país en comparación con el impacto observado a nivel global?

Italia se encuentra en la posición 9 de los países con mayores casos de COVID acumulados hasta la fecha, ha experimentado un crecimiento moderado pero constante de los casos de COVID-19 en comparación con otros países. Si bien en el año 2022 hubo un aumento considerable de casos diarios, fue menor que en lo observado en los otros países del top 5

2.¿Cuál ha sido la evolución de los nuevos casos diarios reportados de Covid-19 en el país a lo largo del tiempo?

Los datos indican que en el año 2022 es donde se reportan una mayor cantidad de casos. Observándose varios picos principalmente en Enero que éste duró hasta fines de Febrero, luego gradualmente picos menores en las quinceras de Julio y Octubre.

3. ¿Cuál es la evolución del índice de letalidad del Covid-19 en el país, comparado con los países con los índices históricos más elevados?

Italia llega a tener su pico de letalidad fue de 12.47%, para septiembre del 2020. Disminuyendo en diciembre del mismo año a un 3.5% llegando a valores de menos de 1,5% a partir de febrero del 2022.

4. Desde una perspectiva demográfica, ¿cuáles son las características que tienen un mayor impacto en el índice de letalidad de un país?

Aunque en primera instancia estudiando la regresión del Random Forest muestra que la población es una característica de alto impacto la verdad con la matriz de correlación concluye que más sería la densidad poblacional una característica importante descartando la cantidad de población del país con sus respectivas cifras entre sexos.

Podemos decir que la esperanza de vida Life_Expectancy y la densidad poblacional Population_density son las características que tienen un mayor impacto en el índice de letalidad.

## Conclusiones
Cabe destacar que durante el 2020 registrando 10000 casos semanales de promedio tuvo una alta letalidad llegando al 12% lo cual es muy peligroso para cualquier sistema de salud que puede colapsar repentinamente, sin embargo llegando al 2022 alcanzando el pico de casos reportados e incluso representando la mayor cantidad de casos acumulados hasta la fecha, tiene una letalidad menor al 2% destacando a pesar del brote masivo de ese año no era muy mortal para la gente.

Se recomenda estudiar esta relación del año 2022 con la vacunación que relaciones tienen las personas que no se aplicaron las vacunas con las nuevas muertes registradas.

> [!IMPORTANT]
> Esto fue un proyecto que participamos los miembros del canal del
> 
>[![](https://img.shields.io/youtube/channel/subscribers/UCuerQOTskuNkddcT738357g?style=for-the-badge&logo=youtube&label=ElProfeAlejo)](https://www.youtube.com/@ElProfeAlejo)


