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
#### Nombre (mínimo 3 letras, sin números),
#### Apellido (mínimo 3 letras, sin números),
#### Documento (entre 3 y 15 dígitos, solo números),
#### Correo electrónico (debe contener “@” y terminar en “.com”),
#### Tiempo de préstamo (solo valores permitidos: 5, 10, 15 o 30 días); 
#### Validar todos los datos ingresados
Mostrar mensajes de error si los datos no cumplen las condiciones
### Registro de ítems
#### El sistema debe permitir registrar objetos a prestar con:
##### Nombre (mínimo 3 letras, puede contener números)
##### Categoría (solo una de las siguientes):
###### Videojuegos,
###### Libros,
###### Música y video,
###### Herramientas,
###### Dinero,
###### Misceláneo y varios,
##### Precio de compra,
##### ID único (alfanumérico, asociado a la categoría)
##### Estado del ítem (usando lógica difusa)
### Registro de préstamos

#### El sistema debe:

##### Permitir préstamos solo a usuarios registrados
##### Permitir seleccionar ítems disponibles por ID
##### Validar que el usuario exista
##### Registrar:
###### Usuario
###### Ítem
###### Fecha de préstamo
###### Tiempo de préstamo

#### Si el usuario no existe:

##### Mostrar mensaje de error
##### Solicitar registro previo
### Registro de devoluciones

#### El sistema debe:

##### Permitir devoluciones solo de préstamos activos
##### Validar si el usuario tiene préstamos activos

#### Si NO tiene:

##### Mostrar mensaje de error

#### Si SÍ tiene:

##### Registrar devolución
##### Generar certificado en archivo de texto (o PDF opcional) con:
##### Nombre del usuario
##### Fecha de devolución
##### ID del préstamo
### Generación de ventas

#### El sistema debe:

##### Detectar préstamos mayores a 30 días
##### Convertirlos automáticamente en venta
##### Generar factura con:
##### Motivo de venta
##### Subtotal
##### Impuesto del 23%
##### Total a pagar

### Consulta de estado de préstamos

#### El sistema debe:

##### Mostrar lista de ítems prestados
##### Ordenarlos por cantidad de días
##### Usar estadísticas básicas
##### Leer y almacenar datos en archivos planos
### Módulo de administrador

#### El sistema debe: 

##### Permitir acceso solo con usuario y contraseña válidos
##### Validar contra una lista almacenada

##### Debe mostrar reportes:

###### Total de préstamos
###### Total de devoluciones
###### Total de ventas
###### Total de dinero recaudado
###### Lista de usuarios
###### Usuario con más préstamos
###### Usuario con menos préstamos
## Requisitos no funcionales

### Seguridad
#### Validación de acceso para administrador
#### Protección de credenciales
#### Control de acceso a funciones sensibles
### Rendimiento
#### Respuesta rápida en consultas y registros
#### Manejo eficiente de múltiples datos
### Usabilidad
#### Interfaz clara tipo menú 
#### Mensajes de error comprensibles
#### Flujo lógico de navegación
### Persistencia de datos
#### Uso de archivos planos para almacenar información
#### Lectura y escritura correcta de datos
#### Conservación de datos entre ejecuciones
### Integridad de datos
#### Validaciones estrictas en entradas
#### Evitar duplicados 
#### Consistencia en préstamos, devoluciones y ventas
### Conservación 
#### Código organizado por módulos (usuarios, ítems, préstamos, etc.)
#### Fácil de modificar o ampliar
### Flexibilidad 
#### Posibilidad de agregar nuevas categorías o funcionalidades
#### Soporte para mayor cantidad de usuarios e ítems
### Generación de archivos
#### Creación de archivos de texto para:
#### Certificados de devolución
#### Facturas de venta

