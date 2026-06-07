# Manual del Gestor
Bienvenido al manual de usuario del gestor de prestamos de MZ.Banks desarrollado para Michael Jackson Gamboa. Este programa permite gestionar usuarios, ítems, préstamos, devoluciones y generación automática de certificados y facturas.

## Usuario
### Ingreso al gestor
 Inicialmente encontraran la siguiente pantalla con el **Menu principal**
 
------------------------------------------------------------
                          MZ.Banks                          

                    ..::Bienvenidos::..                     
------------------------------------------------------------

    1. Registrar Usuario
    2. Registrar Prestamo
    3. Registrar devolucion
    4. Consultar items con mas de 30 dias
    5. Consultar articulo prestado
    6. Administrador 
    7. Salir
    
Favor registrar la opcion deseada-->

Seleccionara el número de la acción que desee realizar 

### Función de cada opción
#### Registrar usuario
Permite ingresar un usuario nuevo al gestor con los siguientes datos:
- Nombre, solo se permiten letras y se necesitan mínimo 3 caracteres
- Apellido, solo se permiten letras y se necesitan mínimo 3 caracteres
- Número de Cédula, solo se permiten números y se necesitan mínimo 3 y máximo 15 dígitos
- Correo electronico, este debe contener un @ y terminar en .com
- Tiempo de prestamo, debe escoger entre las opciones de tiempo dadas: 5, 10, 15 o 30 días
  
En caso de que alguno de los datos no cumpla con las restricciones mencionadas el gestor arrogara error, de cumplir con todo lo solicitado el programa muestra un mesaje de registro exito y la oportunidad de registrar otro usuario nuevo o devolcerse al menu de inicio.

#### Registrar préstamo
Permite, a un usuario ya registrado, ingresar el préstamo de ítem con el siguiente proceso:
- Se ingresa el número de cédula de un usuario ya registrado
- El progrma informa si hay ítems en el inventario, en caso de que no, pregunta al usuario si desea registrar uno
   Para registrar un ítem pide:
  - Nombre del item, este debe contener minimo 3 caracteres o digitos
  - Se selecciona la categoria a la pertenece el ítem entre las siguientes:
    1. Videojuegos
    2. Libros
    3. Musica y video
    4. Herramientas
    5. Dinero
    6. Miscelaneo y varios
  - Se introduce el precio del ítem
  - Se introduce en una valoracion del 1.0 a 10.0 acerca del estado del ítem
    Si todo fue ingresado de manera correcta el programa arroja un mensaje de ítem registrado con exito y el ID del ítem. Además, da la oportunidad de registrar un nuevo ítem, en el caso contrario devuelve al usuario al registro de prestamo
    
- Se ingresa el ID del ítem que se desea presar
  
En caso de que el ID del ítem no exita o el usuario no este registrado el programa rechazara el intento de registro de préstamo.

#### Registrar devolución
Permite, a un usuario ya registrado, ingresar la devolucioón de un préstamo con el siguiente proceso:
- Se ingresa el documento del usuario
- Se ingresa el ID del ítem a devolver
  En caso, de ngresar mal el ID del ítem prestado o el de un ítem no prestado el gestor no permitira la continuidad del registro
- Se informa de la cantidad de días que el usuario a estado con el ítam
  -  ,xkdmcdks 
- Se introduce en una valoracion del 1.0 a 10.0 acerca del estado del ítem

Si el proceso es correcto, el gestor entrega un mensaje informando que el registro fue un exito y genera un certifcado nombrado con el nombre completo del usuario, la fecha actual y el ID del ítem.

#### Consultar ítems con más de 30 días
Para consultar si existen ítems con más de 30 días, se realiza el siguiente proceso:
- Se ingresa el documento del usuario
- El gestor informa si existen prestamos registrados por el usuario con más de 30 dias
  En caso de que sí
  - jyuy7h8uji
  En caso de que no:
  - El programa informa al usuario que no existen prestamos con retraso

#### Consultar artículos prestados
Muestra...

#### Administador
Permite al administrador ingresar al gestor con los siguientes datos:
- Usuario del administrador
- Constraseña del usuario
Si el ingreso es correcto, muestra al administrador el menu de administradores:
------------------------------------------------------------
                          MZ.Banks                          

       ..::Bienvenidos al Menu de administradores::..       
------------------------------------------------------------

    1. Total de préstamos registrados
    2. Total de ítems devueltos
    3. Total de ventas realizadas
    4. Total pago realizado
    5. Lista de usuarios
    6. Usuario con mayor y menor cantidad de préstamos.
    7. Salir

##
