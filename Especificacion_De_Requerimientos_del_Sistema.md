# Especificación de Requerimientos del Sistema de comunicación ITAM
# Versión 1.0 aprobada
# Preparado por Andrea de Anda Kuri, Miguel Ángel Cifuentes Jiménez, Damian Pérez Landeros, Isaías Jesús García Moreno
# Instituto Tecnológico Autónomo de México
# 24/11/2020
## Tabla de Contenidos
1. Introducción  
 - Propósito    
 - Convenciones del Documento    
 - Audiencia, Objetivo y Sugerencias de Lectura    
 - Alcance del producto    
2. Descripción General    
 - Perspectiva del producto    
 - Funciones del Producto    
 - Clases y Características del usuario.    
 - Ambiente de operación    
 - Documentación    
3. Requerimientos de Interfaces Externas    
 - Interfaces de usuario    
 - Interfaces del hardware    
 - Interfaces de software    
 - Interfaces de comunicación    
4. Funcionalidades del sistema    
 - Funcionalidad 1
 - Funcionalidad 2  
 - Funcionalidad 3   
5. Otros Requerimientos No Funcionales    
 - Requerimientos operacionales   
 - Requerimientos de protección  
 - Requerimientos de seguridad   
 - Atributos de Software de Calidad    
 - Reglas del negocio    
## 1. Introducción
### 1.1. Propósito
El proposito de este documento consiste en presentar los requerimientos de una aplicación que permita a los alumnos, profesores y personal administrativo del ITAM comunicarse entre si. Este documento describe la version 0 del Sistema que corresponde al prototipo interactivo.
### 1.2. Convenciones del Documento 
Convención | Término 
-- | --
ITAM | Instituto Tecnológico Autónomo de México
TI | Tecnologías de Información 
AWS | Amazon Web Services
### 1.3. Audiencia, Objetivo y Sugerencias de Lectura
Este documento está dirigido al departamento de TI del ITAM y al equipo de desarrollo del proyecto, con el objetivo de explicar las funcionalidades del sistema y sus características. Este documento contiene la información necesaria para comprender el funcionamiento, objetivo, realización y el uso del producto.
Se recomienda que la lectura de este documento sea de forma secuencial, acorde a la tabla de contenido. 
### 1.4. Alcance del producto
Proponemos una aplicación para que los alumnos, profesores y personal administrativo del ITAM puedan comunicarse entre si. Se espera que este sistema facilite la comunicación de la comunidad ITAM dentro de un solo espacio ya que anteriormente, el contacto se realizaba por sistemas externos. 
Objetivos:
 - Que la comunidad ITAM (alumnos, profesores y personal administrativo) pueda comunicarse entre si, dentro de un sistema único.
 - Que la comunicación se establezca de manera efectiva y segura; definimos como efectiva la brevedad de las respuestas de las distintas partes, que tendrán un tiempo esperado de dos días.  
 - Que esta aplicación fomente la cohesión de la comunidad, a través de la apertura de canales de comunicación.  
## 2. Descripción General
### 2.1. Perspectiva del producto
Esta aplicación busca engoblar dentro de un ambiente único la comunicación entre alumnos, profesores y personal administrativo del ITAM. Actualmente el contacto se realiza con sistemas externos y esto ocaciona confusión, lo cual afecta la comunicación entre las tres partes. Este producto surge como una solución para integrar la comunicación de la comunidad estudiantil del ITAM, de manera centralizada.   
### 2.2. Funciones del Producto
- Establecer un canal de comunicación confiable entre alumnos, profesores y personal administrativo del ITAM. 
- Asegurar que el alumno obtenga una respuesta en tiempo promedio de 36 horas. 
- Respaldar las conversaciones pasadas para resolver conlfictos puedan surgir.
- Que los usuarios puedan valorar la comuncación y la información que obtuvieron de ella, para mejorar la experiencia futura. 
- Reportar conducta inapropiada de todas las partes.
- Agendar citas con profesores o personal administrativo. 
### 2.3. Clases y Características del usuario.
Usuarios | Descripción 
-- | --
Estudiante | Persona inscrita en el ITAM que puede enviar mensajes a los demas usuarios, evaluar las respuestas recibidas, reportar, crear canales de comunicación privados o grupales y agendar citas con profesores y personal administrativo.
Docente | Empleado del ITAM que puede enviar mensajes a los demas usuarios, evaluar las respuestas recibidas, reportar, crear canales de comunicación privados o grupales y recibir citas de estudiantes.
Personal administrativo | Empleado del ITAM que puede enviar mensajes a los demas usuarios, evaluar las respuestas recibidas, reportar, crear canales de comunicación privados o grupales y recibir citas de estudiantes.
TI(administradores del sistema) | Personas encargadas de gestionar el sistema y mantener su correcto funcionamiento. Además pueden revisar los reportes y obtener el historial de mensajes de un usuario, reportar usuarios y verificar que los grupos sean correctos.
### 2.4. Ambiente de operación
La aplicación será desarrollada para tener soporte para Android 11, IOS 14 y en las ultimas versiones de los siguientes navegadores web: Chrome, FireFox, Safari, etc. La aplicación la realizaremos en kivy (python) y el manejo de los datos con AWS. 
### 2.5. Restricciones en el diseño y la implementación
- Diseño: la elaboración de los grupo debe ir acorde a la información de inscripción del ITAM. Además el diseño esta restringido por los navegadores web y el ambiente de desarrollo kivy. 
- Hardware: principalmente la aplicación está sujeta al servicio que se contrata con AWS. 
- Seguridad: está sujeta a las políticas y manejo por parte de AWS. Además, el manejo de los datos está sujeto al reglamento interno del ITAM. 
### 2.6. Documentación
Dentro de la documentación se encuentra:
- Manual de usuario: un manual de usuario para los cuatro tipos de usuarios (estudiante, docente, personal administrativo y TI), que contiene el manejo correcto de la aplicación.
- Videos tutoriales: estos videos explicarán de manera gráfica y concisa, distintas funcionalidades de la aplicación.
### 2.7. Dependencias y asunciones
Para el correcto funcionamiento asumimos que:
- El ITAM está dispuesto a pagar AWS, para mantener la aplicación funcional.
- Que el tráfico de usuarios va a permanecer dentro de un rango en el cual la escabilidad no sea necesaria ya que, el ITAM mantendrá el número de alumnos dentro de este rango.
- Que los servidores de AWS funcionen correctamente.
- Que nuestro producto cumpla con las políticas de buen uso de AWS.
## 3. Requerimientos de Interfaces Externas
### 3.1. Interfaces de usuario
### 3.2. Interfaces del hardware
La aplicación esta principalmente destinada a los dispositivos móviles sin embargo, es posible utilizarla en ordenadores. Es importante denotar que en ambos caso se debe tener una conexión a internet. 
### 3.3. Interfaces de software
Este sistema utilizará una API para interactuar con AWS y el sistema de autenticación de usuario del ITAM. En el caso del primero, los datos serán tratados y almacenados por Amazon, y mediante una api los obtendremos. Mientras que con el sistema de autenticación del ITAM, obtenemos una forma más segura para que los usuarios ingresen
### 3.4. Interfaces de comunicación
En primer lugar la comunicación entre los servidores y la web será por medio del protocolo HTTP. Con este protocolo, los datos transferidos son encriptados para lograr mayor seguridad. Más tarde, mediante el protocolo XMPP, realizaremos la transferencia de mensajes entre usuarios. Además los mensajes utilizaran el cifrado de extremo a extremo, para asegurarnos que la información de los usuarios no sea transgredida. 
## 4. Funcionalidades del sistema
### 4.1. Enviar mensaje y recibir mensajes en un canal de comunicación
#### 4.1.1. Descripción y prioridad
Este requerimiento permitirá al sistema cumplir con la funcionalidad básica de mensajería, permitirá a los usuarios enviar y recibir mensajes de texto, archivos, fotografías y videos, es nuestra funcionalidad de más alta prioridad, se le asignará el valor de prioridad 1.
#### 4.1.2. Secuencias Estímulo/Respuesta
Los usuarios entran a la aplicación, donde tendrán todos sus chats abiertos y una opción de nuevo mensaje, seleccionarán la conversación a la que quieren mandar el mensaje o aen el botón de nuevo mensaje podrán buscar por nombre o departamento a quien quieran mandar el mensaje. Una vez seleccionado el destinatario se abrirá la pantalla de la conversación y se podrá escribir el mensaje de texto o adjuntar los archivos. Tendrá un botón de enviar, una vez preionado este se enviará al servidor, que lo distribuirá al cliente correspondiente.
#### 4.1.3. Requerimientos funcionales
- REQ-1.1: Por cada mensaje no leído de alguna conversación el sistema enviará una notificación al receptor del mensaje.
- REQ-1.2: Que el número de conversaciones abiertas sólo esté limitado por la memoria del dispositivo.
- REQ-1.3: Que todos los mensajes enviados estén cifrados de extremo a extremo.
- REQ-1.4: Que el sistema permita enviar el mismo mensaje a varios usuarios.
- REQ-1.5: Que el número de mensajes recibidos esté limitado sólo por la memoria del dispositivo.
### 4.2. Crear chats
#### 4.2.1. Descripción y prioridad 
Poder crear un chat con algún miembro de la organización a quien se desee enviar un mensaje personal, tendrá prioridad alta con valor 1 ya que es parte de las funcionalidades básicas de la aplicación.  
#### 4.2.2. Secuencias Estímulo/Respuesta
Habrá un botón de crear conversación donde puedas elegir a qué persona o personas de la institución quieres mandar el mensaje, una vez seleccionados los destinatarios, se abrirá una nueva ventana de conversación con ese miembro del ITAM. Dentro del chat, el usuario podrá: enviar mensajes ilimitados a otro usuario u usuarios; visualizar los mensajes(imagenes, archivos, videos, texto) previos deslizandose hacia arriba dentro del chat y, visualizar los participantes con su foto y nombre correspondiente.
#### 4.2.3. Requerimientos funcionales
- REQ-2.1: Poder crear un grupo para mandar el mensaje seleccionando dos o más usuarios como destinatarios.
- REQ-2.2: Si se decide crear una conversación con alguien con quien ya se tiene un chat, solo se abrirá el chat que ya existía. 
- REQ-2.3: Poder tener el número de chats que la memoria del dispositivo permita. 
- REQ-2.4: Poder crear un chat con los tres distintos usuarios (estudiante, docente, personal administtrativo).
- REQ-2.5: Poder crear un chat con un usuario con el cual se tenía un chat pero se había borrado.
### 4.3. Reportar un mensaje 
#### 4.3.1. Descripción y prioridad
Poder reportar un mensaje que se considere que no cumple con el reglamento de convivencia establecido por el ITAM. Esta funcionalidad tiene prioridad 2 ya que, es una funcionalidad muy importante para conservar la buena convivencia dentro de la aplicación y evitar problemas sin embargo, no es una funcionalidad primordial para el funcionamiento básico del sistema.
#### 4.3.2. Secuencias Estímulo/Respuesta
Habrá una boton para reportar un mensaje, el cuál al seleccionarlo desplegará una ventana para confirmar que se desea reportar el mensaje. Además se debe seleccionar una o más opciones de una lista, la cual contiene las razones más comúnes que causan un reporte.   
#### 4.3.3. Requerimientos funcionales
- REQ-3.1: Poder reportar multiples mensajes dentro de un mismo chat.
- REQ-3.2: Poder seleccionar múltiples razones por la cual se realiza el reporte.
- REQ-3.3: Que el sistema permita reportar indistintamente del tipo de usuario (estudiantes, docentes, personal administrativo).
- REQ-3.4: Que el sistema permita escribir sobre una caja de texto otra razón por la cual se realizó el reporte, en el caso de que la lista de razones más comúnes no sea suficiente. 
- REQ-3.5: Que el sistema permita cerrar la ventana de reporte, en el caso que no se requiera hacer el reporte y se haya seleccionado la opción por accidente. 
- REQ-3.6: Que el sistema permita realizar un reporte sobre un mensaje de cualquier tipo. Es decir, que el sistema permita reportar videos, imagenes, archivos y mensajes de texto. 
### 4.4. Reenvio temporizado de mensajes de duda
#### 4.4.1. Descripción y prioridad 
Para evitar que una duda se quede sin respuesta, el usuario podrá recibir respuesta de los demás profesores que imparten la materia y de los estudiantes que la están cursando. Esta funcionalidad tiene prioridad alta 2, ya que es de suma importancia que las dudas de los alumnos se resuelvan en un tiempo promedio de 24 horas. 
#### 4.4.2. Secuencias Estímulo/Respuesta
El reenvio de los mensajes comenzara 12 horas después que el mensaje fue enviado, si dentro de este plazo el profesor al que se le envió la duda responde la pregunta, no será necesario reenviar el mensaje a los profesores de otros grupos. Más tarde si se cumple un plazo de 24 horas sin recibir respuesta, el mensaje será reenviado a los alumnos del grupo para ellos tambíen puedan responder a la pregunta.
#### 4.4.3. Requerimientos funcionales
- REQ-4.1: Reenviar un mensaje a los profesores después de 12 horas
- REQ-4.2: Reenviar un mensaje a los alumnos de la materia después de 24 horas
- REQ-4.3: Que el sistema solamente reenvie las dudas que no han sido contestadas, evitando mensajes de otra indole. 
- REQ-4.4: Que el sistema reenvie el mensaje asignando un nombre anonimo como autor del mensaje. Este nombre anonimo tendrá como propositó evitar alguna molestia o inconveniente que el estudiante pueda tener, en caso de que su mensaje sea reenviado a otras personas que no sean el destinatario original.
- REQ-4.5: En el caso que un mensaje cumpla alguno de los dos plazos (12 y 24 horas) el sistema debe reconocer si ya se tiene un chat abierto con los profesores o con los demás estudiantes. Con esto se evita tener grupos repetidos en el caso de que más de una duda no sea respondida por el profesor antes de las 12 horas establecidas.
- REQ-4.5: Que el sistema reenvie el número de mensajes que se hayan mandado y no tengan respuesta. Es decir, si se mando un mensaje de texto con un archivo, el sistema reenviará el mensaje de texto con el archivo. 
### 4.5. Agendar citas
#### 4.5.1. Descripción y prioridad 
Dentro de la aplicación se puede tener la opción de agendar una cita. Dicha cita es para resolver dudas con el profesor, o realizar algún trámite con un personal administrativo.
#### 4.5.2. Secuencias Estímulo/Respuesta
Habrá un boton para agendar una cita. Al presionar el botón se desplegará una pantalla con los contactos con los que se puede agendar una cita. Al seleccionar el contacto con el que deseas agendar una cita, se desplegara información para detallar la fecha y el lugar de la cita. Más tarde se seleccionará un boton para confirmar la cita el cual, desplegará una pantalla con la información de la cita y un boton de salir.
#### 4.5.3. Requerimientos funcionales
- REQ-5.1: Que el sistema permita agendar una cita con cualquier tipo de usuario(estudiantes, profesores, personal administrativo)
- REQ-5.2: Que el sistema permita que se puedan realizar multiples citas, incluso cuando ya se tienen otras citas agendadas.
- REQ-5.3: Que el sistema no permita agendar una cita en un horario en que se haya agendado una cita previamente. 
- REQ-5.4: Que el sistema realice permita ir a la pagina del ITAM para realizar una cita con profesores de otros departamentos, a los cursos que se tienen escritos en el semestre en curso.
- REQ-5.5: Que el sistema permita realizar una cita con más de un usuario.
## 5. Otros Requerimientos No Funcionales
### 5.1. Requerimientos operacionales
Los requerimientos de rendimiento nos exigen a que se satisfaga la demanda por el producto bajo todos los escenarios de estrés que al que se exponga. Para esto tenemos que considerar el número de usuarios que usarán la aplicación. El ITAM tiene 5 mil alumnos,200 profesores y 100 usuarios administrativos contando a los de IT, por lo que el sistema debe tener capacidad de atender los requests de estos 5300 usuarios. Además se espera tener un pico de usuarios en los meses de agosto a octubre de aproximadamenre 500 alumnos más, y de enero a marzo de 100 alumnos. Por lo tanto tendremos que cubrir la capacidad para 5800 usuarios. 
Estos usuarios se estima que se envíen en promedio 60 mensajes al día, por lo que tendríamos en total una concurrencia diaria de 348'000 mensajes, por lo tanto un total de 4.03 mensajes por segundo. Estimamos también que el promedio de tamaño de archivo es de 10 kb, por lo que necesitaremos 40.3 kb/s de ancho de banda. 
A través de una simulación de tiempos exponenciales con un promedio de 4.03 transacciones por segundo nos dio en promedio que se habrá un tiempo entre transacciones de 0.249 ms.
### 5.2. Requerimientos de protección
Para tener una óptima protección de los usuarios habrá un cifrado de extremo a extremo para que los mensajes, debe prevenirse el uso inadecuado de la aplicación como que se use para acoso, para esto los usuarios podrán bloquear y reportar a usuarios que hagan uso idebido de la plataforma o que tengan un comportamiento fuera de los estándares institucionales.
### 5.3. Requerimientos de seguridad
Al ser un software de uso institucional es muy importante declarar a los usuarios en un aviso de privacidad que todos los datos generados dentro de la aplicación, son propiedad del ITAM y se adecuará a la política de uso de datos de la institución. Las autenticaciones se harán con el correo institucional, y los únicos datos que se obtendrán del perfil institucional serán el nombre, la clave única y las grupos de las materias a las que está inscrito en caso de ser alumno, y las materias que imparte y a qué grupos en caso de ser profesor. También opcionalmente se podrá generar en el perfil un resumen personal con datos curriculares y áreas de interés. Estos datos estarán almacenados de acuerdo con los estándares del ITAM.
Para cuidar la integridad de los datos se procesarán los mensajes con base en un timestamp generado al momento del envío para que se procesen en el órden que se reciban en el servidor, para que se mantenga el órden lógico de la conversación.
En términos de disponiblididad de los datos, las conversaciones serán almacenadas durante un período de 6 meses antes de ser destruídas, a excepción de los mensajes que sean reportados como uso inapropiado que serán guardados mientras la aplicación se use, para tener un registro. Además de estos 6 meses de tiempo máximo de tolerancia se dará un mes de tiempo en una archivero temporal que se borrará cada més para tener un tiempo de rescate de un mes extra. Los permisos y autorizaciones se darán conforme se tenga registrado al usuario en el ITAM, ya sea como estudiante, administrativo, o empleado docente o de TI, cada uno de estos perfiles de usuarios tendrán distintos permisos, por ejemplo el administrador del sistema será el único que tendrá permiso de ver los mensajes reportados, y sancionar al perfil involucrado. Todas las estadísticas de uso serán recolectadas a través de logs, se contarán los mensajes enviados, los tiempos de respuesta a los mensajes, los tiempos de respuesta del servidor, estos podrán ser consultados en el sitio oficial del ITAM, donde también habrá reportes de los errores que se presenten y de las correcciones para prevenirlos.
### 5.4. Atributos de Software de Calidad

- Fiabilidad:
    Se tendrá especial cuidado en medir los incidentes cuando sabemos que hay picos de usuarios, por ejemplo a principios y final de semestres que se espera tener sobrecargas de transacciones. Además definir en los logs cuáles incidentes son los más graves para establecer la prioridad de resolverlos de acuerdo con qué tan prioritarios son y qué tan frecuentes son, también en los logs será importante reportar dónde se están presentando los incidentes para evaluar si el módulo en general debe ser revisado. Todo esto con la finalidad de reducir drásticamente los errores en los primeros meses de productivo.

- Rendimiento:
    Para obtener el rendimiento necesario de nuestra plataforma se hará una fase de pruebas en el desarrollo, está descrita más a fondo en el Plan de Calidad, los requerimientos de rendimiento están especificados en la sección 5.1 de este documento. Se realizarán pruebas de carga, de estresamiento, pruebas de ataque y pruebas unitarias por módulo y su integración con la API.

- Mantenibilidad:
    La métrica para la mantenibilidad que usaremos para este desarrollo es la de errores promedio por línea de código, ya que al hacerlo por microservicios, nos permitirá hacer estimaciones por módulo cuando se vaya a integrar otro servicio de manera informada y nos ayudará a mantener consciencia del costo en tiempo y dinero de este mantenimiento.
    
-Capacidad de entrega:
    Se mantendrán abiertos los canales de comunicación con los usuarios y la institución para generar periódicamente más historias de usuario que se puedan convertir en nuevas funcionalidades que podrán ser integradas como nuevos microservicios.

## 5.5. Reglas del negocio
La aplicación busca que todos puedan mensajear a cualquiera de los usuarios, la principal regla de negocio es que los mensajes se procesen deacuerdo a la hora en la que fueron enviados para darle sentido a las conversaciones, y que los requests de mensaje de usuarios bloqueados no sean enviadas a ningún destinatario. Una segunda regla de negocio es que cuando haya un mensaje de duda sin responder, después de 12 horas de haberse mandado se envíe a todos los profesores de asignatura para aumentar las probabilidades de respuesta, si llegaran a pasar 12 horas más sin respuesta, se enviará a todos los alumnos que hayan llevado o estén llevando la materia para aumentar aún más la probabilidad de respuesta. La bandeja de entrada de todos los perfiles tendrán los mensajes ordenados conforme vayan llegando y se enviarán alertas cuando se hayan dejado mensajes sin contestar por 18 horas. 
Las reglas de contenido serán impuestas por el reglamento de comportamiento para alumnos y empleados del ITAM. 
## Apéndice A: Glosario
## Apéndice B: Análisis
