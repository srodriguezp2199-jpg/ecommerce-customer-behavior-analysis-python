# Análisis del comportamiento de clientes — NovaRetail+

## 📌 Descripción del proyecto

NovaRetail+ es una plataforma de comercio electrónico en Latinoamérica. En este proyecto analicé información sobre el comportamiento de sus clientes con el objetivo de responder una pregunta principal:

**¿Qué factores del comportamiento del cliente están más fuertemente asociados con el ingreso anual generado?**

Para responderla realicé un análisis exploratorio y correlacional utilizando información sobre visitas, compras, inversión en publicidad dirigida, satisfacción, membresía premium, abandono y otras características de los clientes.

El objetivo no fue únicamente encontrar correlaciones, sino entender cuáles podían tener mayor relevancia para el negocio y cuáles requerían análisis adicionales antes de tomar decisiones.

> Este proyecto es un análisis correlacional. Las relaciones encontradas no permiten establecer causalidad.
> Este proyecto fue desarrollado como parte de mi formación en Data Analytics en TripleTen, utilizando un caso de negocio y un dataset proporcionados para fines educativos.

## 🎯 Objetivo

Identificar qué variables del comportamiento de los clientes presentan una mayor asociación con el ingreso anual generado y utilizar estos resultados para detectar posibles oportunidades relacionadas con recurrencia de compra, publicidad y retención.

## 📊 Datos analizados

El dataset contiene **15.000 registros de clientes** y variables relacionadas con:

* edad;
* nivel de ingreso;
* visitas mensuales;
* compras mensuales;
* gasto en publicidad dirigida;
* satisfacción;
* membresía premium;
* abandono;
* tipo de dispositivo;
* región;
* ingreso anual generado.

La variable principal del análisis fue `ingreso_anual`.

## 🛠️ Herramientas utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Jupyter Notebook

## 🔎 Análisis realizado

El proyecto comenzó con una exploración y validación general de los datos, revisando tipos de variables, valores faltantes, distribuciones y posibles valores extremos.

Posteriormente analicé las relaciones entre las diferentes variables utilizando visualizaciones y distintos coeficientes de asociación dependiendo del tipo de dato:

* **Pearson** para relaciones lineales entre variables numéricas.
* **Spearman** para complementar el análisis sin asumir una relación estrictamente lineal.
* **Correlación punto-biserial** para variables binarias frente a variables numéricas.
* **V de Cramér** para evaluar asociaciones entre variables categóricas.

También utilicé heatmaps y scatterplots para complementar la evidencia numérica con una revisión visual de las relaciones más relevantes.

## 📈 Principales hallazgos

### Compras mensuales e ingreso anual

La relación más fuerte encontrada fue entre `compras_mes` e `ingreso_anual`.

* **Pearson:** 0.967
* **Spearman:** 0.967

Los clientes que realizan más compras mensuales tienden a generar mayores ingresos anuales. La relación observada es muy fuerte y prácticamente lineal.

Desde una perspectiva de negocio, este resultado muestra que la frecuencia de compra es una variable importante para entender el valor generado por los clientes y abre la posibilidad de explorar estrategias enfocadas en aumentar la recurrencia.

### Publicidad dirigida y visitas

También se encontró una asociación positiva moderada entre `gasto_publicidad_dirigida` y `visitas_mes`.

* **Pearson:** 0.579
* **Spearman:** 0.559

Un mayor gasto en publicidad tiende a estar asociado con un mayor número de visitas, aunque existe una variabilidad considerable entre clientes.

Esto sugiere que aumentar la inversión no necesariamente genera resultados proporcionales para todos los usuarios y que sería necesario analizar con mayor detalle la segmentación y efectividad de las campañas.

### Membresía premium

La relación entre `miembro_premium` e `ingreso_anual` fue positiva pero muy débil:

* **Punto-biserial:** 0.093

Esto indica que, dentro de este análisis, pertenecer al programa premium tiene poca asociación con el ingreso anual generado.

### Abandono

La relación entre `abandono` e `ingreso_anual` fue prácticamente nula:

* **Punto-biserial:** -0.003

Por lo tanto, el ingreso anual por sí solo no parece ser una variable suficiente para entender el abandono de clientes.

## 💡 Implicaciones para el negocio

Los resultados muestran dos líneas de análisis especialmente interesantes.

La primera es la **recurrencia de compra**. La fuerte asociación entre compras mensuales e ingreso anual indica que identificar clientes con potencial para aumentar su frecuencia de compra podría ser relevante para futuras estrategias de retención y crecimiento.

La segunda es la **eficiencia de la publicidad dirigida**. Aunque existe una relación positiva entre inversión publicitaria y visitas, la dispersión observada muestra que algunos clientes generan más tráfico con niveles de inversión similares o incluso menores.

Por esta razón, sería interesante analizar qué segmentos responden mejor a la publicidad antes de aumentar de manera generalizada la inversión.

## ⚠️ Limitaciones

Este análisis es exploratorio y correlacional, por lo que **no permite establecer relaciones causales**.

También se identificaron valores extremos en diferentes variables numéricas que podrían influir en algunos coeficientes de correlación.

Además, las correlaciones analizadas son principalmente bivariadas y no consideran posibles variables adicionales que puedan influir simultáneamente sobre las relaciones observadas.

## 🚀 Próximos pasos

A partir de los resultados del proyecto, algunas líneas de análisis que podrían desarrollarse son:

1. Segmentar clientes según compras mensuales e ingreso anual para identificar perfiles de alto valor.
2. Analizar con mayor profundidad qué segmentos responden mejor a la publicidad dirigida.
3. Investigar el abandono utilizando variables como satisfacción y frecuencia de visitas.
4. Desarrollar modelos que permitan controlar otras variables y estudiar con mayor profundidad los factores asociados al ingreso generado.

## 📁 Estructura del repositorio

```text
novaretail-customer-behavior-analysis/
│
├── README.md
│
└── notebooks/
    ├── README.md
    └── novaretail_customer_behavior_analysis.ipynb
```

## 🚀 Habilidades aplicadas

* Limpieza y validación de datos
* Análisis exploratorio de datos (EDA)
* Análisis de correlación
* Pearson y Spearman
* Correlación punto-biserial
* V de Cramér
* Visualización de datos
* Interpretación de resultados
* Traducción de resultados estadísticos a implicaciones de negocio

## 👤 Autor

**Santiago Rodríguez Pérez**

Data Analyst | Python | SQL | Power BI


---

## 📋 Requisitos

- Python 3.7+
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scipy`
