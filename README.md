## Descripción general
Esta implementación viene dada a través de realizar una modificación a la [primera versión](https://github.com/SaraSorianoRossa/Marlin-v1). 
La modificación que se ha realizado consiste en eliminar la fase de inner del [algoritmo de Marlin](https://github.com/arkworks-rs/marlin). 
Es decir, suprimir las funciones tanto del probador como del verificador que implicaban estos envíos y de realizar cambios en el resto de funciones para hacerlo posible. 
Además, la sección correspondiente que permitía al verificador verificar el inner_sumcheck también se eliminó del archivo mod.rs. 
En definitiva, esta modificación ha consistido en identificar las diferentes funciones y partes que se programaron para conseguir hacer la fase del inner en Marlin.

A esta implementación se han realizando nuevas modificaciones con tal de poder obtener un mejor rendimiento del algoritmo de Marlin:
1. [Segunda modificación](https://github.com/SaraSorianoRossa/Marlin-v3)
2. [Tercera modificación](https://github.com/SaraSorianoRossa/Marlin-v4)

Además de estas modificaciones se ha definido un [nuevo proceso inner](https://github.com/SaraSorianoRossa/New-inner) en el cual se comprobaba la veracidad de la abertura del polinomio $t(X)$.

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
