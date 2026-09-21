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

 



