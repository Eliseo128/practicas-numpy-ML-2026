Claro. Para esta **Práctica 6 de Machine Learning con NumPy**, mantendremos el mismo procedimiento utilizado en la práctica anterior, pero ahora trabajaremos exclusivamente con **NumPy** y cinco situaciones sencillas de la vida real.

# Práctica 6 — Machine Learning con NumPy desde VS Code

**Nivel:** 3.er semestre de preparatoria
**Carpeta:** `practica6-ml-numpy`
**Entorno virtual:** `.venv6`
**Biblioteca:** NumPy
**Editor:** Visual Studio Code

> Nota: en tu solicitud aparece “utilizar pandas”, pero por el contexto de la práctica se trabajará con **NumPy**, que es la biblioteca indicada para esta Práctica 6.

---

## 1. Crear la carpeta de trabajo

Abre **VS Code → Terminal → New Terminal** y ejecuta:

```powershell
mkdir practica6-ml-numpy
cd practica6-ml-numpy
code .
```

### ¿Qué hacemos?

* `mkdir` crea la carpeta.
* `cd` entra en la carpeta.
* `code .` abre el proyecto en VS Code.

---

## 2. Crear el entorno virtual `.venv6`

En la terminal:

```powershell
python -m venv .venv6
```

### ¿Qué hacemos?

Creamos un entorno virtual independiente para instalar NumPy solamente en este proyecto.

---

## 3. Activar el entorno virtual

En PowerShell:

```powershell
.\.venv6\Scripts\Activate.ps1
```

Si se activó correctamente, aparecerá:

```text
(.venv6) PS C:\...\practica6-ml-numpy>
```

El indicador `(.venv6)` confirma que el entorno está activo.

---

## 4. Actualizar pip

Ejecuta:

```powershell
python -m pip install --upgrade pip
```

Esto actualiza el administrador de paquetes de Python.

---

## 5. Instalar NumPy

Ejecuta:

```powershell
python -m pip install numpy
```

NumPy permite trabajar con **arreglos, vectores, matrices y operaciones numéricas**, elementos fundamentales para posteriormente estudiar Machine Learning.

---

## 6. Verificar la instalación

Ejecuta:

```powershell
python -c "import numpy as np; print('NumPy instalado correctamente'); print('Versión:', np.__version__)"
```

Debe aparecer algo similar a:

```text
NumPy instalado correctamente
Versión: 2.x.x
```

---

# 7. Seleccionar el intérprete de Python en VS Code

Presiona:

```text
Ctrl + Shift + P
```

Busca:

```text
Python: Select Interpreter
```

Selecciona el Python correspondiente a:

```text
.venv6
```

Por ejemplo:

```text
Python 3.x.x ('.venv6': venv)
```

### ¿Por qué es importante?

VS Code utilizará el Python del entorno `.venv6`, donde acabamos de instalar NumPy.

---

# 8. Estructura del proyecto

Crea los siguientes archivos:

```text
practica6-ml-numpy/
│
├── .venv6/
│
├── practica6a-0777.py
├── practica6b-0777.py
├── practica6c-0777.py
├── practica6d-0777.py
├── practica6e-0777.py
│
└── requirements.txt
```

Los cinco programas utilizarán NumPy.

| Archivo              | Situación de la vida real | Conceptos                 |
| -------------------- | ------------------------- | ------------------------- |
| `practica6a-0777.py` | Calificaciones            | promedio, máximo y mínimo |
| `practica6b-0777.py` | Gastos semanales          | suma y promedio           |
| `practica6c-0777.py` | Ventas                    | operaciones con arreglos  |
| `practica6d-0777.py` | Temperaturas              | máximo, mínimo y promedio |
| `practica6e-0777.py` | Inventario                | filtros y operaciones     |

---

# 9. Práctica 6A — Calificaciones

**Situación:** analizar las calificaciones de cinco alumnos.

Archivo:

```text
practica6a-0777.py
```

Código completo:

```python
import numpy as np

calificaciones = np.array([9, 8, 10, 7, 9])

print("=== CALIFICACIONES ===")
print("Calificaciones:", calificaciones)

promedio = np.mean(calificaciones)
maxima = np.max(calificaciones)
minima = np.min(calificaciones)

print("Promedio:", promedio)
print("Calificación mayor:", maxima)
print("Calificación menor:", minima)
```

### Explicación

```python
import numpy as np
```

Importa NumPy y utiliza `np` como nombre corto.

```python
calificaciones = np.array([9, 8, 10, 7, 9])
```

Crea un arreglo NumPy.

```python
np.mean(calificaciones)
```

Calcula el promedio.

```python
np.max(calificaciones)
```

Obtiene la calificación mayor.

```python
np.min(calificaciones)
```

Obtiene la calificación menor.

### Ejecutar

```powershell
python practica6a-0777.py
```

---

# 10. Práctica 6B — Gastos semanales

**Situación:** analizar los gastos realizados durante cinco días.

Archivo:

```text
practica6b-0777.py
```

Código:

```python
import numpy as np

gastos = np.array([50, 35, 80, 45, 60])

print("=== GASTOS SEMANALES ===")
print("Gastos:", gastos)

total = np.sum(gastos)
promedio = np.mean(gastos)
mayor = np.max(gastos)

print("Gasto total: $", total)
print("Gasto promedio: $", promedio)
print("Gasto mayor: $", mayor)
```

### Explicación

```python
gastos = np.array([50, 35, 80, 45, 60])
```

Representa los gastos de lunes a viernes.

```python
np.sum(gastos)
```

Suma todos los gastos.

```python
np.mean(gastos)
```

Calcula el gasto promedio.

```python
np.max(gastos)
```

Encuentra el gasto más alto.

Ejecutar:

```powershell
python practica6b-0777.py
```

---

# 11. Práctica 6C — Ventas de una papelería

**Situación:** calcular el importe de diferentes productos vendidos.

Archivo:

```text
practica6c-0777.py
```

Código:

```python
import numpy as np

precios = np.array([35, 10, 250, 8, 15])
cantidades = np.array([5, 10, 2, 15, 6])

totales = precios * cantidades

print("=== VENTAS DE PAPELERÍA ===")

print("Precios:", precios)
print("Cantidades:", cantidades)
print("Totales por producto:", totales)

print("Venta total: $", np.sum(totales))
```

### Explicación

Tenemos dos arreglos:

```python
precios = np.array([35, 10, 250, 8, 15])
```

y:

```python
cantidades = np.array([5, 10, 2, 15, 6])
```

NumPy permite multiplicarlos directamente:

```python
totales = precios * cantidades
```

Por ejemplo:

```text
35 × 5 = 175
10 × 10 = 100
250 × 2 = 500
```

Finalmente:

```python
np.sum(totales)
```

calcula la venta total.

Ejecutar:

```powershell
python practica6c-0777.py
```

---

# 12. Práctica 6D — Temperaturas

**Situación:** analizar las temperaturas registradas durante cinco días.

Archivo:

```text
practica6d-0777.py
```

Código:

```python
import numpy as np

temperaturas = np.array([27, 29, 31, 28, 30])

print("=== TEMPERATURAS ===")
print("Temperaturas:", temperaturas)

promedio = np.mean(temperaturas)
maxima = np.max(temperaturas)
minima = np.min(temperaturas)

dia_maximo = np.argmax(temperaturas)
dia_minimo = np.argmin(temperaturas)

dias = np.array(["Lunes", "Martes", "Miércoles", "Jueves", "Viernes"])

print("Temperatura promedio:", promedio, "°C")
print("Temperatura máxima:", maxima, "°C")
print("Día con mayor temperatura:", dias[dia_maximo])
print("Temperatura mínima:", minima, "°C")
print("Día con menor temperatura:", dias[dia_minimo])
```

### Explicación

```python
np.argmax(temperaturas)
```

encuentra la posición donde se encuentra el valor máximo.

```python
np.argmin(temperaturas)
```

encuentra la posición donde está el valor mínimo.

Después utilizamos esa posición para obtener el día:

```python
dias[dia_maximo]
```

Ejecutar:

```powershell
python practica6d-0777.py
```

---

# 13. Práctica 6E — Inventario

**Situación:** identificar productos con pocas existencias.

Archivo:

```text
practica6e-0777.py
```

Código:

```python
import numpy as np

productos = np.array(["Teclado", "Mouse", "Monitor", "USB"])
existencias = np.array([8, 20, 4, 15])

print("=== INVENTARIO ===")

print("Productos:", productos)
print("Existencias:", existencias)

total = np.sum(existencias)

print("Existencias totales:", total)

print("\nProductos con menos de 10 unidades:")

filtro = existencias < 10

print(productos[filtro])
print(existencias[filtro])
```

### Explicación

Creamos los productos:

```python
productos = np.array(["Teclado", "Mouse", "Monitor", "USB"])
```

Y sus existencias:

```python
existencias = np.array([8, 20, 4, 15])
```

Creamos una condición:

```python
filtro = existencias < 10
```

NumPy identifica cuáles valores son menores que 10.

Después:

```python
productos[filtro]
```

muestra únicamente los productos que cumplen la condición.

Ejecutar:

```powershell
python practica6e-0777.py
```

---

# 14. Crear `requirements.txt`

Después de instalar NumPy, puedes generar automáticamente el archivo:

```powershell
python -m pip freeze > requirements.txt
```

La estructura final queda:

```text
practica6-ml-numpy/
│
├── .venv6/
│
├── practica6a-0777.py
├── practica6b-0777.py
├── practica6c-0777.py
├── practica6d-0777.py
├── practica6e-0777.py
│
└── requirements.txt
```

---

# 15. Procedimiento general para el alumno

El flujo de trabajo de la práctica es:

```text
Crear carpeta
      ↓
Crear .venv6
      ↓
Activar .venv6
      ↓
Actualizar pip
      ↓
Instalar NumPy
      ↓
Verificar NumPy
      ↓
Seleccionar intérprete .venv6
      ↓
Crear 5 archivos .py
      ↓
Escribir los programas
      ↓
Ejecutar cada programa
      ↓
Analizar los resultados
      ↓
Crear requirements.txt
```

## 16. Comandos principales

Una vez abierta la terminal de VS Code:

```powershell
mkdir practica6-ml-numpy
cd practica6-ml-numpy
code .

python -m venv .venv6

.\.venv6\Scripts\Activate.ps1

python -m pip install --upgrade pip

python -m pip install numpy

python -c "import numpy as np; print(np.__version__)"

python -m pip freeze > requirements.txt
```

Y para ejecutar las prácticas:

```powershell
python practica6a-0777.py
python practica6b-0777.py
python practica6c-0777.py
python practica6d-0777.py
python practica6e-0777.py
```

### Conceptos de NumPy que practicarán

Con estos cinco ejercicios los alumnos comienzan a trabajar con:

* `np.array()`
* `np.sum()`
* `np.mean()`
* `np.max()`
* `np.min()`
* `np.argmax()`
* `np.argmin()`
* operaciones entre arreglos
* filtros booleanos
* arreglos numéricos y de texto

Estos conceptos constituyen una base práctica para posteriormente trabajar con **datos, matrices y operaciones numéricas utilizadas en Machine Learning**.
