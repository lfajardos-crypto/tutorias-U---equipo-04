
Funcionales:


Campo:     Contenido
ID:      RF-001
Nombre:     Consultar disponibilidad de horarios 
Actor:             Coordinación
Descripción:         El sistema debe permitir a la Coordinación consultar los horarios de                                 tutoría disponibles antes de confirmar una tutoría.

Resultado esperado:        Se muestran únicamente los horarios disponibles para que la                                         coordinación pueda seleccionar uno y confirmar la tutoría, sin incluir                               horarios ocupados.
Fuente:                Coordinación necesita conocer cuáles horarios están disponibles antes de                             confirmar una tutoría.
Método de verificación : Consultar los horarios disponibles y comprobar que el sistema muestra                                 únicamente quellos que no se encuentran ocupados.


ID: RF-02
Nombre: Distribución de reservas
Actor: Coordinación
Descripción: El sistema debe mostrar las tutorías disponibles en un solo lugar
Resultado esperado: Las tutorías disponibles se muestran en el sistema
Fuente: La información de las reservas se encuentra distribuida en diferentes medios
Metodo de verificacion: Agregar las tutorías disponibles y se muestran en pantalla.

ID: RF-03
Nombre: Observación del proceso
Actor: Coordinación
Descripción: El sistema debe de revisar la lista de horarios antes que confirmen las tutorías.
Resultado esperado:  Una vez se seleccione una tutoría el horario de este campo ya no debe de aparecer como disponible
Fuente:  Los estudiantes deben de ser capaces de observar que horarios siguen con disponibilidad
Método de verificación:  El horario que fue seleccionado para la tutoría ya no debe de aparecer para que lo seleccione otro estudiante.                                     




No Funcionales

ID: RNF-01
Atributo: Rendimiento
Escenario/Condición: La distribución de tutorías disponibles
Métrica: Tiempo de respuesta
Umbral/criterio	: <=5 segundos
Fuente: La información de las reservas se encuentra distribuida en diferentes medios
Metodo de verificacion: Prueba de carga

¿Cuánto tiempo considera que es el tiempo de respuesta deseable?


ID: RNF-02
Atributo: Disponibilidad
Escenario/Condición: Observar que horarios siguen con disponibilidad
Métrica: Porcentaje de tiempo operativo
Umbral/criterio	: 100%
Fuente	: Los estudiantes deben de ser capaces de observar que horarios siguen con disponibilidad
Método de verificación: Al ingresar a los horarios debe mostrar la información.

Debe de aparecer la información disponible siempre o no mostrarse durante algún periodo de tiempo?




