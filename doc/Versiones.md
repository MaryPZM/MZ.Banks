## Historial de versiones

### v 0.1.0 
- Inicio de la creación del codigo en clase.
- Implementación del esqueleto del menú principal usando match case
- Funciones base para validar el registro de usuario:
  - Validación de longitud del nombre, mínimo 3 caracteres.
  - Validación de solo letras en nombre y apellido.
  - Validación de documento, solo números, entre 3 y 15 dígitos.

### v 0.2.0
- Se agregaron dos validaciones clave dentro del case 1 del menú principal:
- Validación de correo electrónico:
  - Debe contener @ y terminar en .com
- Validación de tiempo de préstamo:
 - Solo se permiten los valores 5, 10, 15 o 30 días
- Se implementó un diccionario para almacenar usuarios registrados, usando el número de cédula como clave
- Corrección de errores menores en validaciones previas

### v 0.3.0 
- Se inició el desarrollo del match case 2, Registrar Préstamo
- Se identificó que primero se necesitaba registrar ítems antes de prestarlos
- Se creó la función para registrar ítems con:
  - Nombre, categoría, precio, estado del ítem
  - Generación automática de ID único
- Se comenzó a estructurar el case 3, Registro de Devoluciones
- Se plantearon diccionarios separados para:
  - Ítems en inventario
  - Ítems prestados activamente
- Base conceptual para futuras validaciones

### v 0.4.0 
- Al intentar desarrollar el match case 4, consultar ítems con más de 30 días, se detectó un error crítico:
  - La función de préstamo no estaba guardando la fecha exacta del préstamo
- Se corrigió la función del match case 2 para almacenar la fecha actual automáticamente al prestar un ítem
- Esto permitió calcular correctamente los días transcurridos
- Se completó la lógica base del match case 2:
  - Solo permite préstamos si el usuario está registrado y el ítem existe

### v 0.5.0 
- Se corrigió nuevamente el match case 2 después de consultar el flujo real:
  - Si no hay ítems registrados, se muestra un mensaje y se impide el préstamo
  - Si hay ítems disponibles, se listan y se puede seleccionar uno
- Además, el usuario puede registrar un ítem nuevo directamente desde el menú de préstamo si lo desea
- Se desarrolló el match case 5, consultar artículos prestados, basado en el diccionario de ítems prestados, mostrando los resultados ordenados por días.

### v 0.6.0 
- Se inició el desarrollo del match case 6 (Administrador)
- Se identificó la necesidad de nuevos diccionarios:
  - Devoluciones realizadas
  - Préstamos completados, historial
  - Administradores predeterminados, usuario y contraseña fijos
- Se creó el submenú de administrador con estructura similar al menú principal usando match case
- Se implementaron las funciones para cada reporte del submenú:
  - Total préstamos registrados
  - Total ítems devueltos
  - Total ventas realizadas
  - Total pagado acumulado
  - Lista de usuarios
  - Usuario con mayor y menor cantidad de préstamos
### v 1.0.0
- El codigo ya tenia estructura para gestionar y guardar los prestamos
### v 1.1.0
- Mejoras en consultas
- Archivos planos
- Certificados y facturas
### v 1.2.0	
- Codigo finalizado.

MZ.Banks(v1.2.0)
