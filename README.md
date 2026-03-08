# 📊 Telecom X – Análisis de Evasión de Clientes (Churn)

**Autor:** Alberto Edgardo Villalba  
**Challenge:** Telecom X – Alura (Data Analytics / Data Science)  

---

## 🧠 Introducción

Este proyecto analiza el fenómeno de **evasión de clientes (churn)** en Telecom X, con el objetivo de identificar patrones y factores asociados a la cancelación del servicio.

La evasión de clientes representa un problema relevante para el negocio, ya que impacta directamente en la estabilidad y los ingresos. A través del análisis de datos, se busca generar información que sirva como base para futuras estrategias de retención y modelos predictivos.

El trabajo forma parte del **Challenge Telecom X del programa de formación de Alura** y tiene **fines educativos y analíticos**.

---

## 🎯 Objetivos del análisis

- Analizar la distribución del churn entre los clientes.
- Identificar variables categóricas asociadas a la evasión.
- Comparar variables numéricas entre clientes que cancelan y los que no.
- Explorar relaciones entre variables mediante análisis de correlación.
- Generar insights relevantes para la toma de decisiones.

---

## 🧹 Limpieza y preparación de datos

Durante el proceso de preparación se realizaron las siguientes tareas:

- Carga de datos desde la API en formato JSON.
- Conversión de los datos a un DataFrame para su análisis.
- Revisión de valores inconsistentes y tratamiento de datos faltantes.
- Conversión de variables numéricas a su tipo correcto.
- Estandarización de variables binarias (Yes / No).
- Creación de variables derivadas, como **Cuentas_Diarias**.

---

## 📊 Análisis Exploratorio de Datos (EDA)

### 🔹 Distribución de evasión
Se analizó la proporción de clientes que cancelaron el servicio frente a los que permanecieron activos.

### 🔹 Variables categóricas
Se estudió la evasión según:
- Tipo de contrato
- Género
- Método de pago

El análisis muestra una mayor tasa de churn en contratos mensuales y ciertos métodos de pago.

### 🔹 Variables numéricas
Para las variables numéricas (**antigüedad, cargos mensuales, total gastado y cuentas diarias**) se utilizaron **boxplots**, ya que permiten comparar de forma clara la distribución, la mediana y la presencia de valores atípicos entre clientes que evaden y los que no.

Los resultados indican que:
- Los clientes que abandonan el servicio tienden a tener menor antigüedad.
- Los clientes con churn presentan, en promedio, cargos mensuales más elevados.
- El total gastado está fuertemente asociado a la antigüedad del cliente.

---

## 🔗 Análisis de correlación

Se realizó una matriz de correlación entre variables numéricas para identificar relaciones relevantes.

Principales hallazgos:
- La antigüedad presenta una relación inversa con el churn.
- Los cargos mensuales y diarios muestran asociación positiva con la evasión.
- El total gastado se correlaciona fuertemente con la antigüedad.

---

## 📌 Conclusiones e insights

- El churn se concentra en clientes recientes.
- Los contratos mensuales presentan mayor tasa de evasión.
- La antigüedad actúa como un factor protector frente al churn.
- El nivel de cargos influye en la decisión de abandono.

---

## 💡 Recomendaciones

- Incentivar la migración hacia contratos de mayor duración.
- Implementar estrategias de retención temprana en los primeros meses.
- Evaluar beneficios para clientes con cargos elevados.
- Utilizar las variables analizadas como base para modelos predictivos de churn.

---

## 🛠️ Tecnologías utilizadas

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Google Colab  

---

## 📘 Nota final

Este proyecto forma parte del **Challenge Telecom X de Alura** y fue desarrollado con **fines educativos y analíticos**, como ejercicio práctico de análisis exploratorio de datos aplicado a un caso de negocio.
