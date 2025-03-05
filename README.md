# OpenMP-MPI

Este proyecto contiene el desarrollo y análisis de dos algoritmos aplicando distintas técnicas de optimización(paralelización).

En cuanto la estructura de directorios,sigue una forma simple y eficiente. Los distintos directorios son:

    ·Code: Contiene los códigos en C, que se necesitan para las ejecuciones del algoritmo, tanto sin optimización, como con estas(OpenMP,MPI y OpenMP&MPI).
    ·Plots: Contiene las gráficas dónde se comparan los rendimientos de las distintas ejecuciones.
    ·Resuts: Contiene los resultados de las ejecuciones en formato .txt, los cuales se usarán para generar los CSVs y gráficas.
    ·Results_csv: Contiene los directorios con los resultados por tipo de ejecución además de las gráficas por tipo.
    ·data_processor.ipynb: Es un Notebook en el cual se realizan procesamientos sobre los resultados adquiridos para mejorar la limpieza de datos, análisis,
    creación e interpretación de gráficas. Las distintas funciones se explican línea a línea en el documento.

Los algoritmos a estudiar son distintas estimaciones de pi, la primera mediante rectángulos y el segundo usando el algoritmo de Montecarlo.

El estudio constaba de comprobar la estimación de tiempo de los distintos algoritmos:

    · Básico: Se lanza el algoritmo sin ningún tipo de paralelización.
    · OpenMP: Se lanza el algoritmo modificado para usar la librería openMP de C. Probando hasta 16 hilos.
    · MPI: Se lanza el algoritmo modificado para usar la librería MPI de C. En este caso se lanzó con una máquina virtual con acceso a un cluster
    pudiendo paralelizar el proceso en 8 partes.
    · OpenMP&MPI: En esta parte se desarrolló un código que permitió lanzar el algoritmo con ambas librerías para obtener el máximo rendimiento.