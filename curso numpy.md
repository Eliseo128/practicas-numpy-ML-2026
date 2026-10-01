# Índice del curso de NumPy: de Principiante a Avanzado

Curso orientado a estudiantes de **preparatoria**, con enfoque práctico en **Python, Ciencia de Datos, Machine Learning e Inteligencia Artificial**.

## Módulo 1. Fundamentos de NumPy — Principiante

1. **Introducción a NumPy**

   * ¿Qué es NumPy?
   * Características principales
   * Ventajas frente a las listas de Python
   * Aplicaciones en Ciencia de Datos e Inteligencia Artificial

2. **Instalación y configuración**

   * Instalación de NumPy
   * Verificación de la instalación
   * Importación de NumPy
   * Uso de NumPy en VS Code
   * Uso de NumPy en Jupyter Notebook

3. **Arrays (ndarray)**

   * Concepto de array
   * Crear un array
   * `np.array()`
   * Arrays de una dimensión
   * Arrays de dos dimensiones
   * Arrays multidimensionales

4. **Propiedades de los arrays**

   * `ndim`
   * `shape`
   * `size`
   * `dtype`
   * `itemsize`

5. **Tipos de datos**

   * Enteros
   * Decimales
   * Booleanos
   * Cadenas
   * Conversión de tipos con `astype()`

6. **Acceso a elementos**

   * Índices
   * Índices negativos
   * Acceso a filas y columnas
   * Modificación de elementos

---

## Módulo 2. Operaciones básicas con arrays — Principiante

7. **Creación de arrays**

   * `zeros()`
   * `ones()`
   * `full()`
   * `empty()`
   * `arange()`
   * `linspace()`

8. **Operaciones matemáticas**

   * Suma
   * Resta
   * Multiplicación
   * División
   * Potencias
   * Módulo

9. **Operaciones entre arrays**

   * Operaciones elemento por elemento
   * Comparación de arrays
   * Operaciones con escalares

10. **Funciones matemáticas**

* `sqrt()`
* `abs()`
* `round()`
* `floor()`
* `ceil()`
* `exp()`
* `log()`

11. **Estadística básica**

* `sum()`
* `mean()`
* `median()`
* `min()`
* `max()`
* `std()`
* `var()`

---

## Módulo 3. Indexación y manipulación — Principiante/Intermedio

12. **Slicing**

* Selección de rangos
* Filas
* Columnas
* Subarrays

13. **Indexación avanzada**

* Indexación booleana
* Indexación mediante listas
* Condiciones múltiples

14. **Redimensionamiento**

* `reshape()`
* `resize()`
* `flatten()`
* `ravel()`

15. **Transposición**

* `transpose()`
* `.T`

16. **Unión de arrays**

* `concatenate()`
* `stack()`
* `vstack()`
* `hstack()`

17. **Separación de arrays**

* `split()`
* `vsplit()`
* `hsplit()`

---

## Módulo 4. Operaciones intermedias con NumPy

18. **Broadcasting**

* Concepto
* Reglas del broadcasting
* Operaciones entre diferentes dimensiones
* Ejemplos prácticos

19. **Funciones universales (ufuncs)**

* Concepto
* Operaciones vectorizadas
* Funciones matemáticas
* Comparaciones

20. **Ordenamiento y búsqueda**

* `sort()`
* `argsort()`
* `where()`
* `searchsorted()`

21. **Valores únicos**

* `unique()`
* Conteo de valores
* Frecuencias

22. **Valores booleanos**

* `any()`
* `all()`
* Condiciones
* Máscaras booleanas

23. **Manejo de valores especiales**

* `NaN`
* `Inf`
* `isnan()`
* `isinf()`
* `nanmean()`
* `nanmedian()`

---

## Módulo 5. Álgebra lineal

24. **Conceptos de matrices**

* Vectores
* Matrices
* Matrices cuadradas
* Matriz identidad

25. **Operaciones matriciales**

* Suma y resta
* Multiplicación
* Producto punto
* Producto matricial

26. **Álgebra lineal con `numpy.linalg`**

* `dot()`
* `matmul()`
* `det()`
* `inv()`
* `solve()`

27. **Vectores y normas**

* Norma de un vector
* Distancias
* Normalización

28. **Valores y vectores propios**

* Eigenvalues
* Eigenvectors
* `eig()`

---

## Módulo 6. NumPy para Ciencia de Datos

29. **Generación de datos**

* Datos aleatorios
* `random`
* Semillas
* Reproducibilidad

30. **Distribuciones estadísticas**

* Uniforme
* Normal
* Binomial
* Poisson

31. **Análisis estadístico**

* Media
* Mediana
* Desviación estándar
* Percentiles
* Correlación

32. **Limpieza de datos con NumPy**

* Valores faltantes
* Filtrado
* Reemplazo de valores
* Detección de valores atípicos

33. **NumPy y Pandas**

* Convertir NumPy → Pandas
* Convertir Pandas → NumPy
* `Series`
* `DataFrame`
* Cuándo utilizar NumPy y cuándo Pandas

---

# Módulo 7. NumPy aplicado a Machine Learning

34. **Preparación de datos**

* Variables de entrada
* Variables de salida
* Matrices de características
* Vectores objetivo

35. **Normalización**

* Escalamiento
* Normalización de datos
* Estandarización

36. **Separación de datos**

* Datos de entrenamiento
* Datos de prueba
* Manipulación de matrices

37. **NumPy y regresión lineal**

* Representación de datos
* Cálculo de predicciones
* Error
* Operaciones matriciales

38. **NumPy y clasificación**

* Representación numérica
* Variables binarias
* Matrices de datos

39. **NumPy y redes neuronales**

* Entradas
* Pesos
* Sesgos
* Funciones de activación
* Propagación hacia adelante

---

# Módulo 8. NumPy avanzado

40. **Arrays multidimensionales avanzados**

* 3D
* 4D
* Manipulación de dimensiones

41. **Stride y memoria**

* `strides`
* Layout de memoria
* C vs Fortran order

42. **Views y copies**

* Diferencia entre vista y copia
* `copy()`
* Modificación de datos compartidos

43. **Vectorización avanzada**

* Eliminación de ciclos `for`
* Operaciones vectorizadas
* Optimización de código

44. **Broadcasting avanzado**

* Broadcasting multidimensional
* Aplicaciones en Machine Learning

45. **Funciones personalizadas**

* `vectorize()`
* `apply_along_axis()`
* `apply_over_axes()`

---

# Módulo 9. NumPy avanzado para Inteligencia Artificial

46. **Manipulación de grandes matrices**

* Matrices de características
* Operaciones por lotes
* Representación de datasets

47. **Cálculo numérico**

* Derivadas aproximadas
* Gradientes
* Integración numérica

48. **Transformaciones matemáticas**

* Transformaciones lineales
* Rotaciones
* Escalamiento
* Transformaciones multidimensionales

49. **NumPy en procesamiento de imágenes**

* Imagen como array
* Canales RGB
* Escala de grises
* Recorte
* Redimensionamiento
* Operaciones píxel por píxel

50. **NumPy en visión artificial**

* Matrices de imágenes
* Máscaras
* Umbralización
* Manipulación de canales

---

# Módulo 10. Optimización y proyectos avanzados

51. **Optimización de código**

* Vectorización
* Evitar ciclos innecesarios
* Uso eficiente de memoria

52. **Medición del rendimiento**

* `time`
* `timeit`
* Comparación de algoritmos

53. **Procesamiento de grandes cantidades de datos**

* Arrays grandes
* Memoria
* Operaciones eficientes

54. **Integración con otras bibliotecas**

* NumPy + Pandas
* NumPy + Matplotlib
* NumPy + Scikit-learn
* NumPy + OpenCV

55. **Buenas prácticas**

* Organización del código
* Nombres de variables
* Documentación
* Reutilización
* Optimización

---

# Módulo 11. Proyectos integradores

56. **Proyecto 1 — Análisis de calificaciones**

* Crear dataset
* Calcular promedios
* Identificar máximos y mínimos
* Estadística básica

57. **Proyecto 2 — Análisis de ventas**

* Productos
* Precios
* Cantidades
* Ventas mensuales
* Estadísticas

58. **Proyecto 3 — Predicción de precios**

* Datos históricos
* Preparación de matrices
* Variables de entrada
* Predicción con Machine Learning

59. **Proyecto 4 — Procesamiento de imágenes**

* Cargar imagen
* Convertir a array
* Manipular píxeles
* Crear filtros básicos

60. **Proyecto 5 — Mini sistema de Machine Learning**

* Preparar datos con NumPy
* Entrenamiento
* Predicción
* Evaluación
* Visualización de resultados

---

## Ruta de aprendizaje

| Nivel                      | Módulos | Competencia principal                       |
| -------------------------- | ------- | ------------------------------------------- |
| 🟢 **Principiante**        | 1–3     | Crear, consultar y manipular arrays         |
| 🟡 **Intermedio**          | 4–6     | Realizar análisis y operaciones matriciales |
| 🟠 **Intermedio-Avanzado** | 7–8     | Aplicar NumPy a Machine Learning            |
| 🔴 **Avanzado**            | 9–10    | Optimizar y utilizar NumPy en IA            |
| 🔵 **Integrador**          | 11      | Desarrollar proyectos completos             |

**Resultado esperado:** al finalizar, el estudiante podrá utilizar NumPy para **manipulación de datos, cálculo numérico, álgebra lineal, análisis estadístico, procesamiento de imágenes y preparación de datos para Machine Learning e Inteligencia Artificial**.
