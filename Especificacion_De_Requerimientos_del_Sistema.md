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
![Interfaz de Hardware](https://github.com/Ingenieria-de-Software-ITAM-2020/Softwerinos/blob/main/imagenes/interfaz_hardware.PNG)
### 3.3. Interfaces de software    
### 3.4. Interfaces de comunicación
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
## 4.2. Crear chats
#### 4.2.1. Descripción y prioridad 
Poder crear un chat con algún miembro de la organización a quien se desee enviar un mensaje personal, tendrá prioridad alta con valor 1 ya que es parte de las funcionalidades básicas del aplicativo.
#### 4.2.2. Secuencias Estímulo/Respuesta
Habrá un botón de crear conversación donde puedas elegir a qué persona de la institución quieres mandar el mensaje, una vez seleccionados los destinatarios, se abrirá una nueva ventana de conversación con ese miembro del ITAM.
#### 4.2.3. Requerimientos funcionales
- REQ-2.1: Poder crear un grupo para mandar el mensaje seleccionando 2 o más usuarios como destinatarios.
- REQ-2.2: Si se decide crear una conversación con alguien con quien ya se tiene un chat, solo se abrirá el chat que ya existía. 
- REQ-2.3: 
## 4.3. Reportar un mensaje
#### 4.3.1. Descripción y prioridad 
#### 4.3.2. Secuencias Estímulo/Respuesta
#### 4.3.3. Requerimientos funcionales
- REQ-3.1: 
- REQ-3.2: 
- REQ-3.3: 
## 4.4. Reenvio temporizado de mensajes de duda
#### 4.4.1. Descripción y prioridad 
#### 4.4.2. Secuencias Estímulo/Respuesta
#### 4.4.3. Requerimientos funcionales
- REQ-3.1: Reenviar un mensaje a los profesores después de 12 horas
- REQ-3.2: Reenviar un mensaje a los alumnos de la materia después de 24 horas
- REQ-3.3: 
## 4.5. Agendar citas
#### 4.5.1. Descripción y prioridad 
#### 4.5.2. Secuencias Estímulo/Respuesta
#### 4.5.3. Requerimientos funcionales
- REQ-3.1: 
- REQ-3.2: 
- REQ-3.3: 
## 5. Otros Requerimientos No Funcionales
### 5.1. Requerimientos operacionales
### 5.2. Requerimientos de protección
### 5.3. Requerimientos de seguridad
### 5.4. Atributos de Software de Calidad

- Exactitud 
- Fiabilidad 
- Adecuación 
- Capacidad de Aprendizaje
- Robustez 
- Mantenibilidad
- Legibilidad
- Extensibilidad
- Facilidad de Prueba
- Eficiencia 
- Portabilidad

## 5.5. Reglas del negocio

## Apéndice A: Glosario
## Apéndice B: Análisis
