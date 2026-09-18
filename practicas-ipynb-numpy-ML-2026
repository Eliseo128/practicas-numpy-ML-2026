Claro. Siguiendo exactamente el procedimiento de la **Práctica 6 con NumPy**, ahora convertiremos los cinco ejercicios a **Jupyter Notebook (`.ipynb`)**, trabajando desde **VS Code** con el entorno virtual `.venv6`.

# Práctica 6 — NumPy con Jupyter Notebook desde VS Code

**Nivel:** 3.er semestre de preparatoria
**Carpeta:** `practica6-ml-numpy`
**Entorno virtual:** `.venv6`
**Bibliotecas:** NumPy + Jupyter + IPykernel
**Editor:** Visual Studio Code

---

## 1. Crear la carpeta de trabajo

Abre **VS Code → Terminal → New Terminal**.

Ejecuta:

```powershell
mkdir practica6-ml-numpy
cd practica6-ml-numpy
code .
```

**Explicación:**
Se crea la carpeta del proyecto y se abre en VS Code.

---

# 2. Crear el entorno virtual `.venv6`

En la terminal:

```powershell
python -m venv .venv6
```

**Explicación:**
El entorno virtual mantiene las bibliotecas de esta práctica separadas de otros proyectos de Python.

---

# 3. Activar el entorno virtual

En PowerShell:

```powershell
.\.venv6\Scripts\Activate.ps1
```

Debe aparecer:

```text
(.venv6) PS C:\...\practica6-ml-numpy>
```

El texto `(.venv6)` indica que el entorno está activo.

---

# 4. Actualizar pip

```powershell
python -m pip install --upgrade pip
```

**Explicación:**
Actualiza el administrador de paquetes de Python.

---

# 5. Instalar NumPy

```powershell
python -m pip install numpy
```

**Explicación:**
NumPy proporciona arreglos y operaciones numéricas que utilizaremos en los ejercicios.

---

# 6. Instalar Jupyter

```powershell
python -m pip install jupyter
```

**Explicación:**
Jupyter permite crear y ejecutar los archivos `.ipynb`.

---

# 7. Instalar IPykernel

```powershell
python -m pip install ipykernel
```

**Explicación:**
IPykernel permite que Jupyter utilice el Python que se encuentra dentro de nuestro entorno `.venv6`.

---

# 8. Registrar el entorno como kernel

Ejecuta:

```powershell
python -m ipykernel install --user --name practica6-venv6 --display-name "Python (.venv6)"
```

**Explicación:**
Se registra `.venv6` como un kernel disponible para los notebooks.

---

# 9. Verificar NumPy

Ejecuta:

```powershell
python -c "import numpy as np; print('NumPy instalado correctamente'); print('Versión:', np.__version__)"
```

Resultado esperado:

```text
NumPy instalado correctamente
Versión: 2.x.x
```

---

# 10. Verificar Jupyter

```powershell
python -m jupyter --version
```

Debe mostrar las versiones de Jupyter instaladas.

---

# 11. Seleccionar el intérprete de Python

En VS Code presiona:

```text
Ctrl + Shift + P
```

Escribe:

```text
Python: Select Interpreter
```

Selecciona:

```text
Python 3.x.x ('.venv6': venv)
```

**Explicación:**
De esta manera VS Code utilizará el Python del entorno `.venv6`.

---

# 12. Crear los cinco archivos `.ipynb`

En el explorador de VS Code crea:

```text
practica6-ml-numpy/
│
├── .venv6/
│
├── practica6a-0777.ipynb
├── practica6b-0777.ipynb
├── practica6c-0777.ipynb
├── practica6d-0777.ipynb
├── practica6e-0777.ipynb
│
└── requirements.txt
```

Los archivos son:

1. `practica6a-0777.ipynb`
2. `practica6b-0777.ipynb`
3. `practica6c-0777.ipynb`
4. `practica6d-0777.ipynb`
5. `practica6e-0777.ipynb`

---

# 13. Seleccionar el kernel de Jupyter

Abre, por ejemplo:

```text
practica6a-0777.ipynb
```

En la parte superior derecha selecciona:

**Select Kernel**

y después:

```text
Python (.venv6)
```

Haz lo mismo en cada notebook.

> Es importante seleccionar **Python (.venv6)** para que las prácticas utilicen el NumPy instalado en nuestro entorno virtual.

---

# 14. Práctica 6A — Calificaciones

### Situación real

Un profesor desea analizar las calificaciones de cinco alumnos.

Archivo:

```text
practica6a-0777.ipynb
```

### Celda 1 — Importar NumPy

```python
import numpy as np
```

### Celda 2 — Crear los datos

```python
calificaciones = np.array([9, 8, 10, 7, 9])

print("=== CALIFICACIONES ===")
print("Calificaciones:", calificaciones)
```

### Celda 3 — Analizar los datos

```python
promedio = np.mean(calificaciones)
maxima = np.max(calificaciones)
minima = np.min(calificaciones)

print("Promedio:", promedio)
print("Calificación mayor:", maxima)
print("Calificación menor:", minima)
```

### ¿Qué aprende el alumno?

```python
np.mean()
```

Calcula el promedio.

```python
np.max()
```

Obtiene el valor mayor.

```python
np.min()
```

Obtiene el valor menor.

Para ejecutar una celda:

```text
Shift + Enter
```

---

# 15. Práctica 6B — Gastos semanales

### Situación real

Un estudiante registra cuánto dinero gastó durante cinco días.

Archivo:

```text
practica6b-0777.ipynb
```

### Celda 1

```python
import numpy as np
```

### Celda 2

```python
gastos = np.array([50, 35, 80, 45, 60])

print("=== GASTOS SEMANALES ===")
print("Gastos:", gastos)
```

### Celda 3

```python
total = np.sum(gastos)
promedio = np.mean(gastos)
mayor = np.max(gastos)

print("Gasto total: $", total)
print("Gasto promedio: $", promedio)
print("Gasto mayor: $", mayor)
```

### Explicación

`np.sum()` suma los valores:

```python
np.sum(gastos)
```

`np.mean()` obtiene el promedio:

```python
np.mean(gastos)
```

`np.max()` obtiene el gasto más alto:

```python
np.max(gastos)
```

---

# 16. Práctica 6C — Ventas de papelería

### Situación real

Una papelería desea calcular el importe de varios productos vendidos.

Archivo:

```text
practica6c-0777.ipynb
```

### Celda 1

```python
import numpy as np
```

### Celda 2

```python
precios = np.array([35, 10, 250, 8, 15])
cantidades = np.array([5, 10, 2, 15, 6])

print("Precios:", precios)
print("Cantidades:", cantidades)
```

### Celda 3

```python
totales = precios * cantidades

print("=== VENTAS DE PAPELERÍA ===")
print("Totales por producto:", totales)
```

### Celda 4

```python
venta_total = np.sum(totales)

print("Venta total: $", venta_total)
```

### Explicación

NumPy permite realizar operaciones directamente entre arreglos:

```python
totales = precios * cantidades
```

Por ejemplo:

```text
35 × 5   = 175
10 × 10  = 100
250 × 2  = 500
8 × 15   = 120
15 × 6   = 90
```

Después:

```python
np.sum(totales)
```

obtiene la venta total.

---

# 17. Práctica 6D — Temperaturas

### Situación real

Se registran las temperaturas de lunes a viernes para identificar el día más caluroso y el más frío.

Archivo:

```text
practica6d-0777.ipynb
```

### Celda 1

```python
import numpy as np
```

### Celda 2

```python
dias = np.array([
    "Lunes",
    "Martes",
    "Miércoles",
    "Jueves",
    "Viernes"
])

temperaturas = np.array([27, 29, 31, 28, 30])

print("=== TEMPERATURAS ===")
print("Días:", dias)
print("Temperaturas:", temperaturas)
```

### Celda 3

```python
promedio = np.mean(temperaturas)
maxima = np.max(temperaturas)
minima = np.min(temperaturas)

print("Temperatura promedio:", promedio, "°C")
print("Temperatura máxima:", maxima, "°C")
print("Temperatura mínima:", minima, "°C")
```

### Celda 4

```python
posicion_maxima = np.argmax(temperaturas)
posicion_minima = np.argmin(temperaturas)

print("Día con mayor temperatura:", dias[posicion_maxima])
print("Día con menor temperatura:", dias[posicion_minima])
```

### Explicación

`np.argmax()` encuentra la posición del valor máximo.

`np.argmin()` encuentra la posición del valor mínimo.

Por ejemplo:

```python
posicion_maxima = np.argmax(temperaturas)
```

encuentra la posición de `31`.

Después:

```python
dias[posicion_maxima]
```

obtiene:

```text
Miércoles
```

---

# 18. Práctica 6E — Inventario

### Situación real

Una tienda necesita identificar los productos que tienen pocas existencias.

Archivo:

```text
practica6e-0777.ipynb
```

### Celda 1

```python
import numpy as np
```

### Celda 2

```python
productos = np.array([
    "Teclado",
    "Mouse",
    "Monitor",
    "USB"
])

existencias = np.array([8, 20, 4, 15])

print("=== INVENTARIO ===")
print("Productos:", productos)
print("Existencias:", existencias)
```

### Celda 3

```python
total = np.sum(existencias)

print("Existencias totales:", total)
```

### Celda 4

```python
filtro = existencias < 10

print("=== PRODUCTOS CON MENOS DE 10 UNIDADES ===")
print(productos[filtro])
print(existencias[filtro])
```

### Explicación

Creamos una condición:

```python
filtro = existencias < 10
```

El resultado identifica los valores menores que 10.

Después:

```python
productos[filtro]
```

muestra únicamente los productos que cumplen la condición.

---

# 19. Ejecutar las cinco prácticas

En cada notebook:

1. Abrir el archivo `.ipynb`.
2. Seleccionar **Python (.venv6)**.
3. Ejecutar la primera celda con `Shift + Enter`.
4. Ejecutar las siguientes celdas.
5. Revisar el resultado.
6. Guardar el notebook.

Los cinco archivos serán:

```text
practica6a-0777.ipynb
practica6b-0777.ipynb
practica6c-0777.ipynb
practica6d-0777.ipynb
practica6e-0777.ipynb
```

---

# 20. Crear `requirements.txt`

Con `.venv6` activado:

```powershell
python -m pip freeze > requirements.txt
```

Esto registra las bibliotecas instaladas en el entorno.

---

# 21. Estructura final del proyecto

```text
practica6-ml-numpy/
│
├── .venv6/
│   └── ...
│
├── practica6a-0777.ipynb
├── practica6b-0777.ipynb
├── practica6c-0777.ipynb
├── practica6d-0777.ipynb
├── practica6e-0777.ipynb
│
└── requirements.txt
```

---

## 22. Comandos completos de instalación

Para que el alumno tenga todos los comandos juntos:

```powershell
mkdir practica6-ml-numpy
cd practica6-ml-numpy
code .

python -m venv .venv6

.\.venv6\Scripts\Activate.ps1

python -m pip install --upgrade pip

python -m pip install numpy

python -m pip install jupyter

python -m pip install ipykernel

python -m ipykernel install --user --name practica6-venv6 --display-name "Python (.venv6)"

python -c "import numpy as np; print('NumPy:', np.__version__)"

python -m jupyter --version

python -m pip freeze > requirements.txt
```

### Resultado esperado

Al finalizar, el alumno tendrá cinco notebooks funcionales para practicar:

**calificaciones → gastos → ventas → temperaturas → inventario**

y habrá utilizado los principales fundamentos iniciales de NumPy:

```text
np.array()
np.sum()
np.mean()
np.max()
np.min()
np.argmax()
np.argmin()
operaciones entre arreglos
filtros booleanos
```

Estos ejercicios sirven como introducción al manejo de datos numéricos que posteriormente se utilizarán en algoritmos de **Machine Learning**.
