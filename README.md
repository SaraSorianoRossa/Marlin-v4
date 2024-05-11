## Descripción general
Esta implementación viene dada a través de realizar una modificación a la [tercera versión](https://github.com/SaraSorianoRossa/Marlin-v3) del [algoritmo de Marlin](https://github.com/arkworks-rs/marlin). 
Una vez completada la versión anterior donde se eliminó el envío del compromiso del polinomio $t(X)$, se ha observado que el siguiente paso debe ser eliminar el polinomio $s(x)$. 
Para ello se han modificado los polinomios calculados por el probador, en los cuales este polinomio formaba parte. 
Después de realizar las modificaciones se ha visto que eliminando este polinomio no se puede asegurar que haya un conocimiento nulo al completo. Por lo tanto, para conseguirlo se debe realizar una modificación al circuito que viene dado.
Este dato nos ha permitido establecer el siguiente paso que sería necesario realizar, pero que por falta de conocimientos no se pudo conseguir a pesar de conocer la solución.

Con el fin de poder demostrarle al verificador que toda la prueba es verídica se ha definido un [nuevo proceso inner](https://github.com/SaraSorianoRossa/New-inner).

## Ejecutar
Para ejecutar este programa es necesario tener previamente instalado cargo y rust. Una vez se tienen instaladas las librerías necesarias para poder ejecutar la prueba con esta versión es necesario estar en el directorio y escribir en la terminal:
```sh
cargo build --release
```

## Testear
En esta versión, igual que en el resto, se ofrece una serie de funciones para testear. Si se desea ejecutarlas para ver el resultado de ellas:
```sh
cargo test
```

## Todas las implementaciones
1. [Versión original](https://github.com/SaraSorianoRossa/Marlin-v1)
2. [Primera modificación](https://github.com/SaraSorianoRossa/Marlin-v2)
3. [Segunda modificación](https://github.com/SaraSorianoRossa/Marlin-v3)
4. [Tercera modificación](https://github.com/SaraSorianoRossa/Marlin-v4)
5. [Nuevo proceso inner](https://github.com/SaraSorianoRossa/New-inner)
