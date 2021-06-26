---
title: "Curso de Análisis Exploratorio de Datos"
day: "1"
publishDate: "2021-06-24"
thumbnailImage: "../images/day-1.png"
shareText: " Description: Vamos a desarrollar diferentes técnicas para explorar, explicar y entender cuáles son los patrones que tienes en cualquier data set y cómo podemos empezar a plantear cualquier modelo de ML, para saber si son de valor o no son de valor o cómo hacer esta propuesta. "
hashtags: ['learn', 'EDA', 'analisis', 'Exploratorio']
draft: false

---

## Transformación de los datos

| Source:      | [Platzi URL](https://platzi.com/clases/2178-analisis-exploratorio-datos/34158-bienvenida-al-curso/) |
| ------------ | ------------------------------------------------------------ |
| **Course:    | Curso de Análisis Exploratorio de Datos                      |
| **Teacher:** | Maria Cruz                                                   |



## Notes 

```python
#Llamamos el set de datos público 
Chicago_data = 'https://raw.githubusercontent.com/terranigmark/curso-analisis-exploratorio-datos-platzi/main/Traffic_Crashes1.csv'

# Debes crear tu propio token
token_map_plot='tu_token'
```

[Crea tu mapbox token](https://docs.mapbox.com/help/tutorials/get-started-tokens-api/) Esto sirve para poder graficar sobre mapas. 

```python
import pandas as pd 
```

```python
Chicago_df=pd.read_csv(Chicago_data,error_bad_lines=False)

# Explorar un poco los datos
Chicago_df.head()
Chicago_df.info()
```

```python
# Hacer algunas transformaciones de fechas con la guncion apply
Chicago_df['CRASH_DATE'] = Chicago_df['CRASH_DATE'].apply(lambda x: pd.to_datetime(x,
errors='coerce', utc=True))

# Hacer algunas transformaciones de tipo de dato
Chicago_df['NUM_UNITS'].astype('int32')
```

```python

# Usamos el api a mapbox y plotly para graficar nuestro mapa de accidentes en chicago
import plotly.express as px
px.set_mapbox_access_token(token_map_plot)
```

```python
#df = px.data.carshare()

fig = px.scatter_mapbox(Chicago_df, lat="LATITUDE", lon="LONGITUDE", color="CRASH_HOUR", size="NUM_UNITS", color_continuous_scale=px.colors.cyclical.IceFire, size_max=15, zoom=10)

fig.show()
```



#### Lecturas recomendadas

![img](https://www.google.com/s2/favicons?domain=https://colab.research.google.com/drive/1OaxV31RAEuIU73x7Tp81Lbb_cwc-lNbb?usp=sharing/img/favicon.ico?vrz=colab-20201208-085602-RC00_346307824)https://colab.research.google.com/drive/1OaxV31RAEuIU73x7Tp81Lbb_cwc-lNbb?usp=sharinghttps://colab.research.google.com/drive/1OaxV31RAEuIU73x7Tp81Lbb_cwc-lNbb?usp=sharing![img](https://www.google.com/s2/favicons?domain=https://static-assets.mapbox.com/branding/favicon/v1/apple-touch-icon.png?v=gAd4JjrGWl)

Creating access tokens with the Tokens API | Help | Mapboxhttps://docs.mapbox.com/help/tutorials/get-started-tokens-api/![img](https://www.google.com/s2/favicons?domain=https://static.platzi.com/media/favicons/platzi_favicon.png)

https://raw.githubusercontent.com/terranigmark/curso-analisis-exploratorio-datos-platzi/main/Traffic_Crashes1.csvhttps://raw.githubusercontent.com/terranigmark/curso-analisis-exploratorio-datos-platzi/main/Traffic_Crashes1.csv