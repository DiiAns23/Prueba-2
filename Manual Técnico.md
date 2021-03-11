
## Indice

#### • [Descripción de la solución](#descipcion-de-la-solucion) ####

#### • [Requerimientos Funcionales del Sistema](#requerimientos-funcionales-del-sistema) ####

#### • [Requerimientos del Entorno de Desarrollo](#requerimientos-del-entorno-de-desarrollo) ####

#### • [Diccionario de Clases](#diccionario-de-clases) ####

#### • [Diccionario de Funciones](#diccionario-de-funciones) ####


Descripción de la solución 
-----------------------

#### Ejecucion ####

Para ejecutar los archivos _Léxico_ y _Sintáctico_ se utilizó el archivo _*Compilar.bat*_ el cual es un tipo de puente entre los archivos ya antes mencionados y a su vez la creación de los archivos Léxico.java y Sintáctico.java.

#### Lectura ####

Para una lectura rapida del archivo de entrada se utilizaron las herramientas JLex y Cup, creando gramaticas en la misma. Los archivos utilizados para este proceso son Lexico, Sintáctico, Léxico.java y Sintáctico.java.

#### Analizador ####

El programa lee caracter por caracter el archivo de entrada, el cual deberá de tener una extensión de tipo _olc_ , si un caracter no cumple con la estructura definida en el programa se creará un archivo de Reporte de Errores de tipo pdf.

Requerimientos Funcionales del Sistema
-----------------------
• Existe un paquete el cual es el encargado de gestionar el almacenamiento de las bases de datos, proporcionando al servidor un conjunto de funciones para ingresar, modificar extraer y eliminar la información.

• Cada registro que corresponde a una tupla de una tabla será almacenado en cada nodo que corresponden a un Arbol B. Estos registros seran débilmente tipados.

• Se proporcionan funciones relacionadas al CRUD de bases de datos, tablas y registros.

• El paquete cuenta con una interfaz gráfica que facilita el manejo de la información, para ello se requiere tener instalado [graphviz](https://graphviz.org/download/)


Requerimientos del Entorno de Desarrollo
-----------------------
• Versión de Java: Java 8.0.0 o superior

• IDE utilizada: NetBeans IDE 8.2

• Espacio en memoria: 20 MB como mínimo

• Versión de Graphviz:  graphviz version 2.46.1 (20210213.1702)

• Liberia JLex y Cup

Diccionario de Clases 
-----------------------
Clase |  Definición 
------------ | -------------
`Arbol` | Genera todas las estructuras del programa como el Arbol de Expresiones Regulares, Tabla Siguiente, Tabla Transiciones, AFD y AFND.
`AFND` | Clase en la cual estan los datos necesarios para realizar el Automata Finito No Determinista.
`Estado` | Contiene los datos de los estados creados para el Automata Finito Determinista.
`Expresion_Regular` | Realiza la lectura caracter por caracter de la expresion ingresada.
`Generar_AFD, Generar_AFND, Generar_Arbol, Tabla_Follow y Tabla_Transicion` | Su funcionalidad es extraer los datos de la clase _Arbol_ para realizar los grafos correspondientes con la herramienta _GraphViz_
`Interfaz1` | Clase de tipo visual para el usuario que puede mandar a llamar a las claes ya antes mencionadas. Interfaz Grafica.

Diccionario de Funciones
-----------------------

### Funciones Principales ###

Función |  Definición 
------------ | -------------
`Arbol` | Manda a llamar a los distintos metodos para realizar todas las funciones del programa
`Agregar` | Genera los nodos para la realización del arbol de expresiones.
`Follow` | Genera la lista de siguientes las cuales se contienen en el arbol de expresiones.
`Estados` | Genera los estados para realizar el grafo del AFD.
`Crear_AFND` | Genera los estados para realizar el grafo del AFND.

### Funciones Secundarias  ###

Función |  Definición 
------------ | -------------
`Recorrer_Arbol` | Realiza la escritura del archivo para generar el archivo dot.
`recorrer` | Realiza la adicion de Siguientes 
`Separacion` | Recorre caracter por caracter la expresion ingresada en el archivo. 

### Funciones para Grafos ###
`CMD` | Funcion utilizada en distintas clases para la generacion de los grafos.


### Requerimientos
* Tener instalado [java](https://www.oracle.com/technetwork/es/java/javase/downloads/jdk-netbeans-jsp-3413139-esa.html).

* Si el archivo _Compilar.bat_ no se puede ejecutar desde NetBeans se puede ejecutar desde consola. 

* El archivo de entrada debe de ser con extensión _.olc_

```
Universidad San Carlos de Guatelama 2021
Programador: Diego Andrés Obín Rosales
Carné: 201903865
```

