# Tarea-2-Vicente-
Tarea 2 Vicente 
Sistema de busqueda de canciones


Descripción
Este sistema permite a los usuarios cargar una base de datos de canciones y buscarlas rápidamente por cualquiera de los siguientes criterios :
- Género
- Artista
- Tempo


Cómo compilar y ejecutar

Este sistema ha sido desarrollado en lenguaje C y puede ejecutarse fácilmente utilizando Replit.
Para comenzar a trabajar con el sistema en tu equipo local, sigue estos pasos:

Pasos para compilar y ejecutar:
1. Descarga el archivo `.zip` en una carpeta de tu elección.
2. Abre el proyecto en Replit 
    - Entrar a https://replit.com/~.
    - Iniciar Sesión
    - Selecciona `+ > Import an existing proyect > Zip file` y elige la carpeta donde se encuentra el proyecto.
    - Carga el archivo y selecciona `View app ´
3. Compila el código
    - Abrir la librería desde arriba a la derecha (Ctrl + Shift + L en su defecto)  
    - Seleccionar 'Files' 
    - Arrastrar el archivo .csv hasta la carpeta 'data' 
    - Abre el archivo principal (`tarea2.c`). 
    - Selecciona `+ > Shell ´ para abrir la terminal  integrada 
    - En la terminal, compila el programa con el siguiente comando (ajusta el nombre si el archivo principal tiene otro nombre): 

			gcc tdas/*.c tarea2.c -Wno-unused-result -o tarea2

    - Luego ejecuta la aplicación con:

			./tarea2

Funcionalidades :


Funcionando correctamente:
-Cargar archivo de canciones
-Buscar canciones por género
-Buscar canciones por artista 
-Buscar canciones por tempo

Problemas conocidos:
-En caso de no encontrar un artista o género no se diferencia entre inexistencia del buscado o falta de carga del archivo
-Funciona solo para columnas estandarizadas del archivo
-La búsqueda por artista solo funciona al escribir el nombre con mayúsculas al incio

A mejorar :

Eficiencia al momento de cargar el archivo csv
Especificación de errores (problema #1)
Globalización de registros de canciones (problema #2)
Hacer que la búsqueda por artista no discrimine entre mayusc. y minusc. 

Ejemplo de uso

Paso 1: añadir el csv a los archivos accesibles

-Se comienza añadiendo el archivo a la carpeta data (canciones.csv para este ejemplo).

Paso 2: cargar el csv
```
Opción seleccionada: 1) Cargar Canciones
```
-Buscar el archivo .csv en la carpeta data
-Apretar click derecho
-Seleccionar "Copy file path"
-Apretar click derecho en la consola y seleccionar "paste"
-Apretar Enter

El programa carga todas las canciones y está listo para realizar las siguientes funciones

Paso 3: Buscar canciones según el criterio seleccionado

Paso3.1: Buscar por género
```
Opción seleccionada: 2) Buscar por género
Ingrese el género buscado : spanish
```
El sistema procede a mostrar los datos de todas las canciones del genero 'spanish' (a excepción del género, ya que sería redundante).

Paso 3.2: Buscar por artista
```
Opción seleccionada: 3) Buscar por artista
Ingrese el artista buscado : Shakira
```
La lista muestra todas las canciones en las que participó el/la artista seleccionad@.

Paso 3.3: Buscar por tempo

Basándose en su velocidad (Lentas, Moderadas, Rápidas) el sistema muestra todas las canciones del grupo correspondiente.

```
Opción seleccionada: 3) Buscar por tempo
Seleccione una categoría : 2) Moderadas
```
El sistema procederá a mostrar todas las canciones con un tempo mayor a 80 y menor a 120 BPM

