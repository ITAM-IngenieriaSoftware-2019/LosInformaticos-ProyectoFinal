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
2.	Inscribir Materia
3.	Baja de Materias

## 5. Requerimientos No Funcionales
1.	Requerimientos de rendimiento
2.	Requerimientos de seguridad
3.	Requerimientos de fiabilidad
4.	Atributos de Calidad de Software
5.	Reglas del Negocio

## 6. Arquitectura del Software


## Equipo Los Informáticos
Creado el 3 de Diciembre de 2019


## 1. Introducción

### 1.1 Propósito

### 1.2 Convenciones del Documento

### 1.3 Audiencia prevista y sugerencias de lectura

### 1.4 Alcance del producto

### 1.5 Referencias


## 2. Descripción general

### 2.1 Perspectiva del producto

### 2.2 Funcionalidad del producto

### 2.3 Clases de usuario y características

### 2.4 Ambiente de operación

### 2.5 Limitaciones de diseño e implementación

### 2.6 Documentación del usuario

### 2.7 Supuestos y dependencias


## 3. Requerimientos Externos de Interfaz

### 3.1 Interfaz de usuario
#### Interface 1
#### Interface 2
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

### 4.2 
#### Descripción y prioridad
#### Secuencias de respuesta
#### Requerimientos funcionalidades

### 4.3
#### Descripción y prioridad
#### Secuencias de respuesta
#### Requerimientos funcionalidades


## 5. Requerimientos No Funcionales

### 5.1 Requerimientos de Rendimiento

### 5.2 Requerimientos de Seguridad

### 5.3 Requerimientos de Seguridad

### 5.4 Atributos de Calidad de Software

### 5.5 Reglas del Negocio


## 6. Arquitectura del software

El proyecto será planeado, desarrollado, desplegado y mantenido por alumnos del ITAM, esto determina muchos factores a tomar en cuenta para decidir una arquitectura para el proyecto.

- Desarrollo: Se debe de tener una estructura sencilla y que sea fácil de entender y abstraer para los desarrolladores, pues probablemente es el primer proyecto de desarrollo de software al que se enfrentan los alumnos
- Despliegue: El despliegue debe de ser lo suficientemente sencillo para que un alumno pueda entenderlo, planearlo y llevarlo a cabo, de preferencia solamente en las partes en las que sí se hicieron cambios y no todo el servicio
- Operaciones: Debido a que no hay nadie que cuide la operación, se debe de estar seguro que el software ha pasado por varias etapas de pruebas y que en caso de falla sea sencillo recuperarse y regresar al funcionamiento normal
- Mantenimiento: Después de que los alumnos abandonen la institución, otros alumnos se encargarán de mantener el código y de aumentar sus funcionalidades, en este caso es muy importante que el código sea fácilmente mantenible pues la rotación es muy rápida y los desarrolladores son inexpertos.

En general se requiere que el servicio sea sencillo, fácil de manejar y desarrollar y que cualquiera pueda entender la estructura. La arquitectura de __Microservicios__ nos ofrece alta comprobabilidad para poder asegurarnos que el software desplegado funciona correctamente, despliegue y operaciones muy sencillos pues hay muchos módulos que funcionan lo más independientes uno del otro y esto permite fácil recuperación tras una falla, ademas de tener una estructura sencilla en la queu un desarrollador puede enfocarse a una sola funcionalidad sin tener que enfrentarse a entender y trabajar con la totalidad del código.
