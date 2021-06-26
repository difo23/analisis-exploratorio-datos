---
title: "Curso de Análisis Exploratorio de Datos"
day: "1"
publishDate: "2021-06-24"
thumbnailImage: "../images/day-1.png"
shareText: " Description: Vamos a desarrollar diferentes técnicas para explorar, explicar y entender cuáles son los patrones que tienes en cualquier data set y cómo podemos empezar a plantear cualquier modelo de ML, para saber si son de valor o no son de valor o cómo hacer esta propuesta. "
hashtags: ['learn', 'EDA', 'analisis', 'Exploratorio']
draft: false

---

## Agrupamiento de datasets

| Source:      | [Platzi URL](https://platzi.com/clases/2178-analisis-exploratorio-datos/34158-bienvenida-al-curso/) |
| ------------ | ------------------------------------------------------------ |
| **Course:    | Curso de Análisis Exploratorio de Datos                      |
| **Teacher:** | Maria Cruz                                                   |



## Notes 

```python
Chicago_df.groupby(['LIGHTING_CONDITION','REPORT_TYPE','CRASH_HOUR']).agg({'BEAT_OF_OCCURRENCE':'sum',})
```

```python
Chicago_df.groupby(['LIGHTING_CONDITION','REPORT_TYPE']).agg({'CRASH_HOUR':'mean'})
```

```python
Chicago_df.groupby(['LIGHTING_CONDITION','REPORT_TYPE']).agg({'CRASH_HOUR':['mean','min','max']})
```

- [Pandas groupby](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.groupby.html)

- [Pandas agg](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.agg.html)

  

#### Lecturas recomendadas

https://colab.research.google.com/drive/1RSrbKmS9N6wZOhJT9Guo-2F_-IiTTx66?usp=sharinghttps://colab.research.google.com/drive/1RSrbKmS9N6wZOhJT9Guo-2F_-IiTTx66?usp=sharing

https://raw.githubusercontent.com/terranigmark/curso-analisis-exploratorio-datos-platzi/main/Traffic_Crashes1.csvhttps://raw.githubusercontent.com/terranigmark/curso-analisis-exploratorio-datos-platzi/main/Traffic_Crashes1.csv



## Pandas GroupBy: Your Guide to Grouping Data in Python

### Organizando ambiente de trabajo con Python 

```bash
$ python -m venv pandas-gb-tut
$ source ./pandas-gb-tut/bin/activate
$ python -m pip install pandas
```

```python
import pandas as pd

# Use 3 decimal places in output display
pd.set_option("display.precision", 3)

# Don't wrap repr(DataFrame) across additional lines
pd.set_option("display.expand_frame_repr", False)

# Set max rows displayed in output to 25
pd.set_option("display.max_rows", 25)
```

[Guia para Pandas groupby](https://realpython.com/pandas-groupby/)

