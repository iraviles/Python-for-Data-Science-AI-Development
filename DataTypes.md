Perfecto, vamos a comenzar con la documentación. Aquí está la estructura inicial en markdown para el tema de **Tipos de Datos en Python**.

### Tipos de Datos en Python

#### 1. Introducción a los Tipos de Datos en Python

En Python, los tipos de datos definen la naturaleza de los valores que se pueden almacenar y manipular. Comprender los tipos de datos es esencial para trabajar con variables y estructuras de datos. Python es un lenguaje de tipado dinámico, lo que significa que no es necesario declarar el tipo de una variable al momento de crearla.

Los principales tipos de datos en Python son:

- **Numéricos**: enteros (`int`), flotantes (`float`).
- **Secuencias**: cadenas de texto (`str`), listas (`list`), tuplas (`tuple`).
- **Booleanos**: `bool` (valores `True` y `False`).
- **Colecciones**: diccionarios (`dict`).
  
Vamos a explorar cada uno de estos tipos a continuación.

#### 2. Tipos de Datos Numéricos

##### 2.1 Enteros (`int`)

Un **entero** es un número sin decimales. Pueden ser positivos o negativos.

**Ejemplo:**

```python
x = 5        # un número entero positivo
y = -3       # un número entero negativo
z = 0        # cero también es un entero
```

##### 2.2 Flotantes (`float`)

Un **flotante** es un número que tiene una parte decimal. Se utilizan para representar números reales.

**Ejemplo:**

```python
a = 3.14     # un número flotante positivo
b = -2.5     # un número flotante negativo
c = 0.0      # un número flotante igual a cero
```

##### 2.3 Operaciones con Números

Python permite realizar operaciones matemáticas básicas con números. Algunos ejemplos incluyen:

**Ejemplo:**

```python
# Suma
x = 5 + 3  # resultado: 8

# Resta
y = 5 - 3  # resultado: 2

# Multiplicación
z = 5 * 3  # resultado: 15

# División
w = 5 / 2  # resultado: 2.5 (siempre devuelve flotante)

# División entera (descarta la parte decimal)
q = 5 // 2  # resultado: 2

# Módulo (resto de la división)
r = 5 % 2   # resultado: 1

# Potenciación
p = 2 ** 3  # resultado: 8
```

#### 3. Cadenas de Texto (`str`)

Una **cadena de texto** es una secuencia de caracteres. Se define entre comillas simples (`'`) o dobles (`"`).

**Ejemplo:**

```python
mensaje = "Hola, Mundo!"  # cadena de texto con comillas dobles
saludo = 'Hola'           # cadena de texto con comillas simples
```

##### Métodos Comunes para Cadenas

- `.lower()`: Convierte la cadena a minúsculas.
- `.upper()`: Convierte la cadena a mayúsculas.
- `.split()`: Divide la cadena en una lista de palabras.

**Ejemplo:**

```python
texto = "Hola, Python"
print(texto.lower())  # salida: 'hola, python'
print(texto.upper())  # salida: 'HOLA, PYTHON'

# Dividir la cadena por espacios
palabras = texto.split()  
print(palabras)  # salida: ['Hola,', 'Python']
```

#### 4. Tipos Booleanos (`bool`)

El tipo **booleano** tiene solo dos valores posibles: `True` y `False`. Se utilizan comúnmente en condiciones y bucles.

**Ejemplo:**

```python
es_adulto = True
es_nino = False

if es_adulto:
    print("Es un adulto")
else:
    print("No es un adulto")
```

#### 5. Tipos de Datos Compuestos

##### 5.1 Listas (`list`)

Una **lista** es una colección ordenada de elementos. Puede contener elementos de diferentes tipos.

**Ejemplo:**

```python
frutas = ["manzana", "plátano", "cereza"]
print(frutas[0])  # salida: 'manzana'
```

##### 5.2 Tuplas (`tuple`)

Una **tupla** es similar a una lista, pero es **inmutable**. Una vez creada, no puedes modificar sus elementos.

**Ejemplo:**

```python
coordenadas = (10, 20)
print(coordenadas[1])  # salida: 20
```

##### 5.3 Diccionarios (`dict`)

Un **diccionario** es una colección no ordenada de pares clave-valor.

**Ejemplo:**

```python
persona = {"nombre": "Juan", "edad": 30}
print(persona["nombre"])  # salida: 'Juan'
```

#### 6. Conversión de Tipos de Datos

A veces, es necesario convertir entre diferentes tipos de datos. Python proporciona funciones como `int()`, `float()`, y `str()` para convertir valores entre tipos.

**Ejemplo:**

```python
# Convertir a entero
num_str = "123"
num = int(num_str)  # ahora num es un entero
print(num)  # salida: 123

# Convertir a flotante
num_float = float(num_str)  # ahora num_float es un flotante
print(num_float)  # salida: 123.0

# Convertir a cadena
num_str2 = str(num)  # convierte el número a cadena
print(num_str2)  # salida: '123'
```

#### 7. Resumen y Tabla de Tipos de Datos

| Tipo de Dato   | Descripción                                        | Ejemplo                         |
|----------------|----------------------------------------------------|---------------------------------|
| `int`          | Números enteros sin decimales                      | `5`, `-3`, `0`                  |
| `float`        | Números con decimales                              | `3.14`, `-2.5`, `0.0`           |
| `str`          | Cadenas de texto                                   | `"Hola"`, `'Python'`            |
| `bool`         | Valores booleanos (`True` o `False`)               | `True`, `False`                 |
| `list`         | Colección ordenada de elementos                    | `[1, 2, 3]`, `["a", "b"]`       |
| `tuple`        | Colección ordenada e inmutable de elementos        | `(1, 2, 3)`, `("a", "b")`       |
| `dict`         | Colección de pares clave-valor                     | `{"clave": "valor"}`            |

---


