---
title: "Curso de Análisis Exploratorio de Datos"
day: "1"
publishDate: "2021-06-24"
thumbnailImage: "../images/day-1.png"
shareText: " Description: Vamos a desarrollar diferentes técnicas para explorar, explicar y entender cuáles son los patrones que tienes en cualquier data set y cómo podemos empezar a plantear cualquier modelo de ML, para saber si son de valor o no son de valor o cómo hacer esta propuesta. "
hashtags: ['learn', 'EDA', 'analisis', 'Exploratorio']
draft: false

---

## Pivot tables y cross-tabulations

| Source:      | [Platzi URL](https://platzi.com/clases/2178-analisis-exploratorio-datos/34158-bienvenida-al-curso/) |
| ------------ | ------------------------------------------------------------ |
| **Course:**  | Curso de Análisis Exploratorio de Datos                      |
| **Teacher:** | Maria Cruz                                                   |



## Notes

Pivot table or crosstab? Let’s see panda’s description.

![](https://miro.medium.com/max/904/1*6H0DLixQPR5KH8PPvxMqvA.png)

**Crosstab**: “Compute a simple cross-tabulation of two (or more) factors. By default computes a frequency table of the factors unless an array of values and an aggregation function are passed.”

```python
pd.crosstab(index=df['Car'], columns=df['Color'])
```


![](https://miro.medium.com/max/1133/1*6xZ8YGeHTypsL-ubqy8_Lg.png)

**Pivot Table**: “Create a spreadsheet-style pivot table as a DataFrame. The levels in the pivot table will be stored in MultiIndex objects (Hierarchical indexes on the index and columns of the result DataFrame.

```python
pd.pivot_table(df, index='Car', aggfunc='mean')
#Deleting aggfunc='mean' will yield the same value.
```



![](https://miro.medium.com/max/481/1*JlFe7bGYaCPU7u4aetLXqQ.png)

Both create tables and compare features/columns of data. Let’s see some examples.

> - [Quick Guide to Pandas Pivot Table & Crosstab](https://medium.com/@yangdustin5/quick-guide-to-pandas-pivot-table-crosstab-40798b33e367)
> - [Pandas Crosstab Explained](https://pbpython.com/pandas-crosstab.html)
> - [Reshaping and pivot tables](https://pandas.pydata.org/docs/user_guide/reshaping.html#reshaping-and-pivot-tables)



## El mismo resultado para las dos tablas:

```python
#Pivot Table
pd.pivot_table(df, index='Car', columns='Color', values='MPG', aggfunc='count', fill_value=0)

#For the values parameter, I could have used 'Name' or 'Price and still get the same result.

#Crosstab
pd.crosstab(index=df['Car'], columns=df['Color'])
```

![](https://miro.medium.com/max/1118/1*kp8TrZ9dAHdJBBkRnotrxA.png)


```python
#Pivot Table
pd.pivot_table(df, index='Car', columns='Color', values='Price', margins=True)

#Crosstab
pd.crosstab(index=df['Car'], columns=df['Color'], values=df['Price'], margins=True, aggfunc='mean')
```

![](https://miro.medium.com/max/1313/1*9Ah3zclU_8kxrFNENEO98Q.png)

