# Predicción del Nivel de PIB Global: Enfoque de Machine Learning

## 📋 Descripción del Proyecto
Este portafolio desarrolla un modelo predictivo para clasificar el nivel de Producto Interno Bruto (PIB) de distintos países utilizando datos del Banco Mundial (2023). El proyecto aborda la alta dimensionalidad de los indicadores económicos mediante técnicas de reducción de datos y limpieza rigurosa.

## 🌿 Estructura y Contenido de las Ramas (Etapas)

Este repositorio organiza el desarrollo en ramas independientes, cumpliendo con los hitos del proyecto:

### 📍 Rama: `etapa-1` (Análisis Descriptivo e Imputación)
*Contenido y tareas realizadas:*
1.  **Carga de Datos:** Extracción automatizada de indicadores mundiales usando `wbgapi`.
2.  **Filtrado de Calidad:** Eliminación de variables con más del **15% de datos faltantes** para reducir ruido.
3.  **Imputación:** Relleno de valores nulos restantes utilizando la **mediana** (robusta a valores extremos).
4.  **Análisis Exploratorio:** Generación de histogramas y boxplots para visualizar la distribución del PIB.
5.  **Ingeniería de Variables:** Creación de la variable objetivo categórica (PIB discretizado en: *Low, Medium-Low, Medium, Medium-High, High*).

### 📍 Rama: `etapa-2` (Reducción de Dimensionalidad - PCA)
*Contenido y tareas realizadas:*
1.  **Preprocesamiento:** Selección de variables numéricas y exclusión de identificadores.
2.  **Estandarización:** Aplicación de `StandardScaler` para normalizar las escalas de las variables.
3.  **Modelado PCA:** Entrenamiento del algoritmo de Componentes Principales.
4.  **Análisis de Varianza:** Gráfico de varianza acumulada para determinar la pérdida de información.
5.  **Selección de Componentes:** Retención de componentes suficientes para explicar más del **85% de la varianza**.
6.  **Dataset Final:** Generación de un DataFrame reducido (`X_pca`) listo para modelos de clasificación.

### 📍 Rama: `main` (Consolidado)
* Contiene la integración final de todo el código, incluyendo las funciones de carga, limpieza y transformación listas para producción.

---
**Autor:** Diego Fierro
**Contacto:** diego.fierro2@mail.udp.cl
