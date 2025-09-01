# Regresión No Lineal

Este proyecto tiene como objetivo aplicar y comparar distintos modelos de regresión no lineal para analizar la relación entre el tiempo de entrega de las actividades y la calificación obtenida. 
La hipótesis a probar es que, mientras más cerca de la hora de cierre se entrega la tarea, peor será la calificación.

Utilizaremos el archivo de nombre [TiempoDeEntregaOriginal](TiempoDeEntregaOriginal.csv), el cual contiene información de **432 actividades entregadas** en la materia de Sistemas Digitales en la Universidad de Monterrey. Los datos fueron generados en el semestre de Otoño 2022 por el Dr. Antonio Martínez Torteya.

## Datos utilizados
En el archivo se encuentran las siguientes variables:

- **Tiempo**: Tiempo restante antes de que cerrara la bandeja de entrega, en horas (ej. 1 = domingo 11:00 p.m.; 48 = viernes a medianoche).  
- **Calificación**: Calificación obtenida en la actividad (escala de 0 a 110).

## Pasos del análisis

### 1. Carga y exploración  
- Importar el archivo TiempoDeEntrega.csv.  
- Revisar datos, detectar errores o valores no numéricos y eliminarlos.  
- Eliminar outliers poco realistas.  
- Generar una gráfica de dispersión inicial.

### 2. División de datos  
- Separar en entrenamiento (70%) y prueba (30%).  
- Calcular promedios de tiempo y calificación en cada conjunto y comentarlos.

### 3. Regresión polinomial  
- Entrenar un polinomio (grado 2).  
- Revisar el resumen estadístico del modelo.  
- Comentar sobre el signo y la significancia del término lineal.  
- Graficar curva polinomial vs datos reales.

### 4. Regresión segmentada 
- Entrenar un modelo segmentado con polinomios cuadráticos en cada segmento.  
- Generar predicciones en prueba.  
- Graficar línea del modelo sobre los datos.

### 5. Regresión KNN  
- Entrenar un modelo KNN (probando distintos valores de k).  
- Generar predicciones en prueba.  
- Graficar curva vs valores reales.  

### 6. Comparación de modelos  
- Calcular el RSE de los tres modelos.  
- Identificar cuál tiene menor error.  

### 7. Visualización conjunta  
- Generar una gráfica con datos reales y las predicciones de los tres modelos, diferenciados por colores.  
- Extraer conclusiones finales.

## Archivos del proyecto
- [Reporte en ipynb](A1.6_648241.ipynb)  
- [Reporte en html](A1.6_648241.html)  
- [Archivo TiempoDeEntrega utilizado](TiempoDeEntrega.csv)
- [Archivo TiempoDeEntrega original](TiempoDeEntregaOriginal.csv)  
