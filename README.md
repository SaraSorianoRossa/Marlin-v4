## Descripción general
Esta implementación viene dada a través de realizar una modificación a la [tercera versión](https://github.com/SaraSorianoRossa/Marlin-v3) del [algoritmo de Marlin](https://github.com/arkworks-rs/marlin). 
Una vez completada la versión anterior donde se eliminó el envio del compromiso del polinomio $t(X)$, se observó que el siguiente paso sería eliminar el polinomio $s(x)$. 
Para ello se modificaron los polinomios calculados por el probador, en los cuales este polinomio formaba parte. 
Después de realizar las modificaciones se observó que eliminando este polinomio no se puede asegurar que haya un conocimiento nulo al completo, se debería realizar una modificación al circuito que viene dado.
Este dato nos permitió establecer un siguiente paso que sería necesario realizar, pero que por falta de conocimientos no se pudo conseguir a pesar de conocer la solución.

Como siguiente paso de esta última modificación, se ha definido un [nuevo proceso inner](https://github.com/SaraSorianoRossa/New-inner) en el cual se comprueba la veracidad de la abertura del polinomio $t(X)$.

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
