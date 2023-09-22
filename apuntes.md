# Pedro Andrés Castillo Gildo - Ingenieria en computacion inteligente - Universidad de Colima - Semestre 3 grupo B - Facultad de Ingenieria Mecanica y Electrica - 
## Apuntes de Notas en clase de Programacion Funcional en Python
### Operadores logicos
```python
True
False
if 5 > 4:
    print(True)
print(5>7)

received: bool = False
not received
```

```python
nombre: str = 'hugo'
print(nombre)
print(type(nombre))
nombre.capitalize()
nombre.upper()
```
```python
num: int = 10
pi: float = 3.14
es_alumno: bool = True
name: str = 'Hugo'
print(f'{num}--{pi}--{es_alumno}--{name.upper()}')
```
```python
print(True and False)
print(True or False)
print(not False)
````

### Operadores Aritmeticos
```python
print(5+4)
print(5-4)
print(5*4)
print(5/4)
print(5//4) # division entera
print(5%4) # modulo o residuo
print(5**4) # x a la y
```

### Condicionales
```python
n1: int = 30
n2: int = 20
if n1>n2:
    print(f'{n1} > {n2}')
```
```python

n1=10
if n1>n2:
    print(f'{n1} > {n2}')
else:
    print(f'{n2} > {n1}')
```

```python
edad: int = 18
if edad > 18:
    print('mayor de edad')
elif edad == 18:
    print('acabas de llegar a la mayoria de edad')
else:
    print('eres menor de edad')
```

```python
match True:
    case 18:
        print('acabas de llegar a la mayoria de edad')
        case edad
```
### Tipos de datos
```python
mensaje: str = "Hi"             #Las mayusculas estan designadas para las clases
numero: float = 3.1416
otro_numero: int = 15    
apellido_paterno = " "
apellidoPaterno = "Asi no se hace nunca en python"
```

```python
#num = ""
n = int(input("Dame un numero entero positivo"))
if n%2 == 0:
    num = "Par"
else:
    num = "Impar"

num
```

```python
n = int(input("Dame un numero entero positivo"))
(num := "Par" if n%2 == 0 else "Impar")
num
```

```python
(num := "par" if int(input("dame un numero entero posaitivo"))%2 == 0 else "impar")
num
```

```
suma = a+b
```

```python
#Casting
#conversion de tipos
num_str = "3"
num_int = int(num_str)
print(f"num_int: {num_int}") #fstrings

num_float = 3.14
num_int = int(num_float)
print(f"num_int: {num_int}")

def res():
    num_str = "3"
    num_int = 10
    return (num_str, num_int)

num_str = str(num_float)
res_tupla = (num_str, num_int)
print(f"num_str: {res()}")
print(f"res: %s %d" % res())
num_str

a, b = res()
print(f"res: {a} {b}")
```
### Logicos Bool
```python
True
False
if 5 > 4:
    print("True")

print(5>7)

received: bool = False
not received
```

### Cadena String
```python
nombre: str = "pedro" #Python es un lenguaje interpretado
nombre #Compilados manejan mejor la memoria
print(type(nombre)) #Todas las clases tienen propiedades y tienen objetos
nombre.capitalize()
nombre.upper()
```

```python
num: int = 10
pi:float = 3.14
es_alumno: bool = True
name:str = "Alex"

print(f"{num}-{pi}-{es_alumno}-{name}")
```

### Listas
```python
# Listas 
# Colecciones (colections)

def suma(a, b):
    return a + b 
def resta(a, b):
    return a - b
def multiplicacion(a, b):
    return a * b
def division(a, b):
    return a / b

operaciones = [suma, resta, multiplicacion, division]
print(operaciones[0](5,4))
print(operaciones[1](5,4))
print(operaciones[2](5,4))
print(operaciones[3](5,4))

for operacion in operaciones:
    print(operacion(5, 4))

Lista = [1, 2, 3, 4, 5, True, 4.5, "hola", [1, 2, 3]]
```
```python
# La lista es indexable osea que todos los valores tienen posicion y son mutables y pueden contener cualquier tipo de dato
Lista[8]
```

```python
Lista[8]="Hola mundo"
Lista
```
```python
#slices
print(Lista)
print(Lista[:])
```

```python
print(Lista[0:])
```

```python
print(Lista[:-1])
```

```python
def suma(a, b): #una funcion siempre debe de retornar algo, una caracteristicas de las listas
    pass

print(suma(3, 4))
```

```python
def operaciones(a, b):
    return [a+b, a-b, a*b, a/b]

respuestas = operaciones(5, 4)
print(respuestas)
w, x, y, z = operaciones(5, 4)
print(w)
```

```python
res_suma,_,_,_ = operaciones(5, 4)
res_suma
```

```python
lista = [3, 6, 7, 40, 34, 67, 89]
max(lista)
```

```python
sum(lista)
min(lista)
sorted(lista)
lista.sort()
lista
print(lista.sort())
lista.sort(reverse=True)
lista
```

### Set
```python
# set conjuntos en python asi podemos eliminar los elementos repetidos en orden 1

mi_set = {1, 2, 3, 3, 3, 3, 3}
mi_set
```

### Data
```python
data = [15, 14, 13, 12, 11, 10, 1, 2, 3, 4, 5, 6, 7, 8, 9, 1, 2, 1, 2, 1, 2, 1, 2, 1, 2]

set(data) #datos no repetidos en una misma linea en orden 1
```

```python
data2 = {1, 56, 57, 58}

mi_set.union(data2)
```

### Diccionarios
```python
# diccionarios
mi_dict = {"llave": "valor"}
mi_dict["llave"]
```

```python
mi_dict.keys()
```

```python
mi_dict.values()
```

```python
do a dict
```

### Tuplas
# Tuplas tuple son inmutables, no puedes cambiarle los datos
```python
tupla_funciones = (suma, resta , multiplicacion, division)
print(tupla_funciones[1](5, 4))

tupla = (1, 2, 3, 4, 5, True, 4.5, "hola" , [1, 2, 3])
```

```python
Lista.append[10]
Lista

```
```python
tupla.__add__((10,10))
tupla[0].__mod__(2)
```

```python
def suma(a: int, b: int) -> int:
    return a + b 

def operacion(a: int, b: int) -> (int, int):
    return (a+b, a-b)

(a, b) = operacion(5, 6)
a,b = operacion(6, 5)
print(a, b)
```

### Uso de range
```python
#range

numeros = range(10)
print(numeros)
```

```python
for i in numeros:
    print(i, end="")
```

```python
numeros = range(5, 10)
```

```python
for i in numeros:
    print(i, end=",")
```

```python
numeros_pares = range (2,11,2)
for par in numeros_pares:
    print(par, end=" ")
```

```python
for item in range(2,11,2):
    print(item, end=" ")
```

### Funcion suma y resta
```python
def suma(a: int, b: int)->int: #pistas
    return a + b

if __name__== "__main__":
    print(suma(5,6))

```

```python
def resta(a: int, b: int)-> int:
    return a + b

if __name__== "__main__":
    print(resta(8,4))
```
#### Importamos la carpeta en la que se encuentran ambas funciones
```python
""" import milibreria.suma as lib
import milibreria.resta as lib """
""" import milibreria as lib """
from milibreria import suma, resta

def suma1(a: float, b:float)->float:
    return a + b

def suma2(a: float, b:float)->float:
    return a + b

def suma(a: int|float, b:int|float)-> int|float:
    return a + b

if __name__== "__main__":
    print(suma(5,6.5))
    print(suma1(5,6))
    print(suma2(5.3,6.4))
```

### Uso de streamlit en python
#### Uso de @dataclass
#### Agenda hecha en python usando streamlit
```python
# funcion decorador se utiliza para modificar el comportamiento de otra funcion

from dataclasses import dataclass

@dataclass #decorators
class User:
    id: str
    name: str
    age: int

    def show_data(self):
        return f"ID: {self.id}\nNOMBRE: {self.name}\nAÑO: {self.age}"

if __name__ == "__main__":
    usuario1 = User("1","Pedro",25)
    usuario2 = User("2","Andrés",25)
    usuario3 = User("3","Castillo",25)
    usuario4 = User("4","Gildo",25)
    usuarios = [usuario1,usuario2,usuario3,usuario4]
    for usuario in usuarios:
        print(usuario.show_data())
```
#### Calculadora hecha en python haciendo uso de streamlit
```python
import streamlit as st
st.sidebar.title("CALCULADORA ICI")

def pedir_valores():
    name = st.text_input("NOMBRE: ")
    n1 = st.number_input("NUMERO 1")
    n2 = st.number_input("NUMERO 2")

    if st.button("SUMAR"):
        st.success(f"HOLA {name}")
        st.write(f"{n1} + {n2} = {n1+n2}")
    elif st.button("RESTAR"):
        st.success(f"HOLA {name}")
        st.write(f"{n1} - {n2} = {n1-n2}")


opcion = st.sidebar.selectbox("opciones:",[
    "SUMA","RESTA","MULTIPLICACION","DIVISION","ACERCA DE"
])

match opcion:
    case "SUMA":
        st.write("ESTA ES LA SUMA DE...")
        pedir_valores()
    case "RESTA":
        st.write("ESTA ES LA RESTA DE...")
        pedir_valores()
    case "MULTIPLICACION":
        st.write("ESTA ES LA MULTIPLICACION DE...")
    case "DIVISION":
        st.write("ESTA ES LA DIVISION DE...")
    case "ACERCA DE":
        st.write("DERECHOS RESERVADOS")
        st.write("UCOL-FIME-ICI")
```
