# Taller 1 Estuctura de Datos
## Integrantes
**Emily Franchesca Volta Miranda; 20.718.229-k; emily.volta@alumnos.ucn.cl; Paralelo C2**

**Martín Ubilla Briceño; 20.751.624-4; martin.ubilla@alumnos.ucn.cl; Paralelo C2**
# Biblioteca

Esto es un sistema para una biblioteca en la que habrá diferentes funciones para gestionar dicha biblioteca. 

## Funciones
- Agregar materiales a la biblioteca (Libro o Revista)
- Mostrar información de los materiales
- Buscar material por autor o título
- Prestar y devolver material
- Gestión de usuarios (Agregar, eliminar, buscar)

## Modo de uso
1. Compilación `g++ -g -o programa .\Biblioteca.cpp .\Usuario.cpp .\MaterialBibliografico.cpp .\Libro.cpp .\Revista.cpp .\main.cpp`
2. Ejecutar programa.exe
3. Elegir opciones del menú
   
   (1) Agregar material
   
   (2) Buscar material en la Biblioteca

   (3) Mostrar información de los materiales
   
   (4) Agregar usuario
   
   (5) Eliminar usuario
   
   (6) Buscar Usuario
   
   (7) Prestar material
   
   (8) Devolver material
   
   (9) Salir

## Estructura

`main.h` = Header de la clase `main.cpp` 

`main.cpp` = Implementa el header `main.h` y clase en la que se ejecuta el programa

`Biblioteca.h` = Header de la clase `Biblioteca.cpp`

`Biblioteca.cpp` = Implementa el header `Biblioteca.h` y es la clase en la que se gestiona toda la biblioteca 

`Usuario.h` = Header de la clase `Usuario.cpp`

`Usuario.cpp` = Implementa el header `Usuario.h` en donde se representa y gestiona las funciones del usuario de la biblioteca

`MaterialBibliografico.h` = Header de la clase `MaterialBiblbiografico.cpp`

`MaterialBbibliografico.cpp` = Implementa el header `MaterialBibliografico.h` en donde se representa y gestiona las funciones de los materiales de la biblioteca

`Libro.h` = Header de la clase `Libro.cpp`

`Libro.cpp` = Implementa la clase `Libro.h` clase que hereda de `MaterialBibliografico`, simboliza un libro

`Revista.h` = Header de la clase `Revista.cpp`

`Revista.cpp` = Implementa la clase `Libro.h` clase que hereda de `MaterialBibliografico`, simboliza un libro

`Usuarios.txt` = Archivo en el que se lee y guarda informacion de los usuarios ingresados en el sistema de la biblioteca

`Materiales.txt` = Archivo en el que se lee y guarda informacion de los materiales ingresados en el sistema de la biblioteca

## Información de los objetos que se crean en el main
## Usuarios:
Los usuarios que se crearán al iniciar el programa serán:

- **ID:** `JPX-874-29Q7-45` - **Nombre:** Juan Pérez
- **ID:** `MLZ-129-7TQ3-88` - **Nombre:** María López
- **ID:** `CGY-563-9XN4-02` - **Nombre:** Carlos García

Estos se crearán al leer el archivo `Usuarios.txt` de la siguiente manera:

**Formato del archivo**:  
`ID;NOMBRE`
## Materiales Bibliográficos:

- **TIPO:** `L` - **Título:** `1984` - **Autor:** `George Orwell` - **ISBN:** `100-1` - **Fecha de Publicación:** `08/06/1949` - **Resumen:** `Una distopía sobre un futuro totalitario donde se controla el pensamiento` - **IdUsuario:** `S/U`
- **TIPO:** `L` - **Título:** `Sapiens: A Brief History of Humankind` - **Autor:** `Yuval Noah Harari` - **ISBN:** `978-0062316097` - **Fecha de Publicación:** `04/09/2014` - **Resumen:** `Historia de la humanidad desde sus inicios hasta la era moderna` - **IdUsuario:** `MLZ-129-7TQ3-88`
- **TIPO:** `R` - **Título:** `National Geographic (Edición especial sobre el cambio climático)` - **Autor:** `Varios autores` - **ISBN:** `978-1426217138` - **Número Edición:** `Edición N° 9` - **Mes Publicación:** `Octubre` - **IdUsuario:** `JPX-874-29Q7-45`

Estos se crearán al leer el archivo `Materiales.txt` de la siguiente manera:

**Formato del archivo**:  
`TIPO;TÍTULO;AUTOR;ISBN;ATRIBUTO 1 REVISTA O LIBRO;ATRIBUTO 2 REVISTA O LIBRO;IdUSUARIO`



