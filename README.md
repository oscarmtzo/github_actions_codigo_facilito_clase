# GitHub actions - clase de Codigo Facilito

*Fuente: https://sre.google/books/*

## ¿Que es integracion Continua (CI)?
- Es un sistema que automaticamente compila y ejecuta todas las pruebas cada vez que un desarrollador 💻 sube nuevo codigo

### Beneficios de Integracion Continua 

## ¿Que es integracion Continua (CD)?
- Despliegue automatizado del codigo a los diferentes entonrnos de pruebas (**test || QA - Quality Assurance**), desarollo (**Dev**) o produccion (**PROD**)

## Estrategias de Despliegue 
- [![5 Deploy Patterns](https://www.devopsschool.com/blog/wp-content/uploads/2023/08/1691822296549.gif)]
### Despliegue Big Bang
- Actualiza todo el sistema de una sola vez, *similar a quitar un curita rapidamente*
- Tiene un tiempo de **no disponibilidad en mis applicaciones** *no downtime*
    - es decir que tarde desde segundos a unos minutos en la aplicacion en ejecutarse

### Despliegue Rolling 
- Actualiza el sistema por partes; se actualiza un servidor a la vez mientras los demás siguen funcionando

### Despliegue Blue Green
- Usa dos ambientes idénticos:
    - **Blue**: env (ambiente) activo 
        - atienda a usuarios
    - **Green**: env (ambiente) pasivo
        - se prueba la nueva version
    - No tiene downtime
    - Requiere tener mas infraestructura, mas costo, mas servidores, mas hardware
        - MTTR: Mean Time to Recovery - tiempos bajos de provisionamiento de la aplicación
            ![MTTR: Mean Time to Recovery](https://dt-cdn.net/wp-content/uploads/2022/11/mttr-stages-rc.png)  

### Despligue Canario
- Prueba de nueva version econ pequeño grupo de usuarios antes de lanzarla a todos los usuarios 

