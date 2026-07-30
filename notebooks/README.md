# Notebooks

Esta carpeta contiene el notebook principal utilizado para desarrollar el análisis del comportamiento de clientes de **NovaRetail+**.
El análisis fue desarrollado como parte de un proyecto académico de TripleTen.

## 📓 NovaRetail+ — Análisis del comportamiento de clientes

El notebook contiene el desarrollo completo del análisis realizado para identificar qué factores del comportamiento de los clientes presentan una mayor asociación con el ingreso anual generado.

### Contenido del notebook

El análisis está organizado en las siguientes etapas:

1. **Carga y exploración de datos**

   * Revisión de la estructura del dataset.
   * Identificación de variables numéricas, binarias y categóricas.
   * Validación de valores faltantes y tipos de datos.

2. **Preparación de los datos**

   * Exploración de variables numéricas.
   * Revisión de variables binarias y categóricas.
   * Identificación de posibles valores extremos.
   * Documentación de los supuestos utilizados en el análisis.

3. **Visualización de relaciones**

   * Matriz de correlación.
   * Heatmap.
   * Scatterplots de las relaciones más relevantes.

4. **Análisis de correlación**

   * Pearson.
   * Spearman.
   * Correlación punto-biserial.
   * V de Cramér.

5. **Interpretación para el negocio**

   * Evaluación de las relaciones encontradas.
   * Diferenciación entre correlación y causalidad.
   * Identificación de posibles implicaciones para NovaRetail+.

6. **Limitaciones y próximos pasos**

   * Limitaciones metodológicas del análisis.
   * Posibles análisis adicionales relacionados con segmentación, publicidad y abandono.

## 🔎 Relaciones principales analizadas

El notebook presta especial atención a dos relaciones:

**Compras mensuales vs. ingreso anual**

Presenta la asociación más fuerte del análisis, con una correlación de Pearson de aproximadamente **0.97**.

**Gasto en publicidad dirigida vs. visitas mensuales**

Presenta una asociación positiva moderada, con una correlación de Pearson de aproximadamente **0.58**.

También se analizan variables como membresía premium, abandono, región y tipo de dispositivo utilizando métodos adecuados para cada tipo de variable.

## ⚠️ Nota metodológica

Los resultados presentados corresponden a un **análisis exploratorio y correlacional**.

Las asociaciones identificadas permiten detectar patrones en los datos, pero no permiten concluir que una variable sea la causa directa de otra.

Para una explicación completa de los objetivos, resultados e implicaciones del proyecto, consultar el **README principal del repositorio**.
