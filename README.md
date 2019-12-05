# Los Informáticos - Proyecto Final

# Software Requirement Specification for RappiITAM
Preparado por:
+ Luciano Montes de Oca Villa
+	Emilio Alfonso Venancio Landeros
+	Andoni Wadgymar Iñiguez

# Tabla de Contenidos

## 1. Introducción
1.	Propósito
2.	Convenciones del Documento
3.	Audiencia prevista y sugerencias de lectura
4.	Alcance del producto
5.	Referencias

## 2. Descripción General
1.	Perspectiva del producto
2.	Funcionalidad del producto
3.	Clases de usuario y características
4.	Ambiente de operación
5.	Limitaciones de diseño e implementación
6.	Documentación del usuario
7.	Supuestos y dependencias

## 3. Requerimientos Externos de Interfaz
1.	Interfaz de Usuario
2.	Interfaz de Hardware
3.	Interfaz de Software
4.	Interfaz de Comunicaciones

## 4. Requerimientos Funcionales
1.	Entrar al sistema con correo y contraseña del usuario
2.	Pedir un RappiITAM
3.	Agregar un método de pago

## 5. Requerimientos No Funcionales
1.	Requerimientos de rendimiento
2.	Requerimientos de seguridad
3.	Requerimientos de fiabilidad
4.	Atributos de Calidad de Software
5.	Reglas del Negocio

## 6. Plan de Calidad
1. Test Plan Identifier 
2. References 
3. Introduction 
4. Test Items 
5. Software Risk Issues 
6. Features to be Tested 
7. Features not to be Tested 
8. Approach 
9. Item Pass/Fail Criteria 
10. Suspension Criteria and Resumption Requirements 
11. Test Deliverables 
12. Remaining Test Tasks 
13. Environmental Needs 
14. Staffing and Training Needs 
15. Responsibilities 
16. Schedule 
17. Planning Risks and Contingencies 
18. Approvals 
19. Glossary 

## 7. Arquitectura 

## 8. Metodología

## 9. Código del proyecto (Pantallas de la aplicación)

## 10. Documentación para replicar


## Equipo Los Informáticos
Creado el 3 de Diciembre de 2019


## 1. Introducción

### 1.1 Propósito
El propósito de este proyecto es crear un sistema que le permita a los alumnos del Instituto Tecnológico Autónomo de México (ITAM) realizar un pedido de un RappiITAM en algún momento donde no puedan salir a comprar algo de comer por distintas razones (proyectos, tareas, exámenes finales) y que el mismo repartidor sea otro alumno del ITAM que en ese instante tenga tiempo libre para comprar el pedido solicitado y llevarlo hasta el lugar donde se solicitó el pedido.

### 1.2 Convenciones del Documento
Las prioridades elegidas para los requerimientos funcionales se eligieron de acuerdo a cómo se encuentran relacionadas unas con otras.
Asimismo cada requisito tiene su propia prioridad y consideramos que todas las prioridades son altas por el hecho de que sin uno de esos requisitos el sistema no estaría completo y no funcionará adecuada y correctamente.
Por otro lado, para la realización del presente documento utilizamos lenguaje Markdown.
Para las estimaciones, decidimos tomar como referencia las dificultades del videojuego Halo, las cuales se definen de la siguiente forma: Fácil (Mini), Normal (Medium), Heroico (Maxi) y Legendario (Giant).

### 1.3 Audiencia prevista y sugerencias de lectura
La audiencia que tenemos provista para la lectura de este documento son los desarrolladores y programadores de software. Para realizar una buena lectura del proyecto, es recomendable leer en el orden en cómo se van presentando cada una de las secciones. De igual manera, si el lector tuviese dudas con respecto a la comprensión de los contenidos del documento, puede visitar las referencias abajo citadas.
Finalmente, el documento se divide en las siguientes secciones: Introducción, Descripción General, Requisitos de Interfaz Externa, System Features, y Otros Requisitos No Funcionales.

### 1.4 Alcance del producto

### 1.5 Referencias
Wiegers, K. (1999). Software Requirements Specification. Recuperado el 25 de Octubre de 2019, de https://drive.google.com/file/d/15UdWMiunZWb1OsIafbTSl1qdl2_EUgeH/view

## 2. Descripción general

### 2.1 Perspectiva del producto
Este producto pretende crear una aplicación de "gig-economy" que permita a un mensajero llevar comida a los alumnos del ITAM a cualquier hora de clase. Se utilizaran las bases de datos existentes de los alumnos del ITAM.

### 2.2 Funcionalidad del producto
+ Inicio de sesión para alumnos del ITAM
+ Solicitar un pedido de RappiITAM
+ Agregar un método de pago
+ Consultar historial de pedidos

### 2.3 Clases de usuario y características
Se deben de definir las siguientes clases:

1. Alumno
+ Nombre
+ Clave Única
+ Celular
+ Correo electrónico
+ Calificación promedio

2. Repartidor
+ Nombre
+ Clave Única
+ Celular
+ Correo electrónico
+ Calificación promedio

3. Pedido
+ Clave del pedido
+ Precio total
+ Hora estimada de entrega
+ Descripción

### 2.4 Ambiente de operación
El sistema actual es alojado en in servidor de Windows con un Microsoft SQL server para la base de datos por lo que reutilizaremos el equipo existente.

### 2.5 Limitaciones de diseño e implementación
Debido a que no se tiene acceso al servidor en el que se va a montar la fase de pruebas, puede ser complicada realizar las pruebas del producto para su correcto funcionamiento. Tampoco se tiene acceso a la base de datos de los alumnos por políticas de la institución.
Solicitaremos ayuda al ITAM para verificar el funcionamiento de la aplicación con sus bases de datos y del mantenimiento futuro de la aplicación, aunque nosotros nos encargaremos del funcionamiento en mayor medida.

### 2.6 Documentación del usuario
El usuario contará con un manual para pedir de forma correcta un RappiITAM y saber cómo funciona el proceso de entrega. También el usuario contará con un manual para saber cómo agregar un método de pago (efectivo, tarjeta de crédito, etc.)y otro manual para saber cómo consultar sus pedidos anteriores (historial).

### 2.7 Supuestos y dependencias
El proyecto depende enteramente del funcionamiento de las bases de datos existentes y del correcto acoplamiento del servidor de bases de datos con la nueva aplicación.


## 3. Requerimientos Externos de Interfaz

### 3.1 Interfaz de usuario
"Los interfaces entre el usuario y el software son de gran importancia ya que un mal interface puede llegar a confundir al usuario y no darle la accesibilidad de lograr las acciones que desea realizar".
#### Interface 1
El usuario se encuentra en la pantalla de log in en donde debería ingresar su correo del ITAM al igual que la contraseña que tiene asignada o que el especifico. En el caso en el que el usuario tenga alguno de los dos datos incorrectos será marcado el error con letras rojas y tendrá la oportunidad de volverlo a intentar. Si el usuario no recuerda la contraseña que asigno, tendrá la opción de asignar una nueva en otra pestaña, que sería la segunda interface. Si el usuario proporciona los datos de forma correcta, será mandado al interface 3.
#### Interface 2
El usuario se encuentra en el interface donde puede asignar una nueva contraseña. Primero debe mandar un correo a otra cuenta de correo electrónico en donde tendrá el link para asignar una nueva contraseña. Una vez hecho esto el usuario deberá crear una nueva contraseña con las características que se requieran y cuando esto se cumpla el sistema cambiara la contraseña. El usuario será redirigido a la primera interfaz en donde podrá acceder con su nueva contraseña.
#### Interface 3
El usuario se encuentra en la pantalla donde podrá pedir un RappiITAM. La interfaz cuenta con un campo para seleccionar entre los distintos locales, tiendas y restaurantes de comida o bebidas aledaños al ITAM. Al seleccionar un restaurante, se despliega otro campo donde se podrá elegir productos del menú o que se vendan en dicho establecimiento. Después habrá un botón para confirmar el pedido y nos llevará a seleccionar un método de pago registrado. Si no hay ninguno, la aplicación nos redirige a la _Interface 4_ donde el usuario podrá registrar el método que desee. Si el usuario decide pagar con tarjeta, el sistema le solicitará el código de seguridad. Después de registrar el método de pago, el sistema buscará una persona disponible para llevar el pedido y se visulizará el tiempo estimado de entrega y precio final del pedido. Cuando se entregue el pedido, el sistema nos redirigirá a la _Interface 5_ donde aparecerá tu recibo y un campo para calificar a tu repartidor.
#### Interface 4
El usuario se encuentra en la pantalla para registrar algún método de pago con el que desee pagar su pedido de RappiITAM. La interfaz cuenta con un campo para seleccionar el método a registrar entre efectivo, tarjeta de crédito o tarjeta de débito. Si seleccionas efectivo, el sistema pedirá que elijas (de preferencia) con qué billete vas a relizar el pago de tu pedido. Si eliges alguna de las tarjetas, el sistema deplegará varios campos donde solicitará al usuario lo siguiente: nombre y apellido del titular, número, fecha de vencimiento y banco. Después de registrar el método de pago deseado, el sistema desplegará un botón para confirmar el registro del método de pago deseado.
#### Interface 5
El usuario se encuentra en la pantalla donde podrá revisar su recibo del pedido que recibió y se visualizará un campo donde se le pida al usuario que califique a su repartidor y la experiencia que tuvo al comprar por la aplicación de RappiITAM. Aquí podrá darle desde 1 hasta 5 estrellas al repartidor (donde 1 es la calificación más baja y 5 la más alta). Después de otorgar una calificación, el sistema redirigirá al usuario a la _Interface 3_ donde podrá realizar otro pedido si así lo desea.

### 3.2 Hardware Interfaces
#### Interface 1
#### Interface 2
#### Interface 3
#### Interface 4

### 3.3 Software Interface
Todos los interfaces tienen que tener una interconexión entre ellas al igual que una conexión con la base de datos. Como varios de los datos requeridos en una interface te dan acceso a otra interface, es necesario que exista una conexión entre todas. La base de datos igual debe de poder ser modificada ya que al realizar un pedido, el sistema registrará ese nuevo pedido y las calificaciones promedio de los usuarios y repartidores cambiarán constantemente. Esta conexión es escencial y hara que el sistema tengan un funcionamiento correcto.

### 3.4 Interfaz de Comunicación
Los usuarios que ingresan a realizar un pedido de RappiITAM deben de tener un correo del ITAM. En el caso que no recuerden una contraseña se mandara un correo para recuperarla a un e-mail privado. De igual manera se contara con un network server communication en el caso de que se presente un error en el sistema el cual necesite de atenciones personales y/o profesionales. La seguridad con la que cuenta el sistema debe ser alta para que se pueda mantener privada y segura la información de los alumnos y no pueda ser atacada. Se hará uso de encriptados para que la información este fuera del alcance de otras personas.


## 4. Funcionalidades del Sistema

### 4.1 Entrar al sistema con correo y contraseña del usuario
#### Descripción y prioridad
Pantalla de login para el usuario de pedidos RappiITAM. En esta pantalla el usuario puede ingresar los datos necesarios para ingresar al sistema. Esta nueva funcionalidad tiene alta prioridad.
#### Secuencias de respuesta
+ Si el usuario inserta una combinación de nombre de usuario y contraseña correctos, se le redirigirá a los menús
+	Si el usuario inserta una combinación de nombre de usuario y contraseña incorrectos, mostrar un mensaje acorde. Ej. "Usuario/Contraseña incorrectos"
+	Si el usuario no recuerda su contraseña, hará clic una etiqueta que lo redirigirá a una pantalla de recuperación de usuario/contraseña
#### Requerimientos funcionalidades
* Req-1: Los usuarios que cuentan con su correo del ITAM y su contraseña deben de poder entrar al sistema. i. La pantalla de inicio cuenta con dos campos para ingresar texto (nombre de usuario y contraseña), un botón para validar los campos ingresados
* Req-2:	La pantalla de inicio debe de contar con una etiqueta para redirigir a otra pantalla de recuperación de contraseña i. La funcionalidad de esta pantalla de recuperación de contraseña todavía está en proceso
* Req-3:	Cuando un usuario no cuenta con un nombre y contraseña correctos el sistema debe de mostrar un mensaje acorde, en donde se indique que el error es debido a que la combinación de correo y contraseña no fue correcta.

### 4.2 Pedir un RappiITAM
#### Descripción y prioridad
Esta funcionalidad permitirá que el usuario (alumno) pida un RappiITAM del establecimiento que desee. La prioridad de esto es muy alta.
#### Secuencias de respuesta
+ Si el usuario intenta pedir un RappiTAM cuando ya tenga un pedido en camino, el sistema no le permitirá realizar el pedido indicando que no se permite realizar un pedido hasta que el pedido en proceso finalice.
+ Si el usuario intenta realizar un pedido con un monto mayor al crédito de su tarjeta (en caso de seleccionar alguna tarjeta), el sistema no permitirá solicitar el pedido.
#### Requerimientos funcionalidades
* Req-1: Pantalla de selección de restaurante o tienda 
* Req-2: Pantalla de error 
* Req-3: Pantalla de búsqueda avanzada de productos
* Req-4 (opcional): Pantalla de solicitud de código de seguridad (en caso de realizar el pago con tarjeta)
* Req-4: Pantalla de visualización del pedido y precio final 
* Req-5: Pantalla de confrimación del pedido
* Req-6: Pantalla de tiempo estimado de entrega del pedido

### 4.3 Agregar un método de pago
#### Descripción y prioridad
Esta funcionalidad permitirá al usuario registrar algún método de pago. La prioridad de esta funcionalidad es muy alta.
#### Secuencias de respuesta
+ Si el usuario intenta registrar una tarjeta que ya esté guardada, el sistema le enviará un mensaje de error indicando que ya se registró dicha tarjeta.
+ Si el usuario coloca algún dato incorrecto, como un número o la fecha de vencimiento, el sistema le enviará un mensaje de rror indicando que los datos registrados son incorrectos y que se deben de verificar.
#### Requerimientos funcionalidades
* Req-1: Pantalla de selección de método (efectivo, tarjeta de crédito, tarjeta de débito)
* Req-2: Pantalla de registro de datos bancarios (en el caso de tarjetas)
* Req-3: Pantalla de error
* Req-4: Pantalla de confirmación de método de pago


## 5. Requerimientos No Funcionales

### 5.1 Requerimientos de Rendimiento
En general el performance de nuestro sistema debe ser constante y funcional pero hay una época en la cual debe aumentar su funcionamiento y no fallar por ningún motivo, esto es cuando se acercan los exámenes finales y los alumnos no pueden salir a comprar comida por seguir estudiando. Nuestro sistema debe de tener la capacidad de poder seguir funcionando aunque la cantidad de usuarios sea muy alta y todos quieran pedir un RappiITAM al mismo instante. Un alumno no puede quedarse sin la oportunidad de solicitar un RappiITAM o que se cancele el pedido por errores de nuestro sistema por lo cual debe estar funcionando sin problemas.
De igual manera el sistema y las interfaces deben ser faciles de comprender para que los usuarios no encuentren dificultades en sus procesos de inscripción.

### 5.2 Requerimientos de Seguridad
Como se menciono en el punto 3 el sistema debe de ser lo más seguro posible ya que información muy relevante se encuentra en la base de datos. Los datos de los alumnos al igual que sus historiales de pedidos y órdenes favoritas están todas bajo la misma de base de datos y un descuido puede resultar en graves problemas.
Debe de haber cero tolerancia hacia la publicación de información personal o del sistema por parte de los developers y por parte de los usuarios. Se deben de tener los firewalls necesarios para prevenir la entrada de un hacker o de un virus que pueda dañar el sistema y los datos que contiene.
El usuario debe de aceptar los términos y condiciones que formen parte del sistema para que se pueda mantener un balance en la seguridad y en las medidas de prevención.

### 5.3 Requerimientos de Seguridad
El usuario debe de acceder al sistema con su correo electrónico institucional o con su nombre de usuario corto y con su PIN.

### 5.4 Atributos de Calidad de Software
El enfoque de este sistema debe de ser el de alta disponibilidad en horas pico, pues el tráfico esta concentrado en un día cercano a exámenes finales donde la mayoría de los alumnos no pueden salir a comer por continuar estudiando para los exámenes.

### 5.5 Reglas del Negocio
Cualquier alumno del ITAM puede solicitar el pedido de un RappiITAM sin importar su género, raza, religión, condición física, discapacidades o su posición social (si es becado o no). Lo anterior también aplica para los repartidores que tengan la posibilidad de aceptar y llevar los pedidos.


## 6. Plan de Calidad

### 6.1 Test Plan Identifier 

### 6.2 References 

### 6.3 Introduction 

### 6.4 Test Items 

### 6.5 Software Risk Issues 

### 6.6 Features to be Tested 

### 6.7 Features not to be Tested 

### 6.8 Approach 

### 6.9 Item Pass/Fail Criteria 

### 6.10 Suspension Criteria and Resumption Requirements 

### 6.11 Test Deliverables 

### 6.12 Remaining Test Tasks 

### 6.13 Environmental Needs 

### 6.14 Staffing and Training Needs 

### 6.15 Responsibilities 

### 6.16 Schedule 

### 6.17 Planning Risks and Contingencies 

### 6.18 Approvals 

### 6.19 Glossary 


## 7. Arquitectura

El proyecto será planeado, desarrollado, desplegado y mantenido por alumnos del ITAM, esto determina muchos factores a tomar en cuenta para decidir una arquitectura para el proyecto.

- Desarrollo: Se debe de tener una estructura sencilla y que sea fácil de entender y abstraer para los desarrolladores, pues probablemente es el primer proyecto de desarrollo de software al que se enfrentan los alumnos
- Despliegue: El despliegue debe de ser lo suficientemente sencillo para que un alumno pueda entenderlo, planearlo y llevarlo a cabo, de preferencia solamente en las partes en las que sí se hicieron cambios y no todo el servicio
- Operaciones: Debido a que no hay nadie que cuide la operación, se debe de estar seguro que el software ha pasado por varias etapas de pruebas y que en caso de falla sea sencillo recuperarse y regresar al funcionamiento normal
- Mantenimiento: Después de que los alumnos abandonen la institución, otros alumnos se encargarán de mantener el código y de aumentar sus funcionalidades, en este caso es muy importante que el código sea fácilmente mantenible pues la rotación es muy rápida y los desarrolladores son inexpertos.

En general se requiere que el servicio sea sencillo, fácil de manejar y desarrollar y que cualquiera pueda entender la estructura. La arquitectura de __Microservicios__ nos ofrece alta comprobabilidad para poder asegurarnos que el software desplegado funciona correctamente, despliegue y operaciones muy sencillos pues hay muchos módulos que funcionan lo más independientes uno del otro y esto permite fácil recuperación tras una falla, ademas de tener una estructura sencilla en la queu un desarrollador puede enfocarse a una sola funcionalidad sin tener que enfrentarse a entender y trabajar con la totalidad del código.


## 8. Metodología

Para la realización de este proyecto, elegimos la metodología __En Cascada__ por encima de las metodologías siguientes: Por Prototipos, Agile, Rapid, Dinámica, Espiral, Extreme Programming y Feauture Driven.

La razón de esta elección es que nuestro proyecto no está pensado para poco tiempo y tenemos bien definido qué vamos a hacer y hacia dónde vamos. En nuestro proyecto vamos siguiendo un orden establecido y hasta no terminar con alguna fase continuamos con la siguiente. De esta manera nos aseguramos que nuestro proyecto este completo y tenga toda la funcionalidad adecuada para que no haya fallas al momento de lanzarla al mercado. 

En primer lugar analizamos todos los requisitos que nos solicitaron. Después hicimos el diseño del programa y de nuestro sistema. Luego realizamos las pruebas pertinentes para asegurar el correcto funcionamiento del proyecto. Seguido de esto, verificamos todo el programa. Por último, realizaremos el mantenimiento del sistema (en caso de que hubiese fallas). De esta forma cualquier error que identifiquemos durante la etapa de desarrollo del proyecto, se identifica rápidamente y esto nos conduce a solucionarlo para poder continuar con los siguientes procesos.


## 9. Código del proyecto (Pantallas de la aplicación)


## 10. Documentación para replicar

