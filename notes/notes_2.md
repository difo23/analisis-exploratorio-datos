---
title: "Curso de Análisis Exploratorio de Datos"
day: "1"
publishDate: "2021-06-24"
thumbnailImage: "../images/day-1.png"
shareText: " Description: Vamos a desarrollar diferentes técnicas para explorar, explicar y entender cuáles son los patrones que tienes en cualquier data set y cómo podemos empezar a plantear cualquier modelo de ML, para saber si son de valor o no son de valor o cómo hacer esta propuesta. "
hashtags: ['learn', 'EDA', 'analisis', 'Exploratorio']
draft: false

---

# Qué es el análisis exploratorio de datos

| Source:      | [Platzi URL](https://platzi.com/clases/2178-analisis-exploratorio-datos/34158-bienvenida-al-curso/) |
| ------------ | ------------------------------------------------------------ |
| **Course:    | Curso de Análisis Exploratorio de Datos                      |
| **Teacher:** | Maria Cruz                                                   |



## Notes 

## Clase 2: Qué es el análisis exploratorio de datos

**¿Qué es un EDA?**

Significa `Exploratory data analysis`. Aquí comienza todo, antes de crear un modelo debemos saber para que lo vamos a hacer, debemos de tener contexto y la forma de hacerlo es exportando nuestros datos.

**Un poco de historia:**

En los años *90’s se comienza a sonar el termino de minería de datos* donde se especifica que busca patrones, busca las tendencias más grandes y es justo la minería de datos es lo que le comienza a dar orden a cómo podemos explorar datos y a buscar estos patrones. Esto no es un termino que haya surgido actualmente, de hecho la IA, las primeras redes neuronales salen en los años 70, solo que actualmente ya tenemos el computo necesario para que tu lo puedas hacer de tu computadora, lo que antes solo se podía hacer en el mundo académico y era exclusivo de super maquinas.

**Pero, todo esto, ¿de donde viene?**

Justo en los años `90’s con la minería de datos` se comienzan a crear metodologías, como estas:

- **KDD**: Knowledge discovery in DataBases.
- **SEMMA**: Sample, Explore, Modify, Model, and Assess.
- **CRISP-DM**: Cross Industry Standard Process for Data Mining.

Y de estás metodologías de minería de datos sale nuestro `EDA`.

Todo esto surge a partir de una necesidad y nos comenzamos a hacer mucha preguntas, pero la pregunta final es: ***¿Puedo contestar o no el requerimiento que me dieron con todos estos datos?*** Y si no tenemos los suficientes datos para resolver esta pregunta, eso es lo que hace precisamente el EDA, explicarnos si podemos contestar esta pregunta y si tenemos todo lo necesario para dar una respuesta.

**¿Pero qué debemos de hacer si no podemos dar una respuesta?** Tenemos que dar un paso atrás, debemos de pedir más datos.

### Antes de hacer cualquier modelo de ML o DP debemos de entender:

- De donde vienen los datos.
- El contexto de los datos.
- Por qué haremos el modelo.

**Etapas del eda:**

- Etapa 1: Definición del problema.
- Etapa 2: Preparación de datos.
- Etapa 3: Análisis de datos.
- Etapa 4: Desarrollo y representación de resultados.

------

> - **Nota:** Si está en nuestra posibilidad usar toda la base de datos para entrenar nuestro modelo, hay que hacerlo. es mucho mejor pagar un poco para dar una propuesta de valor.
>
> El foco principal del EDA es contar una historia prediciendo cuánto se va optimizar el problema implementando el modelo que vamos a proponer. Un científico de datos le da un valor a los datos.



**Metodologia para poner un orden:**

**Data Science:**

- Data requirements: ¿Qué queremos?
- Data collection: ¿Qué informacion tenemos para lograrlo?
- Data Processing: ¿Cómo la procesamos? ¿Qué tipo de datos?
- Data cleaning: ¿La info es correcta?
- EDA: ¿Puedo contestar el requerimiento? ¿Cómo puedo contestar la pregunta?
- Modeling and algorithm
- Data Product
- Communication