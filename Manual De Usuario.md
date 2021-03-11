 MANUAL DE USUARIO
===================
## Índice
- [Introduccion](#introduccion)
- [Descripción General del Sistema](#descrip)
- [Aplicacion](#apli)
- [Glosario](#glosario)
- [FAQ](#questions)

<div id='introduccion'/>

## Introducción
El programa cuenta con la implementación de una interfaz gráfica para el usuario, en la cual la interacción es amigable y compresible. Fue diseñada de forma simple para que consuma un menor gasto de recursos de su ordenador el cual se dara una mejor fluidez durante la ejecución. Este programa es de tipo _Analizador Léxico-Sintáctico_ que permite la validación de cadenas por medio de un archivo de entrada de tipo .olc.

<div id='descrip'/>

## Descripción

  - **Estructura de Almacenamiento**: 
Para cada lectura de un archivo de entrada se utilizaron listas ArrayList así como LinkedList para la implementacion correcta de las gramáticas ingresadas.

  - **Palabras Reservadas**:
El programa cuenta con palabras reservadas como: _CONJ_ la cual indica el inicio de un nuevo conjunto de caracteres, la cual debe de seguir una estructura de tipo Preorden. _%%_ indica la finalización de las expresiones regulares y procederá a realizar las validaciones de cadenas.
  
  - **Caracteres**:
El programa permite la lectura de cualquier caracter en cualquier posicion del archivo de entrada.


<div id='apli'/>

## Aplicación
### Interfaz Gráfica (GUI)
El programa cuenta con una vista gráfica la cual facilita la interacción entre el sistema y el usuario final para un mejor desempeño del mismo. Por medio de dicha interfaz, al usuario se le permite seleccionar de forma _gráfica_ una archivo de entrada que contendrá las gramáticas a analizar. El usuario puede navegar por la aplicación seleccionando a través de botones la acción que desea realizar, si ocurre un error en el ingreso de datos el programa creara un archivo en donde se mostrará al usuario el tipo de error que se está cometiendo y el lugar exacto del mismo. 

- Ventana Inicial: La _Ventana Inicial_ cuenta con las opciones: *_Archivo_*, *_Generar Gramaticas_* y *_Ver Imágenes_*.

![](https://github.com/DiiAns23/Prueba-2/blob/Master/img/InterfazGraficaOLC1.PNG)

   | **Opción** | **Funcionalidad** |
   | ---------- | ----------------- |
   | Archivo   |Para esta funcion se desplegará un submenú en el cual el usuario debe de seleccionar _Abrir_  y se le mostraá una pestaña para seleccionar el archivo de entrada|
   | Generar Gramaticas  | Generará todos los archivos correspondientes al archivo de entrada |
   | Ver Imágenes  | Mostrará las opciones disponibles luego de generar las gramáticas |
   |Siguiente| Mostrará la imagen siguiente correspondiente a la opción seleccionada en _Ver Imágenes_ |
   |Anterior| Mostrará la imagen anterior correspondiente a la opción seleccionada en _Ver Imágenes_ |
     

<div id='glosario'/>

## Glosario

| Palabra | Descripción | 
| ------------------------------- | ----------------------------------------- |
| Gramática | Reglas de un lenguaje |
| Interfaz Gráfica | Interacción entre el usuario y el sistema |
| Archivo de Entrada | Documento de extensión olc para el programa |
| CONJ | Palabra reservada que significa Conjunto |
| Preorden | Entrada que se lee RAIZ-IZQUIERDA-DERECHA |

<div id='questions'/> 

## Preguntas Frecuentes (FAQ)
**1. ¿Se puede cargar un archivo que sea otro tipo de extensión?** 

> _R//_ *No, el programa admite solo extensiones olc*

**2. ¿Puedo correr el .jar desde otro dispositivo?** 

> _R//_ *Para MacOs los .jar no estan disponibles*

**3. ¿Cuantas gramáticas puedo ingresar?** 

> _R//_ *El programa no tiene un límite para el ingreso de gramáticas*

**4.¿En donde se almacenan los archivos ingresados?** 

> _R//_ *Se almacenan en la misma carpeta en la que se encuentre el programa.*

**5. ¿Por qué no me genera ningún archivo?** 

> _R//_ *Suele suceder porque el archivo no cuenta con la estructura correspondiente.*
