# Los Informáticos - Proyecto Final

## Arquitectura del software

El proyecto será planeado, desarrollado, desplegado y mantenido por alumnos del ITAM, esto determina muchos factores a tomar en cuenta para decidir una arquitectura para el proyecto.

- Desarrollo: Se debe de tener una estructura sencilla y que sea fácil de entender y abstraer para los desarrolladores, pues probablemente es el primer proyecto de desarrollo de software al que se enfrentan los alumnos
- Despliegue: El despliegue debe de ser lo suficientemente sencillo para que un alumno pueda entenderlo, planearlo y llevarlo a cabo, de preferencia solamente en las partes en las que sí se hicieron cambios y no todo el servicio
- Operaciones: Debido a que no hay nadie que cuide la operación, se debe de estar seguro que el software ha pasado por varias etapas de pruebas y que en caso de falla sea sencillo recuperarse y regresar al funcionamiento normal
- Mantenimiento: Después de que los alumnos abandonen la institución, otros alumnos se encargarán de mantener el código y de aumentar sus funcionalidades, en este caso es muy importante que el código sea fácilmente mantenible pues la rotación es muy rápida y los desarrolladores son inexpertos.

En general se requiere que el servicio sea sencillo, fácil de manejar y desarrollar y que cualquiera pueda entender la estructura. La arquitectura de __Microservicios__ nos ofrece alta comprobabilidad para poder asegurarnos que el software desplegado funciona correctamente, despliegue y operaciones muy sencillos pues hay muchos módulos que funcionan lo más independientes uno del otro y esto permite fácil recuperación tras una falla, ademas de tener una estructura sencilla en la queu un desarrollador puede enfocarse a una sola funcionalidad sin tener que enfrentarse a entender y trabajar con la totalidad del código.
