# Escuela Colombiana de ingenieria
# Ciencias naturales y tecnologia                 23/10/2019
#Sistema cuantico de particula en una linea

mvn exec:java -Dexec.mainClass="edu.escuelaing.cnyt.app.Calculator"

mvn package

Calculadora cuantica<br/>
En este proyecto contiene los nuevos metodos de particula en una recta y calculadora estadistica para observables<br/>
estos se encuentra en la clase calculator en la linea 235 y 258 respectivamente<br/>

particula en una recta:<br/>
para este metodo se uso la siguiente  formula:<br/>
![imagen](https://i.ibb.co/mzMg4mv/Captura.png) <br/>

Para desarrollar esta formula se saco primero la norma del vector al cuadrado, luego se cada numero del mismo vector se le saco
el modulo al cuadrado y se dividio por la norma del vector al cuadrado, todos los resultados se almacenan en una lista para enviarla
al metodo que construlle el diagrama de barras<br/>
<br/>
calculadora estadistica para observables:<br/>
Para desarrollar esta funcion se hizo uso de las siguientes formulas:<br/>
<br/>
![imagen](https://i.ibb.co/VT4xq5h/Captura2.png) <br/>
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

# Prerrequisitos
Numeros Complejos<br/>
Sumar<br/>
Restar<br/>
Multiplicar<br/>
Dividir<br/>
Modulo<br/>
Conjugado<br/>
Representacion polar <br/>
Representacion cartesiana<br/>
Fase<br/>
Vectores Complejos<br/>
Producto por escalar<br/>
Inversa<br/>
Sumar vectores<br/>

Matrices Complejas<br/>
Sumar matrices<br/>
Inversa<br/>
Producto<br/>
producto Tensor<br/>

# Instalacion
Si quiere probar como funciona el programa tiene que seguir estos pasos<br/>
1. descargue el rar del git<br/>
2. Descargar Eclipse<br/>
3. Abra el proyecto en eclipse y de click derecho en la carpeta calculadora luego busca la opcion 'build path' , 'configure build path' y luego busca la parte de libreries y elimina las librerias de jcommon y jfreechart<br/>
![imagen](https://i.ibb.co/TqkdXmj/built.png)
4. vuelve a insertar las librerias en la opcion add external jars.. y agrega las dos librerias que estan incluidas en rar descargado<br/> 
![imagen2](https://i.ibb.co/Mc2rYKG/built2.png)
5. ingrese los parametros deseados en cada uno de los metodos del programa y corre el programa<br/>

# Construido
Eclipse Editor de Java donde se puede compilar el proyecto<br/>

# Autor
Edwin Yesid Rodriguez Maldonado<br/>

# Licencia
Este programa es de uso libre
