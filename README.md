# Data-cleaning-Global-Shark-Attacks
## First project - Data cleaning and wrangling

![texto cualquiera por si no carga la imagen](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/Jaws_Book_1975_Cover.jpg) 

El objetivo de este primer proyecto es limpiar los datos del dataframe(https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Data/attacks.csv) con dos restricciones: no se pueden eliminar **las columnas** originales, ni reduccir el número de **filas** por debajo de 2500.

Para facilitar la limpieza de datos elegimos un objeto de estudio: analizar la **evolución de la agresividad** de los tiburones en los últimos 50 años.
Para ello, hemos agrupado los tipos de lesión producidos por los ataques de tiburon en 5 categorías:'no injury', 'minor injury', 'injury', 'severe injury', 'fatal' .

- 'no injury': el ataque no produjo lesiones a seres humanos. Solo daños a medios físicos, como barcos.
- 'minor injury' : el ataque produjo lesiones de caraccter superficial o en miembros menos importantes(dedos). Torceduras, contusiones, arañazos, etc.
- 'injury' : el ataque produjo lesiones graves. Laceraciones, abrasiones, heridas en extremidades, etc.
- 'severe injury' : el ataque produjo lesiones muy graves. Fracturas, amputaciones, heridas en el cuello, etc.
- 'fatal': el ataque produjo la muerte.
Esta categorización queda recogida en una nueva columna, **'injury_values'**, otorgando un valor a cada tipo de dato por si a la hora de realizar el estudio necesitamos un dato numérico:
- 'no injury': 0
- 'minor injury' : 1
- 'injury' : 2
- 'severe injury' : 3
- 'fatal': 4
Para esta categorización, previamente hemos limpiado los datos de varias columnas del dataframe para determinar: si el ataque fue producido por un tiburón; si el dato entra dentro de nuestra franja temporal de estudio.

La metodología de trabajo ha sido la siguiente:
- Estudio preliminar del dataframe.
- Estudio preliminar de cada columna.
- Ajustes básicos: mayúsculas, minúsculas, espacios innecesarios, etc.
- Estudio de valores desconocidos, a través de otras columnas relacionadas o, en su defecto, determinando que hacer con ellos.
- Determinar si afecta al objeto de estudio, en cuyo caso pasamos a un estudio en profundidad.
- Ajuste de indices.

## Resultados del estudio ##

Tras realizar la limpieza de datos nos centramos en dos columnas, 'year' e 'injury_values'. Analizamos los valores absolutos, los valores porcentuales y algunas medidas de centralización y de dispersión, que nos arrojan los siguientes resultados:

 ### **1.'no injury' porcentual** ###
  
![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.no_injury.percen.png)

 ### **2.'minor injury' porcentual** ###
  
![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.minor_injury.percen.png)
  
  ### **3.'injury' porcentual** ###
  
![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.injury.percen.png)

  ### **4.'severe injury' porcentual** ###
  
![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.%20major_injury.percen.png)

  ### **5.'fatal' porcentual** ###
  
![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.%20fatal.percen.png)

  ### **6.'no injury' absoluto** ###
  
![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.no_injury.png)

  ### **7.'fatal' absoluto** ###

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/evol.%20fatal.png)

  ### **8.Evolución por decadas de los valores absolutos:** ###

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/graficos%201969-1978.png)

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/graficos%201979-1988.png)

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/graficos%201989-1998.png)

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/graficos%201999-2008.2png.png)

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/graficos%202009-2018.2.png)

En este primer análisis de los datos absolutos y porcentuales, podemos determinar que la agresividad de los ataques de tiburón ha disminuido en los últimos 50 años. Sobre esto se podrían hacer numerosas conjeturas( especialmente con la cantidad de datos disponibles) pero no vamos a entrar en ello.



Para la próxima semana analizaremos la evolución de los ataques de orcas a tiburones porque...

![texto cualquiera](https://github.com/Jaimercmail/Data-cleaning-Global-Shark-Attacks/blob/main/Multimedia/final%20joke.jpg)


 
