# Requerimiento funcional

| Campo | Información |
|---|---|
| *ID* | RF-01 |
| *Nombre* | Registro de reserva de tutoría |
| *Actor* | Estudiante |
| *Descripción* | El sistema debe permitir al estudiante consultar la lista de tutorías disponibles para registrar una tutoría. |
| *Resultado esperado* | El sistema procesa la selección del estudiante y muestra una confirmación de la tutoría programada. |
| *Fuente* | F-03. Entrevista con estudiante: «Poder ver las opciones de mi materia y saber inmediatamente si la reserva quedó confirmada». |
| *Método de verificación* | Ingresar al sistema como estudiante, seleccionar una materia, elegir un horario disponible y completar la reserva; verificar que la sesión quede registrada. |

# Caso de uso

| Campo | Información |
|---|---|
| *ID* | CU-001 |
| *Nombre* | Reservar tutoría |
| *RF relacionado* | RF-01 |
| *Actor principal* | Estudiante |
| *Objetivo* | Reservar un espacio de tutoría disponible para una materia seleccionada. |
| *Precondiciones* | 1. El estudiante ha iniciado sesión en el sistema.<br>2. Existen materias y horarios de tutoría registrados en la plataforma. |
| *Flujo principal* | 1. El estudiante selecciona *Reservar tutoría*.<br>2. El sistema muestra la lista de materias.<br>3. El estudiante selecciona una materia.<br>4. El sistema muestra los horarios de la materia seleccionada.<br>5. El estudiante selecciona un horario.<br>6. El estudiante confirma la reserva.<br>7. El sistema registra la reserva, actualiza el horario como no disponible y muestra el mensaje de confirmación de la tutoría reservada. |
| *Flujo alternativo* | *Cambiar la selección de materia antes de confirmar:*<br><br>1. En el paso 3 del flujo principal, el estudiante decide seleccionar una materia diferente antes de continuar.<br>2. El estudiante selecciona la nueva materia de la lista.<br>3. El sistema muestra los horarios de la nueva materia seleccionada.<br>4. El estudiante selecciona un horario.<br>5. El estudiante confirma la reserva.<br>6. El sistema registra la reserva, actualiza el horario como no disponible y muestra el mensaje de confirmación de la tutoría reservada. |
| *Excepciones* | *E1. Espacio ya ocupado:<br>1. En el paso 7 del flujo principal, el sistema detecta que el horario fue reservado por otro estudiante.<br>2. El sistema muestra el mensaje de error: «El horario seleccionado ya no se encuentra disponible».<br>3. El sistema regresa al paso 4 del flujo principal.<br><br>E2. Límite de dos reservas:*<br>1. En el paso 1 del flujo principal, el sistema verifica si el estudiante ya tiene dos reservas activas.<br>2. El sistema muestra el mensaje de error: «Ha alcanzado el límite de dos tutorías reservadas activas».<br>3. El sistema no muestra la lista de materias. |
| *Postcondiciones* | *Éxito:* La tutoría queda confirmada, el horario pasa a estar reservado y se notifica al estudiante.<br><br>*Fallo:* El sistema no crea la reserva. El horario permanece disponible cuando el estudiante alcanza el límite de reservas; si otro estudiante ocupó el horario, este se mantiene como no disponible. |
