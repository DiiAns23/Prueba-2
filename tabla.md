**Table of Contents**

## Indice

- [Diagrama de Clases](#Diagrama de Clases)


Diccionario de Clases 
-----------------------
Clase |  Definición 
------------ | -------------
DB | Inicializa y contiene todas las funciones con respecto a crear, editar, leer y eliminar de las bases de datos, tablas y registros.
NodoB | Inicializa y contiene la estructura de los nodos que se conforman el arbol B.
ArbolB | Contiene todas la funciones que le rellenan y dan la forma al arbol B, instanciando nodos.
PP | Contiene todas las funciones de la interfaz gráfica.

Diccionario de Funciones 
-----------------------

### Funciones CRUD de las bases de datos ###

Función |  Definición 
------------ | -------------
alterDatabase | Renombra la base de datos seleccionada.
createDatabase | Crea una base de datos.
dropDatabase | Elimina por completo la base de datos seleccionada.
showDatabase | Devuelve una lista de los nombres de las bases de datos.

### Funciones CRUD de las tablas ###

Función |  Definición 
------------ | -------------
alterAddColumn | Agrega una columna al final de cada registro de la tabla y base de datos especificada.
alterAddPK | Asocia a la tabla una llave primaria simple o compuesta mediante la lista de número de columnas.
alterDropColumn | Eliminar una n-ésima columna de cada registro de la tabla excepto si son llaves primarias.
alterDropPK | Elimina la llave primaria actual en la información de la tabla, manteniendo el índice actual de la estructura.
alterTable | Renombra el nombre de la tabla de una base de datos especificada.
createTable | Crea una tabla en una base de datos especificada recibiendo una lista de índices referentes a la llave primaria.
dropTable | Elimina por completo una tabla de una base de datos especificada.
extractRangeTable | Extrae y devuelve una lista con los elementos que corresponden a un rango de registros de la tabla. 
extractTable | Extrae y devuelve una lista con elementos que corresponden a cada registro de la tabla.
showTables | Devuelve una lista de los nombres de las tablas almacenadas en una base de datos.

### Funciones CRUD de los registros ###

Función |  Definición 
------------ | -------------
delete | Elimina un registro de una tabla y base de datos especificados por la llave primaria.
extrectRow | Extrae y devuelve un registro especificado por su llave primaria.
insert | Inserta un registro en la estructura de datos asociada a la tabla y la base de datos.
loadCSV | Carga un archivo CSV de una ruta especificada indicando la base de datos y tabla donde será almacenado.
truncate | Elimina todos los registros de una tabla y base de datos.
update | Inserta un registro en la estructura de datos asociada a la tabla y la base de datos.

### Funciones de utilidad ###

Función |  Definición 
------------ | -------------
identify | Valida que los nombres de bases de datos y tablas sean identificadores de SQL.
searchDB | Verifica si una base de datos especifica ya se encuentra almacenada.
searchTB | Verifica si una tabla de una base de datos ya se encuentra almacenada.
searchRepeat | Verifica si en el arreglo indicado existen datos repetidos.
updateTree |  Actualiza el arbol B de datos cuando se realizan cambios.
verifyPk | Crea y verifica si las llaves primarias estan repetidas.

### Funciones de serializacion ###

Función |  Definición 
------------ | -------------
commit | Genera el archivo binario.
initCheck | Verifica si esta creada la carpeta que almacena archivos binarios.
rollback | Decodifica el archivo binario.

### Funciones del nodo ###

Función |  Definición 
------------ | -------------
buscar_llave | Verifica la existencia de una llave dentro de un nodo.
comparar | Compara las llaves dentro de los nodos.
insertar | Guarda la tupla dentro del nodo.
ordenar_llave | Ordena las llaves dentro del nodo, ascendentemente.
posicionNodo | Obtiene la posicion del nodo dentro del arbol
toASCII | Obtiene la sumatoria del codigo asi de los caracteres de una cadena.

### Funciones del arbol B ###

Función |  Definición 
------------ | -------------
agregarValor | Agrega un dato en la ultima posicion de cada registro.
buscar | Encuentra y devuelve el nodo al que pertenece una llave.
del | Elimina un registro de la estructura.
eliminarValor | Eliminar un dato en especifico de cada registro.
estructurar | Ordena el arbol luego de una inserción.
graficar | Genera el archivo del arbol en forma visual.
insertar | Ingresa una llave en el nodo correcto.
Keys | Obtiene todas las llaves primarias de los registros almacenados.
posicion | Obtiene la posición de la llave a eliminar.
registros | Obtiene todos los registros almacenados en cada nodo del arbol B.
rotar | Determina la posición en la que se insertará una llave.
separar_nodo | Rompe una página del árbol.
unir | Une dos páginas separadas y forma una sola.
valor_buscar | Obtiene la posición de un valor dado en los nodos.


