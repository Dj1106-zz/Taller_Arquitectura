# Multiplicación de Matrices: Naive y Strassen

Este repositorio contiene implementaciones del problema clásico de multiplicación de matrices cuadradas utilizando dos algoritmos principales:
Algoritmo Naive (Clásico)
Algoritmo de Strassen (Recursivo)

Las implementaciones están desarrolladas en cuatro lenguajes diferentes para facilitar el análisis comparativo y la práctica:
Python
Java
C
C++
Contenido del Repositorio
Carpetas / Archivos


**Descripción General de los Algoritmos**

Naive:Multiplicación clásica con tres bucles anidados. Sencillo pero con complejidad O(n³).

Strassen:Algoritmo recursivo que reduce el número de multiplicaciones mediante división y combinaciones lineales. más eficiente para matrices grandes.

**Detalle por Lenguaje y Archivos**
# Java
Multiplicación bloqueada para optimización de caché.
Algoritmo de Strassen recursivo.
Tamaños de matriz probados: [128, 256, 512, 1024].
Mide tiempo de CPU y consumo de memoria.

Compilar y Ejecutar
javac -d out src/Matrices/Matriz.java
java -cp out Matrices.Matriz

# python
Ejecuta pruebas en tamaños [128, 256, 512, 1024].

Mide tiempo con time y memoria con tracemalloc.

Exporta resultados a resultados.csv.

Verifica que los resultados de Naive y Strassen coincidan.

Ejecutar:
python multiplicacion_matrices.py


# /c/
Solicitan tamaño de matriz al usuario.
Imprimen matrices si el tamaño es ≤ 10.
Miden tiempo de CPU y memoria estimada.

Ejecutar:
gcc Naive.c -o naive
./naive
gcc Strassen.c -o strassen
./strassen

# /cpp/
C++ — Naive.cpp y Strassen.cpp
Uso de vector para matrices.

Medición de tiempo con <chrono>.

Solicitan tamaño de matriz al usuario.

Ejecutar:

g++ Naive.cpp -o naive_cpp

./naive_cpp

g++ Strassen.cpp -o strassen_cpp

./strassen_cpp

# Notas Importantes
-Strassen tiende a ser más eficiente con matrices grandes en términos de tiempo.

-El algoritmo Strassen funciona mejor con tamaños de matriz que sean potencias de 2; el código agrega padding si es necesario.

-No imprimas matrices grandes para evitar sobrecargar la consola.

-Optimiza el rendimiento en Java ajustando el tamaño del bloque de multiplicación.


