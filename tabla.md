Funciones CRUD de las bases de datos
-------------------------
Función |  Definición 
------------ | -------------
alterDatabase | Renombra la base de datos seleccionada.
createDatabase | Crea una base de datos.
dropDatabase | Elimina por completo la base de datos seleccionada.
showDatabase | Devuelve una lista de los nombres de las bases de datos.

Funciones CRUD de las tablas
-------------------------
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
