---
title: "Curso de Análisis Exploratorio de Datos"
day: "1"
publishDate: "2021-06-24"
thumbnailImage: "../images/day-1.png"
shareText: " Description: Vamos a desarrollar diferentes técnicas para explorar, explicar y entender cuáles son los patrones que tienes en cualquier data set y cómo podemos empezar a plantear cualquier modelo de ML, para saber si son de valor o no son de valor o cómo hacer esta propuesta. "
hashtags: ['learn', 'EDA', 'analisis', 'Exploratorio']
draft: false

---

## Medidas de dispersión

| Source:      | [Platzi URL](https://platzi.com/clases/2178-analisis-exploratorio-datos/34158-bienvenida-al-curso/) |
| ------------ | ------------------------------------------------------------ |
| **Course:    | Curso de Análisis Exploratorio de Datos                      |
| **Teacher:** | Maria Cruz                                                   |



## Notes 

## Medidas de dispersión

**Ejemplo:** Imagina que tienes una compañía de sombreros y comienzas a medir al usuario numero 1, ese sombrero medirá 16, el usuario numero 2 va a medir 18 y al usuario 3 medirá 20. Entonces, ya tenemos un rango de 16 a 20 para producción de sombreros, ahora hay que imaginar que este problema se lleva a millones de usuarios, no podemos medirlos todos, pero si se pueden usar medidas para saber que tan dispersos están los datos, por ejemplo si tu mides en 1 millón de sombreros y miras que solo hay una persona que tiene una medida de 21 no te conviene hacer sombreros con esa medida. Este conocimiento nos lo dará las medidas de dispersión.

------

- **Desviación estándar:** es un índice numérico de la dispersión de un conjunto de datos (o población). Mientras mayor es la desviación estándar, mayor es la dispersión de la población. La desviación estándar es un promedio de las desviaciones individuales de cada observación con respecto a la media de una distribución.

Pero, **¿qué nos indica esa desviación estándar?**

![1.PNG](https://static.platzi.com/media/user_upload/1-ccbc83cc-5f22-4c8b-8d88-bc3ba050b216.jpg)

- **Varianza:** es una medida de dispersión que representa la variabilidad de una serie de datos respecto a su media.

### Conclusiones clave: varianza y desviación estándar

- La varianza y la desviación estándar nos muestran cuánto varían los puntajes en una distribución del promedio.
- La desviación estándar es la raíz cuadrada de la varianza.
- Para conjuntos de datos pequeños, la varianza se puede calcular a mano, pero se pueden utilizar programas estadísticos para conjuntos de datos más grandes.

## Un ejemplo conceptual

La varianza y la desviación estándar son importantes porque nos dicen cosas sobre el conjunto de datos que no podemos aprender con solo mirar la [media o el promedio](https://www.greelane.com/link?to=how-to-calculate-the-mean-or-average-609546&lang=es&alt=https://www.thoughtco.com/how-to-calculate-the-mean-or-average-609546&source=variance-and-standard-deviation-3026711) . 

Como ejemplo, imagina que tienes tres hermanos menores: un hermano de 13 años y gemelos de 10. En este caso, la edad promedio de tus hermanos sería 11. Ahora imagina que tienes tres hermanos de 17, 12 años. y 4. En este caso, la edad promedio de sus hermanos aún sería 11, pero la varianza y la desviación estándar serían mayores.

## Importancia de la varianza y la desviación estándar

La varianza y la desviación estándar son importantes en las estadísticas porque sirven de base para otros tipos de cálculos estadísticos. Por ejemplo, la desviación estándar es necesario para la conversión de resultados de las pruebas en [puntuaciones Z](https://www.greelane.com/link?to=z-scores-worksheet-solutions-3126533&lang=es&alt=https://www.thoughtco.com/z-scores-worksheet-solutions-3126533&source=variance-and-standard-deviation-3026711) . La varianza y la desviación estándar también juegan un papel importante cuando se realizan pruebas estadísticas como las pruebas [t](https://www.greelane.com/link?to=sample-t-test-confidence-interval-example-4022456&lang=es&alt=https://www.thoughtco.com/sample-t-test-confidence-interval-example-4022456&source=variance-and-standard-deviation-3026711) .

- **Asimetría estadística**

![2.PNG](https://static.platzi.com/media/user_upload/2-c89131ae-ecce-407c-8234-c692a28ebc90.jpg)

- **Curtosis:**

![3.PNG](https://static.platzi.com/media/user_upload/3-fa681877-676b-4f3c-836a-904595882fa8.jpg)

La curtosis de una variable estadística/aleatoria es una característica de forma de su distribución de frecuencias/probabilidad.

