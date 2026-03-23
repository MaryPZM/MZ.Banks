# MZ.Banks
# Descripción: 
En este repositorio se presenta el uso de herramientas que nos facilitaran la organizacion conceptual, que forma parte de la creacion de un programa de consola visualmente amigable al usuario, en donde permita gestionar el
préstamo de artículos, gestionando mediante archivos planos la información, para posteriormente
exportar los resultados a un CSV usando Python.
 
# *Integrantes:* 
## *Mary Paz Zuluaga Muñoz* 
estudiante del tercer semestre del programa de Ingenieria Industrial de la unversidad de Antioquia, la cual sera de gran ayuda para este proyecto ya que cuanta con fortalezas como la resposabilidad, liderazgo y la disciplina, las cuales aportara adecuadamente.
## *María Carolina Chaparro Ruiz* 
estudiante del tercer semestre del programa de Ingenieria Industrial de la unversidad de Antioquia, la cual sera de gran ayuda para este proyecto ya que cuanta con fortalezas como la resposabilidad, cratividad, trabajo en equipo y compromiso, las cuales ayudaran a equilibrar la colaboracion en equipo.

<a href="https://github.com/MaryPZM/MZ.Banks">MZ.Banks</a> © 2026 by <a href="https://github.com/MaryPZM">Mary Paz Zuluaga Muñoz</a> is licensed under <a href="https://creativecommons.org/licenses/by-nc-nd/4.0/">CC BY-NC-ND 4.0</a><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nd.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;">

# *Visión*
MZ.Banks es un software orientado a la gestión de operaciones bancarias y financieras, diseñado para simular o administrar procesos típicos de una entidad bancaria de manera estructurada y digital.
Este sistema permitrá organizar y controlar información relacionada con cuentas, usuarios y transacciones, facilitando la administración de recursos económicos dentro de un entorno seguro y eficiente.
Se planea realizar con exito el programa de tal manera que facilite la organización de registros en un ámbito empresarial; mientras tanto, tambien se desea adquirir el conocimiento brindado acerca del uso y aplicación de herramientas que nos facilitaran futuros procesos y
poder entender los diferentes usos de las herramientas que utilizaremos durante este proceso.


# Especificación de requisitos
## Requisitos funcionales
### Registro de usuarios
Nombre (mínimo 3 letras, sin números),
apellido (mínimo 3 letras, sin números),
documento (entre 3 y 15 dígitos, solo números),
correo electrónico (debe contener “@” y terminar en “.com”),
tiempo de préstamo (solo valores permitidos: 5, 10, 15 o 30 días);
validar todos los datos ingresados y
mostrar mensajes de error si los datos no cumplen las condiciones
### Registro de ítems
#### El sistema debe permitir 
registrar objetos a prestar con
nombre (mínimo 3 letras, puede contener números),
categoría (solo una de las siguientes):
videojuegos,
 libros,
 música y video,
 herramientas,
dinero,
 misceláneo y varios;
 precio de compra,
 ID único (alfanumérico, asociado a la categoría) y
 estado del ítem (usando lógica difusa)
### Registro de préstamos

 #### El sistema debe:

 Permitir préstamos solo a usuarios registrados,
permitir seleccionar ítems disponibles por ID,
validar que el usuario exista y
Registrar:
usuario,
 ítem,
 fecha de préstamo y
tiempo de préstamo.
Permitir devoluciones solo de préstamos activos y
validar si el usuario tiene préstamos activos

#### Si el usuario no existe:

 Mostrar mensaje de error,
solicitar registro previo,
 registro de devoluciones.



#### Si, sí tiene usuario debe :

Registrar devolución,
 Generar certificado en archivo de texto (o PDF opcional) con:
 Nombre del usuario,
Fecha de devolución,
ID del préstamo y
### Generación de ventas.

#### El sistema debe:

Detectar préstamos mayores a 30 días,
 convertirlos automáticamente en venta y
 generar factura con:
 motivo de venta,
 subtotal,
 impuesto del 23% y
total a pagar.

### Consulta de estado de préstamos

#### El sistema debe:

 Mostrar lista de ítems prestados,
 ordenarlos por cantidad de días,
usar estadísticas básicas y
 leer y almacenar datos en archivos planos.
### Módulo de administrador

#### El sistema debe: 

 Permitir acceso solo con usuario y contraseña válidos, 
validar contra una lista almacenada, mostrar reportes de: total de préstamos, total de devoluciones, total de ventas
total de dinero recaudado, lista de usuarios,
usuario con más préstamos y
usuario con menos préstamos.
## Requisitos no funcionales.

### Seguridad
Validación de acceso para administrador, protección de credenciales,
control de acceso a funciones sensibles,
rendimiento,
respuesta rápida en consultas y registros y
manejo eficiente de múltiples datos
### Usabilidad
Una interfaz clara tipo menú, 
mensajes de error comprensibles y
flujo lógico de navegación.
### Persistencia de datos
 Uso de archivos planos para almacenar información,
lectura y escritura correcta de datos y
conservación de datos entre ejecuciones.
### Integridad de datos
Validaciones estrictas en entradas,
evitar duplicados, 
consistencia en préstamos, devoluciones y ventas,
### Conservación 
Contará con un código organizado por módulos (usuarios, ítems, préstamos, etc.),
fácil de modificar o ampliar,
### Flexibilidad 
 Posibilidad de agregar nuevas categorías o funcionalidades y
soporte para mayor cantidad de usuarios e ítems
### Generación de archivos
La creación de archivos de texto para:
Certificados de devolución y
para facturas de venta

