# Escuela Colombiana de ingenieria Julio Garavito
# Ciencias naturales y tecnologia                 23/10/2019
# Sistema cuantico de particula en una linea

## Calculadora cuantica

En este proyecto contiene los nuevos metodos de particula en una recta y calculadora estadistica para observables estos se encuentra en la clase calculator en la linea 235 y 258 respectivamente

particula en una recta:
para este metodo se uso la siguiente  formula:
![imagen](https://i.ibb.co/mzMg4mv/Captura.png)

Para desarrollar esta formula se saco primero la norma del vector al cuadrado, luego se cada numero del mismo vector se le saco
el modulo al cuadrado y se dividio por la norma del vector al cuadrado, todos los resultados se almacenan en una lista para enviarla
al metodo que construlle el diagrama de barras

calculadora estadistica para observables:
Para desarrollar esta funcion se hizo uso de las siguientes formulas:

![imagen](https://i.ibb.co/VT4xq5h/Captura2.png)
Para desarrollar estas formulas:<br/> 
* ingresaron la matriz omega y el vector phi<br/>
*luego normalizamos el phi creando un nuevo metodo en la clase ComplexVector 'divisionVectorPorEscalar' para poder dividir cada numero
del vector por su norma<br/>
* sacamos la accion de omega sobre phi<br/>
* sacamos el producto interno de vectores entre la accion y phi y mostramos el valor real que es valor esperado<br/>

* creamos la matriz identidad<br/>
* multiplicamos el valor esperado por la identidad en este caso mutiplicamos el valor esperado por -1 ya que lo necesitamos sumar en el siguiente paso<br/>
* sumamos la matriz omega por la matriz del paso anterior esta es la definicion de delta<br/>
* sacamos delta cuadrada<br/>
* mutiplicamos delta cuadrada con phi<br/>
* y por ultimo hacemos producto interno de matrices entre el resultado anterior y phi<br/>

## Prerrequisitos

### Numeros Complejos
* Sumar
* Restar
* Multiplicar
* Dividir
* Modulo
* Conjugado
* Representacion polar
* Representacion cartesiana
* Fase
* Vectores Complejos
* Producto por escalar
* Inversa
* Sumar vectores

### Matrices Complejas
* Sumar matrices
* Inversa
* Producto
* producto Tensor

# Descarga e instalación

Para descargar este proyecto debera tener descagado git en su maquina y posteriormente copiar el siguiente comando en un shell del sistema operativo
```
git clone https://github.com/Edyesid/Sistema-cuantico-de-particula-en-una-linea.git
```
Pare compilar y ejecutar el programa debera tener instalado [maven](https://maven.apache.org/install.html) en su maquina y luego ejecuta los siguientes comando

1. compilar

```
mvn package
```

2. Ejecutar

```
mvn exec:java -Dexec.mainClass="edu.escuelaing.cnyt.app.Calculator"
```

# Construido
[Eclipse](https://www.eclipse.org/ide/) Editor de Java donde se puede compilar el proyecto

# Autor
Edwin Yesid Rodriguez Maldonado

# Licencia
Este programa es de uso libre
