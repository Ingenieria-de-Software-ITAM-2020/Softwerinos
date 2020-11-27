# Test Plan (IEEE format)

## TEST PLAN OUTLINE (IEEE 829 FORMAT) 

1) Test Plan Identifier 
1) References 
1) Introduction 
1) Test Items 
1) Software Risk Issues 
1) Features to be Tested 
1) Features not to be Tested 
1) Approach  
1) Item Pass/Fail Criteria 
1) Suspension Criteria and Resumption Requirements 
1) Test Deliverables 
1) Remaining Test Tasks 
1) Environmental Needs 
1) Staffing and Training Needs 
1) Responsibilities 
1) Schedule 
1) Planning Risks and Contingencies 
1) Approvals 
1) Glossary


## 1. IDENTIFICADOR DEL PLAN
MasterTestPlan-X Æ A-12

## 2. REFERENCIAS
Este plan de calidad está respaldado por el siguiente documento: [SRS](./Especificacion_De_Requerimientos_del_Sistema.md)

## 3. INTRODUCCIÓN
A continuación se encuentra el plan de calidad del proyecto **BLATT ITAM**. 
El objetivo de este documento es determinar un plan detallado que cuente con todas las pruebas de calidad que se harán para asegurarse que el software cumple con todas las funcionalidades requeridas para un sistema de comunicación entre los miembros de la comunidad ITAM. Adicionalmente, se harán pruebas para asegurarse que el software puede considerarse *seguro* y funciona de una manera *amigable*.



## 4. MÓDULOS A PROBAR
Aquí se encuentra una lista de los diferentes tipos de pruebas que se harán para la **Versión 0**:
1. Login
2. Interacción de mensajes
3. Crear un nuevo chat/grupos
4. Búsqueda
5. Reportar mensajes
6. Reenvio de mensajes de dudas
7. Agendar citas

## 5. RIESGO DE PROBLEMAS CON EL SOFTWARE 
Se han identificado los siguientes riesgos:
1. Seguridad
2. Problemas con la interfaz

## 6. FUNCIONALIDADES A PROBAR
- REQ-1.1: Por cada mensaje no leído de alguna conversación el sistema enviará una notificación al receptor del mensaje.
- REQ-1.3: Que todos los mensajes enviados estén cifrados de extremo a extremo.
- REQ-1.4: Que el sistema permita enviar el mismo mensaje a varios usuarios.
- REQ-2.1: Poder crear un grupo para mandar el mensaje seleccionando dos o más usuarios como destinatarios.
- REQ-2.2: Si se decide crear una conversación con alguien con quien ya se tiene un chat, solo se abrirá el chat que ya existía. 
- REQ-2.4: Poder crear un chat con los tres distintos usuarios (estudiante, docente, personal administtrativo).
- REQ-3.1: Poder reportar multiples mensajes dentro de un mismo chat.
- REQ-3.2: Poder seleccionar múltiples razones por la cual se realiza el reporte.
- REQ-3.3: Que el sistema permita reportar indistintamente del tipo de usuario (estudiantes, docentes, personal administrativo).
- REQ-3.4: Que el sistema permita escribir sobre una caja de texto otra razón por la cual se realizó el reporte, en el caso de que la lista de razones más comúnes no sea suficiente. 
- REQ-4.1: Reenviar un mensaje a los profesores después de 12 horas
- REQ-4.2: Reenviar un mensaje a los alumnos de la materia después de 24 horas
- REQ-4.3: Que el sistema solamente reenvie las dudas que no han sido contestadas, evitando mensajes de otra indole. 
- REQ-4.4: Que el sistema reenvie el mensaje asignando un nombre anonimo como autor del mensaje. Este nombre anonimo tendrá como propositó evitar alguna molestia o inconveniente que el estudiante pueda tener, en caso de que su mensaje sea reenviado a otras personas que no sean el destinatario original.
- REQ-5.1: Que el sistema permita agendar una cita con cualquier tipo de usuario(estudiantes, profesores, personal administrativo)
- REQ-5.2: Que el sistema permita que se puedan realizar multiples citas, incluso cuando ya se tienen otras citas agendadas.



## 7. FUNCIONALIDADES QUE NO SE DEBEN DE PROBAR
- REQ-1.2: Que el número de conversaciones abiertas sólo esté limitado por la memoria del dispositivo.
- REQ-2.3: Poder tener el número de chats que la memoria del dispositivo permita.
- REQ-2.5: Poder crear un chat con un usuario con el cual se tenía un chat pero se había borrado.
- REQ-3.5: Que el sistema permita cerrar la ventana de reporte, en el caso que no se requiera hacer el reporte y se haya seleccionado la opción por accidente. 
- REQ-3.6: Que el sistema permita realizar un reporte sobre un mensaje de cualquier tipo. Es decir, que el sistema permita reportar videos, imagenes, archivos y mensajes de texto. 

## 8. ESTRATEGIA 
Aunque sabemos que se debería de tener diferentes persoans para realizar las diferentes pruebas, por falta de personal, se harán las pruebas por diferentes miembros del equipo una vez que se termine cada módulo. 
Los diferentes tipos de pruebas que se harán son: 
1. Pruebas unitarias
2. Pruebas bajo estrés
3. Pruebas bajo ataque
4. Pruebas de carga

## 9. CRITERIO PARA CONSIDERAR QUE UN ELEMENTO FUNCIONA
Se considerará que el Software estará listo una vez que haya cumplido con un periodo de pruebas de 90 días sin tener fallas. (ver sección 16 para el plan general)

## 10. SUSPENSION CRITERIA AND RESUMPTION REQUIREMENTS
Se deberá para en caso de que:
1) Los mensajes no se estén enviando (por parte del usuario 1) y llegando (al usuario 2) en el orden correcto.
2) Los mensajes no estén llegando
3) Los mensajes estén llegando a un usuario incorrecto    
Para atender los "issues" se está manejando una política de "min flow time," por lo que se optimizarán los recursos para trabajar con los "issues"
de tal forma que se atenderán dependiendo de la prioridad y el tiempo que requiera utilizarlos.

## 11. ENTREGABLES
1) Plan de aceptación o rechazp
2) Reporte de resultados de las pruebas unitarias.
3) Reporte de los mock-ups
4) Reporte de incidentes

## 12. REMAINING TEST TASKS
Se está considerando que las funcionalidades y requerimientos que tengan prioridad baja se lanzarán después del lanzamiento general. 
Es decir, primero se terminará el software con las funcionalidades que han sido clasificadas con prioridad **alta** y **media** se realizarán primero y las funcionalidades de prioridad **baja** se dejarán pendientes. 

## 13. ENVIRONMENTAL NEEDS


## 14. STAFFING AND TRAINING NEEDS


## 15. RESPONSABILIDADES
Cada miembro del equipo tiene diferentes responsabilidades, sin embargo, es importante que para aprobar o rechazar cualquier cosa se sigan las medidas adecuadas. 

Se va a dividir al equipo de trabajo en pares y de esta forma se podrá tener mejor control. Las parejas son: Andrea de Anda Kuri/Miguel Ángel Cifuentes Jiménez y  Damian Pérez Landeros/Isaías Jesús García Moreno

La estructura de la división de tareas es la siguiente: 
|                                      | Pareja 1 | Pareja 2 |
|--------------------------------------|----------|----------|
| Probar la usabilidad                 |     x    |          |
| Revisar que se pueda enviar mensajes |          |     x    |
| Reportar mensajes                    |     x    |          |
| Crear grupos                         |          |     x    |
| Búsquedas                            |     x    |          |
| Enviar un mensaje a muchas personas  |          |     x    |
|                                      |          |          |


## 16. PLAN DE TRABAJO
Para las pruebas de calidad se utilizará una metodología Scrum con sprints de duración predefinida a una semana. 
Se considera que cada módulo se podrá realizar en un módulo de la siguiente forma:
| Sprint | Módulo a revisar  |
|---|---|
| 1  |  Login |
| 2  | Interacción de mensajes  |
| 3  | Crear un nuevo chat/grupos  |
| 4  | Búsqueda  |
| 5  |  Reportar mensajes |
| 6  |  Reenvio de mensajes de dudas |
| 7  |  Agendar citas | 


En cada sprint seguirá la estrategia general que incluye:
1. Pruebas unitarias
2. Pruebas bajo estrés
3. Pruebas bajo ataque 
4. Pruebas de carga


Además se tiene el siguiente plan:
| Semanas | Acciones                                      |
|---------|-----------------------------------------------|
| 1-7     | Pruebas de calidad por parte del equipo       |
| 8       | Lanzamiento a producción                      |
| 9-12    | Lanzamiento preeliminar para detectar errores |
| 13      | Lanzamiento general                           |


Se está estimando que el lanzamiento general sucederá en caso de que se pasen todas las pruebas previstas. 

## 17. RIESGO DE PLANEACIÓN Y EN CASO DE CONTINGENCIA
Para este proyecto se está considerando que el equipo esta formado por cuatro desarrolladores junior, es decir, hay que tomar en cuenta que
las fechas pueden variar entre la estimación y las fechas reales. Además, la pandemia actual llegó con diferentes retos para todos, por lo que se entenderá que se cambien las fechas de los sprints. Pero, esto no implica que se podrá lanzar el software sin hacer las debidas pruebas, en caso de que haya problemas se 
tendrán que modificar las fechas de entrega, el alcance o el costo. 

## 18. APROBACIÓN
Lider del Proyecto - Andrea de Anda Kuri        
Test Manager - Miguel Ángel Cifuentes Jiménez         
Architecture manager - Damian Pérez Landeros          
Representante del equipo - Isaías Jesús García Moreno

## 19. GLOSARIO
| Palabra | Definición |
|---------|------------|
|Administrativo|Personal que trabaja en el ITAM, puede ser en becar, caja, biblioteca, etc.|
|    BLATT     |  Nombre del proyecto del equipo Softwerinos     |
|    Softwerinos     |    Equipo de la materia de Ingenieria de Software del ITAM      |
|      ITAM   |        Instituto Tecnológico Autónomo de México    |



