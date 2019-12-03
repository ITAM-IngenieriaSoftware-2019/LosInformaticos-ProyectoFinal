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

## 7. Arquitectura 

## 8. Metodología

## 9. Código del proyecto (Pantallas de la aplicación)

## 10. Documentación para replicar


## Equipo Los Informáticos
Creado el 3 de Diciembre de 2019


## 1. Introducción

### 1.1 Propósito

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

### 2.2 Funcionalidad del producto

### 2.3 Clases de usuario y características

### 2.4 Ambiente de operación
El sistema actual es alojado en in servidor de Windows con un Microsoft SQL server para la base de datos por lo que reutilizaremos el equipo existente.

### 2.5 Limitaciones de diseño e implementación

### 2.6 Documentación del usuario

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
#### Interface 4

### 3.2 Hardware Interfaces
#### Interface 1
#### Interface 2
#### Interface 3
#### Interface 4

### 3.3 Software Interface

### 3.4 Interfaz de Comunicación


## 4. Funcionalidades del Sistema

### 4.1 Entrar al sistema con correo y contraseña del usuario
#### Descripción y prioridad
#### Secuencias de respuesta
#### Requerimientos funcionalidades

### 4.2 Pedir un RappiITAM
#### Descripción y prioridad
#### Secuencias de respuesta
#### Requerimientos funcionalidades

### 4.3 Agregar un método de pago
#### Descripción y prioridad
#### Secuencias de respuesta
#### Requerimientos funcionalidades


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


## 6. Plan de Calidad


## 7. Arquitectura

El proyecto será planeado, desarrollado, desplegado y mantenido por alumnos del ITAM, esto determina muchos factores a tomar en cuenta para decidir una arquitectura para el proyecto.

- Desarrollo: Se debe de tener una estructura sencilla y que sea fácil de entender y abstraer para los desarrolladores, pues probablemente es el primer proyecto de desarrollo de software al que se enfrentan los alumnos
- Despliegue: El despliegue debe de ser lo suficientemente sencillo para que un alumno pueda entenderlo, planearlo y llevarlo a cabo, de preferencia solamente en las partes en las que sí se hicieron cambios y no todo el servicio
- Operaciones: Debido a que no hay nadie que cuide la operación, se debe de estar seguro que el software ha pasado por varias etapas de pruebas y que en caso de falla sea sencillo recuperarse y regresar al funcionamiento normal
- Mantenimiento: Después de que los alumnos abandonen la institución, otros alumnos se encargarán de mantener el código y de aumentar sus funcionalidades, en este caso es muy importante que el código sea fácilmente mantenible pues la rotación es muy rápida y los desarrolladores son inexpertos.

En general se requiere que el servicio sea sencillo, fácil de manejar y desarrollar y que cualquiera pueda entender la estructura. La arquitectura de __Microservicios__ nos ofrece alta comprobabilidad para poder asegurarnos que el software desplegado funciona correctamente, despliegue y operaciones muy sencillos pues hay muchos módulos que funcionan lo más independientes uno del otro y esto permite fácil recuperación tras una falla, ademas de tener una estructura sencilla en la queu un desarrollador puede enfocarse a una sola funcionalidad sin tener que enfrentarse a entender y trabajar con la totalidad del código.


## 8. Metodología


## 9. Código del proyecto (Pantallas de la aplicación)


## 10. Documentación para replicar

