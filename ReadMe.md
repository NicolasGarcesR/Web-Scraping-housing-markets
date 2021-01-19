# Vivienda de interés social en Bogotá 

https://youtu.be/BJp0k3JLyP4

![imagen.png](attachment:imagen.png)<img scr = "1.png">

Una de las principales estrategias que el ministerio de vivienda ha implementado para atacar el déficit inmobiliario ha sido la construcción y financiación de Viviendas de Interés Social (VIS).La ley define la vivienda de interés social como aquella que es habitable, cumple con estándares de calidad,tiene un valor máximo que no pasa de los 135 SMLM y pertenece al estrato 2 o 3. 

El objetivo de estos proyectos es dar vivienda digna a los hogares más necesitados con precios asequibles, a la vez que ayuda a aumentar el bienestar social y contribuir a la equidad. Para comprobar que la vivienda de interés social este cumpliendo estos objetivos, tratare de evaluar el espacio que ocupan estos proyectos en el mercado inmobiliario utilizando web-scrapping.
Las preguntas a tratar de resolver en este proyecto son las siguientes:

-  ¿En el rango de precios entre 100 y 135 millones, las VIS son la mejor opción de vivienda? Que características físicas (número de habitaciones, numero baños, etc) se diferencian en la vivienda no subsidiada de la subsidiada ?

-  Hay sectores donde este tipo de vivienda tienda a ser más construida que en otros del mismo estrato? 

- ¿Logra esta política contribuir al aumento de la equidad a la vez que proporciona vivienda asequible? O, en otras palabras, ¿las VIS son equiparables en términos cuantitativos con otras viviendas del mismo estrato? 

## Metodología

- Scrapping: tomé información de todos los proyectos de interés social disponibles para Bogotá en la página https://www.estrenarvivienda.com/vivienda-interes-social/bogota. Utilicé Selenium y webdriver de Chrome para obetner los datos. Para la vivienda no subsidiada también tomé la información de esta pagina https://www.estrenarvivienda.com/proyectos-vivienda/bogota, de donde tomé los proyectos en los rangos de 100-200 millones y excluí los de interés social comparando los links de acceso. Se utilizó la misma metodología que con las VIS. El código de este proceso se encuentra en el notebook Final_project. 

- Tratamiento de la información : Para transformar el contenido de los xpath en información útil, procesé los datos extraídos con regex y posteriormente creé dataframes con panda para exportarlo como Excel. El resultado de este proceso son los Excel VIS y NO_VIS que se encuentran en el repositorio. Este trabajo tambien se encuentra en el notebook Final_project 

- Graficos: Utilicé Mathplotlib para generar los gráficos que se verán a continuación. El código de este proceso se encuentra en el notebook graphs. 

- Geolocalización: utilicé geopy y folium para transformar las direcciones en coordenadas de latitud y longitud y así realizar el mapa que se puede ver al principio de este read_me. El código de este proceso se encuentra en el notebook MAP 


## Resultados 

Se obtuvo información de 79 proyectos de interés social y 40 de proyectos no subsidiados. Estos son los análisis gráficos más relevantes. 


![imagen.png](attachment:imagen.png)

![imagen.png](attachment:imagen.png)

![imagen.png](attachment:imagen.png)

![imagen.png](attachment:imagen.png)

![imagen.png](attachment:imagen.png)

![imagen.png](attachment:imagen.png)

## Referencias

- “Viviendas de Interés Social.” Viviendavis, viviendavis.online/
- Decreto 1533 de 2019 - EVA - Función Pública.” Www.Funcionpublica.Gov.Co, www.funcionpublica.gov.co/eva/gestornormativo/norma.php?i=99716.
- “Estrenar Vivienda | Casas y Apartamentos Nuevos En Venta.” Estrenar Vivienda, www.estrenarvivienda.com/. Accessed 4 Dec. 2020.

<img scr = "6.png">

<img scr = "7.png">
