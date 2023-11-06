# Montecarlo-sim
Código de python creado por Isidora Ramírez

Es una simulación hecha en base a el método Monte Carlo que nos creará una población estelar aleatoria siguiendo cierta condiciones, como el rango de masa de los cuerpos estelares y el rango del tiempo de nacimiento de estos. El programa nos entregará distintas gráficas que nos ayudarán a comprender la evolución y la distribución de los cuerpos estelares que podrían estar en la Vía Lactea. 

Para usar el codigo solo se debe descargar, se puede encontrar en el siguiente enlace:
```sh
https://github.com/iramirezcal/Montecarlo-sim/blob/eae35a576ad380df23645f6deef41625eaa7918e/MC(1).ipynb
```

## Requerimientos
- Librerías:
    - Numpy
    - Matplotlib   

## Simulación
- Inicialmente se crea una lista con masas aleatorias, entre cierto rango, por defecto 0.08-100 pero estos valores se deben cambiar dependiendo de lo que se quiera modelar, al igual que la cantidad de estrellas que se quieren estudiar. Seguido a esto se hacen 2 listas dependiendo del rango de las masas para realizar la IMF dependiendo del alpha que le corresponda según la power law y así obtenemos los valores para la gráfica, este es nuestro primer output, la gráfica de IMF. 

- En segúnda instancia se entrega un valor de tiempo de nacimiento a cada estrella para así determinar su SFR, con esto se hace un histograma para análizar la distribución de este y podemmos ver que en primera aproximación es constante

- Continuando con separar los datos de las estrellas que siguen en la main sequence de las que ya no forman parte, además de categorizarlas por el tipo de remanente (Enana blanca, estrella de neutrones o agujero negro). Se utilizan rangos en base a literatura específica, estos pueden variar y ser modificados dependiendo de lo que decida el usuario y su literatura específica. Con esto se realiza un histograma de la edad de cada cuerpo estelar para así poder analizar la distribución de estos en la galaxia. Acercandonos al final de la simulación se obtienen las masa finales de cada objeto para volver a realizar un análisis de su distribución dentro de la galaxia. Por último se calcúla la razón en la que se encuentra cada componente en la totalidad de objetos 
