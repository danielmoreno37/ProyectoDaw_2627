# Sistema de Ticketing para incidencias o solicitudes de Empresas
---

## Identificación de necesidad o problema
Muchas empresas ofrecen servicios de mantenimiento / limpieza o otros servicios para otras empresas.

En estas empresas son frecuentes las incidencias de otras empresas solicitando un servicio ya que ha ocurrido un problema.

Vamos a ponernos en el caso de una empresa de IT la cual da los servicios informáticos a otras empresas.

De normal hay un telefono al que se llama cuando ocurre un problema, y eso obliga al trabajador de la empresa IT a detener su tarea para poder ayudar al cliente y así constantemente con las llamadas de otros clientes.

---

## Proposito de la Aplicación
Con el sistema de Ticketing podemos hacer que no haya un colapso en los trabajadores que atienden las incidencias, ya que estos no pararian su trabajo actual por atender a la incidencia, ya que el cliente o una persona interna en la empresa (en función de como se quiera aplicar el sistema), tendría que rellenar un formulario argumentando con sus palabras la incidencia.

Una vez rellenado el formulario de incidencia, a la empresa IT le aparecerá dicha incidencia en su DashBoard.

---

## Identificación de los usuarios
Para esta app web en función de la empresa exitirán los usuarios que la empresa quiera, pero minimamente existirá un usuario.

El usuario administradorEmpresa que permitirá configurar su sistema de tickets para su empresa. Este mas tarde podrá habilitar usuarios para sus Trabajadores y usuarios para sus Clientes.

###### AdministradorEmpresa - Usuario Obligatorio
En este usuario va a ser el usuario que puede controlar el panel y hacer los cambios que este considere.
Este usuario se va a llamar tal cual AdministradorNombreEmpresa, por ejemplo, AdministradorMUSEPAN, este sería por ejemplo el administrador de la plataforma de tickets para la Mutua de Seguros de Panaderos de Valencia.
Este usuario por seguridad solo puede tener un inicio de sesión.

###### TrabajadorEmpresa - Usuaerio Optativo (Recomendado tenerlo).
Este usuario va a ser el usuario para los trabajadores de la empresa que presta el servicio. 
Por ejemplo el usuario de Pepe Devesa que es un trabajador de mi empresa, se llamaría pdevesaMUSEPAN y este usuario no puede dar de alta usuarios ni eliminarlos, tampoco empresas ni nada, solo ve los tickets y los soluciona, también puede crear tickets a nombre de otras empresas.
Un usuario por trabajador

###### NombreEmpresaCliente - Usuario Optativo
Este usuario es el usuario de las empresas, este podrá tener, maximo 3 inicios de sesión.
Su nombre de usuario será PanaderíaIsabel. Y cuando rellene el formulario ya tendrá algunos campos resueltos como puede ser el nombre de empresa y el cif.
Este usuario tendrá un maximo de 3 inicios de sesión en una misma cuenta, si se quieren más deberá ser ampliado.

###### Invitado
Este usuario no le hará falta registro, solo deberá rellenar un formulario donde tendrá que introducir su nombre de empresa y cif y rellenar todos los campos que con el inicio de sesión se autorellenan.

---

## Alcance del proyecto
Como se ha indicado antes, este proyecto esta enfocado para empresas las cuales tienen un servicio de incidencias, sean empresas de IT o cualquier empresa que atienda a estas.

Para la parte Empresa va a tener:
- Panel de configuración del entorno
- Panel tipo DashBoard donde aparecerán las incidencias.
- Panel de formulario de envio de incidencias interno a nombre propio o de clientes
- Diseño responsive
- Navegación entre secciones
- Sistema de usuarios y contraseñas

Para la parte cliente va a tener:
- Panel de formulario de incidencia
- Inicio de Sesión
- Registro de incidencias enviadas

Para la aprte usuario invitado va a tener:
- Panel de formulario de incidencias limitado

No se añade al sistema:
- Pasarela de pagos
- App movil
- Envio de datos a ERP

## Requisitos funcionales
- RF01: El sistema deberá permitir a los usuarios registrarse e iniciar sesión.
- RF02: El sistema deberá permitir crear, consultar, modificar y cerrar tickets de soporte.
- RF03: El sistema deberá permitir consultar el estado de los tickets.
- RF04: El sistema deberá permitir añadir mensajes o comentarios a un ticket.
- RF05: El sistema deberá permitir adjuntar archivos a los tickets.
- RF06: El sistema deberá permitir crear citas desde el módulo de Agenda.
- RF07: El sistema deberá permitir que tanto el cliente como el profesional puedan agendar citas.
- RF08: El sistema deberá permitir modificar y cancelar citas previamente creadas.
- RF09: El sistema deberá mostrar las citas organizadas en una agenda o calendario.
- RF10: El sistema deberá permitir consultar la disponibilidad horaria para agendar una cita.
- RF11: El sistema deberá permitir activar o desactivar el módulo de Ticketing.
- RF12: El sistema deberá permitir activar o desactivar el módulo de Agenda.
- RF13: El sistema deberá mostrar únicamente los módulos que estén activos para cada usuario.
- RF14: El sistema deberá enviar notificaciones relacionadas con la creación, modificación o cancelación de tickets y citas.
- RF15: El sistema deberá permitir consultar un historial de tickets y citas.


## Requisitos no funcionales
- RNF01: La aplicación deberá disponer de una interfaz sencilla e intuitiva.
- RNF02: La aplicación deberá adaptarse correctamente a ordenadores, tablets y dispositivos móviles (responsive).
- RNF03: La aplicación deberá proteger los datos personales y la información de los usuarios.
- RNF04: Las contraseñas deberán almacenarse de forma segura mediante técnicas de cifrado/hash.
- RNF05: El sistema deberá controlar los permisos de acceso según el tipo de usuario.
- RNF06: La aplicación deberá evitar que dos usuarios puedan reservar simultáneamente el mismo horario.
- RNF07: Las operaciones habituales deberán ejecutarse en un tiempo de respuesta reducido.
- RNF08: La aplicación deberá ser compatible con los principales navegadores web actuales.
- RNF09: El sistema deberá mantener la integridad de la información almacenada.
- RNF10: La aplicación deberá estar diseñada de forma modular para permitir añadir o modificar funcionalidades en el futuro.
- RNF11: La interfaz deberá proporcionar una navegación clara entre los módulos de Ticketing y Agenda.
- RNF12: El sistema deberá permitir activar o desactivar los módulos sin afectar al funcionamiento del resto de la aplicación.


## Tecnologias útilizadas
- MarkDown para la documentación
- Visual Studio Code como IDE
- IA
- DRAW.IO
- ...