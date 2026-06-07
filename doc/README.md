# Manual del Gestor
Bienvenido al manual de usuario del gestor de prestamos de MZ.Banks desarrollado para Michael Jackson Gamboa. Este programa permite gestionar usuarios, ítems, préstamos, devoluciones y generación automática de certificados y facturas.

## Usuario
### Ingreso al gestor
 Inicialmente encontraran la siguiente pantalla con el **Menú principal**
 
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
    

Seleccionara el número de la acción que desee realizar 

### Función de cada opción
#### Registrar usuario
Permite ingresar un usuario nuevo al gestor con los siguientes datos:
- Nombre, solo se permiten letras y se necesitan mínimo 3 caracteres
- Apellido, solo se permiten letras y se necesitan mínimo 3 caracteres
- Número de Cédula, solo se permiten números y se necesitan mínimo 3 y máximo 15 dígitos
- Correo electronico, este debe contener un @ y terminar en .com
- Tiempo de prestamo, debe escoger entre las opciones de tiempo dadas: 5, 10, 15 o 30 días
  
En caso de que alguno de los datos no cumpla con las restricciones mencionadas el gestor arrojara error, de cumplir con todo lo solicitado el programa muestra un mesaje de registro exitospo y la oportunidad de registrar otro usuario nuevo o devolcerse al menu de inicio.

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
 En caso, de ingresar mal el ID del ítem prestado o el de un ítem no prestado el gestor no permitira la continuidad del registro
- Se informa de la cantidad de días que el usuario a estado con el ítam
  En caso de que se encuentre dentro de los días estipulados de devolución se sigue con el proceso normal.
  En el caso contrario, se genera un venta forzada del ítem y genera un factura con la siguiente información: Motivo de la venta forzosa, número de la transacción, el ID del ítem, una descripcion del ítem, la cédula del comprador, subtotal, precio base más un impuesto de 23%.
- Se introduce en una valoracion del 1.0 a 10.0 acerca del estado del ítem

Si el proceso es correcto, el gestor entrega un mensaje informando que el registro fue un exito y genera un certifcado nombrado con el nombre completo del usuario, la fecha actual y el ID del ítem.

#### Consultar ítems con más de 30 días
Para consultar si existen ítems con más de 30 días, se realiza el siguiente proceso:
- Se ingresa el documento del usuario
- El gestor informa si existen prestamos registrados por el usuario con más de 30 dias
  En caso de que sí
  - Muestra un reporte detallado del retraso, inicialmente indica la cantidad de prestamos con retraso, luego muestra cada prestamo a detalle, indica que número transacción es, el ID del ítem, una descripcion, el nombre y la cédula del prestamista y la cantidad de días de retraso que tiene el ítem.
  En caso de que no:
  - El programa informa al usuario que no existen prestamos con retraso

#### Consultar artículos prestados
Muestra un documento con la lista de los ítems prestados, muestra cada prestamo a detalle, indica que número ítem es, el tiempo que el ítem lleva préstado, el ID del ítem y una descripcion, y el nombre del prestamista.

#### Administador
Permite al administrador ingresar al gestor con los siguientes datos:
- Usuario del administrador
- Constraseña del usuario
  
Si el ingreso es correcto, muestra al administrador el menú de administradores:
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

Se selecciona el número de la opción a realizar
### Función de cada opción
#### Total de préstamos registrados
Muestra un reporte detallado de los prestamos, inicialmente indica la cantidad de prestamos registrados, luego muestra cada prestamo a detalle, indica que número transacción es, el ID del ítem, una descripcion, la cédula del prestamista y la fecha en que fue realizado el prestamo.
#### Total de ítem devueltos
Muestra un reporte detallado de las devoluciones, inicialmente indica la cantidad de prestamos devueltos, luego muestra cada devolución a detalle, indica que número devolución es, el ID del ítem, una descripcion, la cédula del prestamista y el estado del ítem devuelto.
#### Total de ventas realizadas
Muestra un reporte detallado del total de ventas, inicialmente indica la cantidad de ventas forzadas, luego muestra cada devolución a detalle de venta, indica que número de venta que es, el ID del ítem, la cédula del prestamista, la fecha en que fue realizada la venta y el total pagado.
#### Total pago realizado
Muestra un reporte detallado del total de ingresos a la caja, inicialmente indica la cantidad de ventas forzadas, en un caja va sumando los ingresos de dichas ventas.
#### Lista de Usuarios
Muestra un reporte detallado de los usuarios, inicialmente indica la cantidad de usuarios registrados, luego muestra los datos que fueron solicitados en el registro de cada usuario.
#### Usuario con mayor y menor cantidad de préstamos
Muestra un reporte detallado del récord de préstamso activos, el programa indica dos datos el usuario con más prestamos registrados y el que menos tiene, muestra el número de prestamos, el nombre y cédula del usuario. En caso de que todos los usuarios tengan la misma cantidad de prestamos el progrma muestra la lista de todos los usuarios con la cantidad de prestamos, nombre y cédula. En caso de que no hayan prestamos registrados arroja un mensaje informando que no hay prestamos registrados activos en el sistema.

#### Para salir del menú de administradores se selecciona la opción 7 de salir y el programa devuelve al menú principal.

### Para salir del programa se selecciona la opcion 7 del menú prinicpal.

