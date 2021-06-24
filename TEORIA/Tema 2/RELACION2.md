**1.Clasifique los siguientes requisitos, según su tipo:**

1. Se llevará un control de todas los vehículos del establecimiento incluyendo su estado y disponibilidad**REQUISITO FUNCIONAL**

2. La aplicación funcionará sobre Windows10. **REQUISITO NO FUNCIONAL (implementacion)**

3. Sólo se levantará la barrera de entrada al aparcamiento tras haber reconocido la matrícula del vehículo situado ante la misma. **REQUISITO NO FUNCIONAL**

4. El producto debe llevar un registro de todas las carreteras que hayan sufrido daños. **REQUISITO FUNCIONAL **

5. El conductor debe de poder dar al sistema las ordenes siguientes: Activar, Desactivar, Comenzar Aceleración, Parar Aceleración, y Continuar. **REQUISITO FUNCIONAL**

6. El proceso de desarrollo deberá ajustarse al estándar PSS-05 de ESA.(Estándares de Ingeniería de Software de la European Space Agency) **REQUISITO NO FUNCIONAL(modelo del proceso)**

7. La aplicación estará disponible todos los días de la semana las 24 horas del día. **REQUISITO NO FUNCIONAL(FIABILIDAD)**

8. Cada tipo de fichero tendrá asociado un programa de acceso en la aplicación. **REQUISITO FUNCIONAL**

9. Los usuarios podrán buscar, descargar e imprimir los artículos del repositorio de la biblioteca. **REQUISITO FUNCIONAL**

10. A cada orden se le asignará un identificador único (ORDER-ID), que el usuario podrá copiar en el área de almacenamiento permanente de la cuenta. **REQUISITO FUNCIONAL**

11. La interfaz de usuario deberá implementarse haciendo uso de html simple, sin marcos ni applets JAVA. **REQUISITO NO FUNCIONAL(INTERFAZ)**

12. La aplicación deberá registrar los pagos de los recibos del impuesto del IBI. **REQUISITO DE INFORMACIÓN**

13. El sistema no podrá mostrar a los operadores la información personal del cliente, salvo su nombre y número de referencia. **REQUISITO FUNCIONAL / TAMBIÉN VALE NO FUNCIONAL **

14. Los usuarios deberán ser capaces de utilizar todas las funciones del programa tras recibir un curso de 3 horas de duración. **REQUISITO NO FUNCIONAL(FACILIDAD DE USO)**

15. La aplicación deberá poder reiniciarse y recuperar su funcionalidad al 100% antes de dos horas, tras producirse una caída por un fallo del tipo FA01. **REQUISITO NO FUNCIONAL (FIABILIDAD)**

**Un requisito funcional describe *lo* que debe hacer un sistema de software, mientras que los requisitos no funcionales imponen restricciones sobre *cómo* lo hará el sistema.EL DE INFORMACIÓN TE DICE CÓMO LO VA A GUARDAR EL SISTEMA. SI NO SABEMOS COMO VA/LO QUE HACE LA APLICACION, ES NO FUNCIONAL**



**7.Realice un análisis y descripción de implicados para una aplicación de gestión de una biblioteca.**

<u>Descripción general de los implicados de la biblioteca:</u>

| Nombre                | Descripción                                      | Tipo             | Responsabilidad                                              |
| --------------------- | ------------------------------------------------ | ---------------- | ------------------------------------------------------------ |
| Cliente sin registrar | Representa a un cliente casual de la biblioteca  | Usuario Sistema  | Usar las instalaciones de la biblioteca                      |
| Cliente Registrado    | Cliente habitual de la biblioteca                | Usuario producto | Ciertos privilegios ante clientes sin registrar              |
| Bibliotecario         | Trabajador de la biblioteca                      | Usuario producto | Atiende a los clientes, les ayuda en sus búsquedas y les da la información que necesitan. |
| Proveedor de libros   | Junta de la comunidad autónoma / empresa privada | Usuario Sistema  | Proporcionar libros a la biblioteca para que esté actualizada |
| Propietario           | Dueño o encargado principal de la biblioteca     | Usuario producto | Gestiona la biblioteca                                       |

<u>Perfil de los implicados:</u>

| Cliente sin registrar  |                                                              |
| ---------------------- | ------------------------------------------------------------ |
| Representante          | Pablo Lámpara                                                |
| Descripción            | Cliente sin registrar                                        |
| Tipo                   | Usuario Casual de la biblioteca, va pocas veces al año para tomar algún libro prestado |
| Responsabilidades      | Cuidar las instalaciones y mantener silencio                 |
| Criterios de éxito     | Cuidar las instalaciones                                     |
| Implicación            | Usar libros y cuidar las instalaciones                       |
| Comentarios/Cuestiones |                                                              |

| Cliente registrado     |                                                              |
| ---------------------- | ------------------------------------------------------------ |
| Representante          | Juan Boli                                                    |
| Descripción            | Cliente  registrado                                          |
| Tipo                   | Usuario común de la biblioteca, va con regularidad para tomar algún libro prestado |
| Responsabilidades      | Cuidar las instalaciones y mantener silencio y respetar el material |
| Criterios de éxito     | Que pueda realixar sus actividades de la forma más sencilla posible |
| Implicación            | Utilizará el sistema para registrarse o de vez en cuando para consultar sus préstamos |
| Comentarios/Cuestiones |                                                              |



| Bibliotecario          |                                                              |
| ---------------------- | ------------------------------------------------------------ |
| Representante          | Álvaro Folio                                                 |
| Descripción            | Bibliotecario                                                |
| Tipo                   | Trabajador de la biblioteca                                  |
| Responsabilidades      | Cuidar las instalaciones, obligar a mantener silencio, utilizar el sistema para gestionar usuarios y libros, ayudar a los clientes con las consultas, principal persona de cara al público, encargado de comunicar los libros que hagan falta. |
| Criterios de éxito     | Correcta funcionalidad de la biblioteca                      |
| Implicación            | Responsable de la biblioteca por debajo del Propietario      |
| Comentarios/Cuestiones |                                                              |



| proveedor de libros    |                                                    |
| ---------------------- | -------------------------------------------------- |
| Representante          | Editorial Libros                                   |
| Descripción            | Proveedor                                          |
| Tipo                   |                                                    |
| Responsabilidades      | Mantener a la biblioteca actualizada y ser fiel    |
| Criterios de éxito     | Biblioteca tiene los libros que los clientes piden |
| Implicación            |                                                    |
| Comentarios/Cuestiones |                                                    |



| Propietario            |                                                              |
| ---------------------- | ------------------------------------------------------------ |
| Representante          | Antonio Ratón                                                |
| Descripción            | Propietario / Administrador                                  |
| Tipo                   | Experto                                                      |
| Responsabilidades      | Gestión de los proveedores<br />Gestión económica            |
| Criterios de éxito     | Hay éxito si hay un buen control de los libros existentes y pedidos. También si se conoce qué proveedores suministran qué libros y se gestionan los pagos de éstos. Hay éxito si se conocen los ingresos y gastos del negocio |
| Implicación            | Responsable de los pedidos y pagos a los proveedores. Gestión económica |
| Comentarios/Cuestiones |                                                              |



<u>Necesidades principales:</u>

| Necesidad                         | Prioridad | Problema                                                     | Solución Actual                             | Solución Propuesta                                          |
| --------------------------------- | --------- | ------------------------------------------------------------ | ------------------------------------------- | ----------------------------------------------------------- |
| Tomar libros prestados            | Alta      | Pocos ejemplares de un libro                                 | Libros más demandados tienen más ejemplares | Pedir más ejemplares                                        |
| Consulta libros                   | Media     | Puede que los libros no estén donde deban estar              | Pedir a los usuarios que los devuelvan      | Devolver al bibliotecario                                   |
| Consultar libros en la biblioteca | Alta      | Pocos ejemplares de un libro o puede que web no esté actualizada con ejemplares disponibles | Bibliotecario actualiza                     | Sistema automático de actualización de ejemplares restantes |
|                                   |           |                                                              |                                             |                                                             |



**8.Realice una lista de objetivos y de requisitos estructurada de la gestión de una biblioteca.**

***Objetivos***

​	OBJ-1. El sistema deberá almacenar y gestionar la información sobre los libros de la biblioteca, tanto disponibles como en préstamo.

​	OBJ-2. El sistema debe automatizar todas las actividades que impliquen a los socios.

​	OBJ-3. Solo los administradores del sistema podrán modificar la información en la base de datos del sistema.

​	OBJ-4. Cualquier usuario debe poder consultar la disponibilidad de los libros en el momento.

***Requisitos***

​	RF-1. Gestión de libros
​	El sistema deberá llevar el control del estado de todos los libros de la biblioteca, tanto disponibles como en préstamo.

​		RF-1.2. Consultar el estado de un libro. (Disponible o no, y en caso de no estarlo, cuándo acaba el préstamo)

​		RF-1.3. Si un libro está en mal estado, debe retirarse y darlo de baja.

​	RF-2. Gestión de socios
​    El sistema deberá llevar el control de los socios de la biblioteca.

​		RF-2.1. Hacer socio a una persona.

​		RF-2.2. Obtener información sobre un socio.
 			RF-2.2.1 Ver los datos personales de un socio
 			RF-2.2.2 Ver los libros que ha cogido en un determinado momento

​		RF-2.3. Modificar los datos de un socio RF-2.4. Eliminar socio.

​	RF-3. Gestión de préstamos 

​		RF-3.1. Obtener libro.RF-3.2. Devolver libro.
​		RF-3.3. Consultar disponibilidad de un libro. 