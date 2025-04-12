# Propuesta TP DSW

## Grupo
### Integrantes
47057 - Bruzzesi, Ignacio <br>
47240 - Oviedo, Bernardo <br>
46122- Sabbioni, Santiago

### Repositorios
* [frontend app](http://hyperlinkToGihubOrGitlab)
* [backend app](http://hyperlinkToGihubOrGitlab)


## Tema
Gestion de clubes
### Descripción
Pagina web destinada a instituciones deportivas incorporando la gestión de socios, pagos de cuotas, noticias, entre otras. Esto servira para que los socios o fanáticos del club puedan estar al tanto de novedades y tener un lugar donde gestionar su membresía como socios en el caso de serlo. También ayuda a tener datos internos como la cantidad exacta de socios del club, cuántos usuarios son socios y a saber qué opinan los usuarios de las noticias del club mediante una sección de comentarios particular para cada novedad.
Las noticias que tengan lugar dentro del club actualizadas momento a momento con notas de jugadores post partidos, logros obtenidos, futuros encuentros deportivos, actividades realizadas dentro de la institución o nuevo merchandising del club. 

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 
### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de clubes de futbol

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Usuario <br>2. CRUD Noticias|
|CRUD dependiente|1. CRUD Socio {depende de} CRUD Cuota<br>2. CRUD Cliente {depende de} CRUD Localidad|<br>3. CRUD Comentario {depende de} CRUD Usuario|
|Listado<br>+<br>detalle| 1. Listado de SOCIO filtrado por los que estan al dia y los que no, muestra nro y tipo de socio => detalle CRUD Socio<br> 2. Listado de noticias filtrado por rango de fecha, muestra titulo de la noticia, fecha, foto de la noticia y breve descripcion => detalle muestra un listado de noticias|
|CUU/Epic|1. Asociarte al club<br>2. Realizar una edicion dentro de las noticias del club|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Tipo Habitacion<br>2. CRUD Servicio<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|
