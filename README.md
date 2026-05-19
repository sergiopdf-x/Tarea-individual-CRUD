## EXPLICACION DEL SISTEMA
Este proyecto nos permite registrar y administrar personas pertenecientes a una institución
educativa mediante las operaciones del CRUD (Crear, Leer, Actualizar, Eliminar)
## HERENCIA
- Al programa se implemento una clase Padre denominada *Persona*, el cual
  va a contener los atributos protegidos, se declararon los atributos como:
  1. Cedula
  2. Nombre completo
  3. Edad
- Y a partir de esta clase Padre se crearon las dos subclases o clases hijas
  # *Estudiante* #
  •	Va a heredar los atributos de la clase Persona con el "extends" y
    se agregara un atributo privado denominado carrera.
  # *Docente* #
  • Tambien va a heredar los atributos de la clase Persona con el "extends" y
    se va a agregar el atributo privado denominado asignatura.
- De esta manera se logra evitar repetir el codigo y se aprovecha reutilizar mediante la herencia
## ENCAPSULAMIENTO
- Los atributos se declararon como *private* y *protected* para lograr la proteger los datos
  internos de cada una de las clases
- Se utilizaron metodos *get* y *set* para poder acceder y modificar los datos de manera controlada
## SOBREESCRITURA
- Las dos clases hijas *Estudiante* y *Docente* van a soobreescribir un metodo que se declaro en la clase Padre
  como mostrarDatos() para esto utilizamos @Override
  # *EJEMPLO* #
  - Un estudiante muestra su carrera
  - Un maestro muestra la asignatura que imparte
## USO DE ARRAYS
- Se utilizo principalmente la linea *ArraysList<Persona> personas = new ArrayList<>();*
- ArraysList: Va a permitir almacenar dinamicamente los objetos de tipo Persona, tanto estudiantes como docentes

  # Porque se eligió ArrayList #
  - Se eligio porque nos va a permitir:
    1. Agregar registros utilizando add()
    2. Obtener registros a traves del get()
    3. Actualizar la informacion
    4. Eliminar registros utilizando remove()
## MEMU INTERACTIVO
- Este proyecto funciona mediante un menu repetitivo implementando con *do-while* y *switch*
- Se implemento tambien el Scanner para que el usuario seleccione una opcion y el sistema va a ejecutar
  la acción correspondiente *(Crear,Mostrar,Actualizar,Eliminar)*
- El menu va a ejecutarse o a mantenerse activo hasta que el usuario seleccione la opcion salir
## MANEJO DE EXCEPCIONES
- En este programa se implemento *try* y *catch* para evitar que el programa finalice por errores de entrada
- Algunos de los datos controlados son:
   1. Ingreso de letras donde se esperan numeros
   2. Opciones invalidas del menu
   3. Posiciones inexistentes
   4. Campos vacios
- Esto nos va a ayudar a tener estabilidad en el sistema y que el usuario tenga una mejor experiencia
## VALIDACIONES ADICIONALES
- En el programa se agregaron algunas validaciones para:
  1. Edades invalidas
  2. Cedulas duplicadas
- Esto nos permite tener un mejor control sobre los datos que ingrese el usuario
## POLIMORFISMO
- El programa utilizo el polimosrfismo mediante el *ArrayList*
  ArrayList<Persona> personas
- Esto nos permitio almacenar los objetos de los diferentes tipos *Estudiante* y *Docente* dentro de una
  misma colección
