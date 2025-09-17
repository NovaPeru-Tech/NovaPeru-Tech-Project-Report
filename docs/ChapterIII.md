<h2 id="requirementsSpecification">Capítulo III: Requirements Specification</h2>
<h3 id="userStories">3.1. User Stories</h3>
| EPIC ID | Título | Descripción |
<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr>
    <td>EP01</td><td>Navegación en la Landing Page</td><td>Como visitante quiero tener una experiencia fluida y completa en el sitio web para conocer los servicios y tomar decisiones informadas. </td>
  </tr>
  <tr>
    <td>EP02</td><td>Soporte y contacto</td><td>Como visitante de la Landing Page, quiero poder contactar a Veyra fácilmente, para resolver dudas o interactuar.</td>
  </tr>
  <tr>
    <td>EP03</td><td>Acceso a Información </td><td>Como familiar  del adulto mayor  quiero poder tener acceso a toda la información de mi familiar para estar informado de su estado.</td>
  </tr>
   <tr>
    <td>EP04</td><td>Gestión de adultos mayores</td><td>
    Como administrador de casa de reposo quiero gestionar perfiles de los adultos mayores para tener un mayor control.
    </td>
  </tr>
   <tr>
    <td>EP05</td><td>Notificaciones automáticas</td><td>Como familiar de un adulto mayor, quiero recibir notificaciones automáticas sobre cambios en su estado o recordatorios importantes , para estar siempre informado sin tener que consultar manualmente la plataforma.</td>
  </tr>
   <tr>
    <td>EP06</td><td>Comunicación con cuidadores</td><td>Como familiar, quiero disponer de un canal de comunicación directo con los cuidadores o el personal de la casa de reposo , para hacer preguntas y recibir respuestas rápidas sobre el cuidado de mi adulto mayor</td>
  </tr>
   <tr>
    <td>EP07</td><td>Gestión de medicamentos</td><td>Como administrador quiero gestionar los medicamentos de la casa de reposo para garantizar que cumplan con todos los controles necesarios.</td>
  </tr>
   <tr>
    <td>EP08</td><td>Gestión de personal</td><td>Como administrador de la casa de reposo, quiero gestionar la información del personal para organizar los turnos de trabajo de los cuidadores y garantizar que siempre haya atención adecuada disponible para los residentes.</td>
  </tr>
   <tr>
    <td>EP09</td><td>Gestión de información de la casa de reposo</td><td>Como administrador quiero gestionar la información general de la casa de reposo para mantener datos actualizados sobre la institución.</td>
  </tr>
   <tr>
    <td>EP10</td><td>Seguridad y privacidad</td><td>Como administrador, quiero garantizar la seguridad y privacidad de los datos personales y médicos para proteger la información sensible de los residentes y familiares, cumpliendo con las normativas correspondientes.</td>
  </tr>
  <tr>
    <td>EP11</td><td>  Diseño de interfaz</td><td>Como usuario, quiero una interfaz bien diseñada para navegar y usar el sistema sin dificultades</td>
  </tr>
</table>

<h3 id="UserStories">User Stories</h3>
<table border="1" style="border-collapse: collapse; width: 100%;font-size: 1px; font-family: Arial, sans-serif;"">
  <tr>
    <td>ID</td><td>Titulo</td><td>Descripción</td><td>Criterios de acceptación</td><td>Epic ID</td>
  </tr>
  <tr>
    <td>US01</td><td>Menú de navegación</td><td>Como visitante de la Landing Page, quiero poder acceder a un menú de navegación en la parte superior de la página, para  explorar fácilmente las  secciones como "Log in", "Sign up", "Planes",  "Contacto",etc.</td><td>
   <strong>Scenario 1 : Menú visible y navegable</strong> <br>
Given un visitante en la landing page
When la página carga por completo y el visitante hace clic (o toca) un enlace del menú
Then el menú está visible en la parte superior con los enlaces principales ("Log in", "Sign up", "Planes", "Contacto") y el visitante es redirigido a la sección correspondiente sin errores. <br> <br>

<strong>Scenario 2 : Menú no carga o enlace roto</strong> <br>
Given un visitante en la landing page
When el menú no se renderiza por fallo de recursos  o al hacer clic en un enlace la ruta devuelve error/404
Then se muestra un mensaje amigable  y el visitante puede acceder a las secciones esenciales mediante enlaces alternativos  sin bloquear la exploración. </td><td>EP01</td>
  </tr>
  <tr>
    <td>US02</td><td>Visualización de Planes </td><td>Como visitante de la Landing Page, quiero ver los planes de suscripción junto a su precio y características, para poder elegir el que mejor se adapte a mis necesidades.</td><td>
    Scenario 1: Visualización correcta de planes
Given un visitante en la sección de planes de la landing page
When la página carga completamente
Then debe ver al menos 2 planes de suscripción diferentes
And cada plan debe mostrar claramente: precio, características principales, duración y botón de selección
And debe poder comparar fácilmente las diferencias entre planes
And todos los elementos deben ser legibles y estar correctamente alineados
Scenario 2: Error en carga de planes
Given un visitante en la sección de planes
When ocurre un error en la carga de información de planes
Then se muestra un mensaje de error amigable
And se proporciona una opción para recargar la información
And el visitante puede acceder a información de contacto como alternativa
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US03</td><td>Selección de Plan en Landing Page</td><td>Como visitante de la landing Page, quiero seleccionar un plan y finalizar la confirmación en la misma pantalla, para agilizar y simplificar el registro.</td><td>
    Scenario 1: Selección y confirmación exitosa
    Given un visitante visualizando los planes disponibles
When selecciona un plan específico y hace clic en "Seleccionar"
Then es dirigido a un formulario de confirmación en la misma pantalla
And el formulario muestra el plan seleccionado con su precio
And puede completar sus datos y confirmar la selección
And recibe una confirmación inmediata del proceso
Scenario 2: Selección sin completar datos requeridos
Given un visitante en el formulario de confirmación de plan
When intenta confirmar sin completar campos obligatorios
Then se muestran mensajes de validación específicos para cada campo faltante
And el formulario mantiene la información ya ingresada
And puede corregir y reenviar sin perder progreso
</td><td>EP01</td>
  </tr>
    <tr>
    <td>US04</td><td>Visualización de creadores</td><td>Como visitante de la Landing Page, quiero ver a los creadores de la aplicación, para conocer al equipo detrás del producto y generar confianza en el servicio.</td><td>
    Scenario 1: Acceso exitoso a información del equipo
Given un visitante en la landing page
When navega a la sección "Sobre nosotros" o "Equipo"
Then puede ver información de cada creador incluyendo: nombre, foto, rol y breve descripción
And la información se presenta de manera profesional y organizada
And puede acceder a perfiles profesionales o redes sociales si están disponibles
Scenario 2: Información de equipo no disponible
Given un visitante intentando acceder a información del equipo
When la sección no carga correctamente
Then se muestra un mensaje explicativo
And se proporciona información de contacto alternativa
And el visitante puede continuar navegando otras secciones sin problemas
    </td><td>EP01</td>
  </tr>
    <tr>
    <td>US05</td><td>Redes sociales</td><td>Como visitante del landing page quiero poder acceder fácilmente a sus redes sociales de Veyra para conocer más sobre la empresa y tener canales adicionales de contacto </td><td>
    Scenario 1: Acceso exitoso a redes sociales
Given un visitante en cualquier página de la landing page
When busca enlaces a redes sociales en el footer o header
Then encuentra íconos claramente identificables de las principales redes sociales
And al hacer clic, se abren en nueva pestaña las páginas oficiales de Veyra
And los enlaces funcionan correctamente y dirigen al contenido apropiado
Scenario 2: Enlaces de redes sociales no funcionales
Given un visitante intentando acceder a redes sociales
When hace clic en un ícono de red social que no funciona
Then recibe un mensaje de error informativo
And se proporciona información de contacto alternativa
And puede continuar su navegación sin interrupciones
</td><td>EP02</td>
  </tr>
    <tr>
    <td>US06</td><td>Formulario de contacto</td><td>Como visitante del landing page quiero completar un formulario de contacto para enviar consultas específicas y recibir una respuesta personalizada de Veyra</td><td>
    Scenario 1: Envío exitoso de consulta
    Given un visitante en el formulario de contacto
When completa todos los campos requeridos (nombre, email, asunto, mensaje)
And hace clic en "Enviar"
Then recibe una confirmación de que su mensaje fue enviado
And se le informa el tiempo estimado de respuesta
And recibe una copia de confirmación en su email
Scenario 2: Formulario con datos inválidos
Given un visitante completando el formulario de contacto
When ingresa un email inválido o deja campos obligatorios vacíos
And intenta enviar el formulario
Then se muestran mensajes de validación específicos
And se mantiene la información correcta ya ingresada
And puede corregir errores y reenviar
</td><td>EP02</td>
  </tr>
    <tr>
    <td>US07</td><td>Cambio de idioma</td><td>Como visitante del Landing Page quiero en el menú un botón para cambiar de idioma entre español e inglés para  entender mejor de que trata Veyra</td><td>
    Scenario 1: Cambio exitoso de idioma
Given un visitante en la landing page en español
When hace clic en el botón de cambio de idioma y selecciona inglés
Then toda la interfaz cambia al idioma seleccionado
And el contenido se mantiene equivalente en significado
And la preferencia de idioma se mantiene al navegar entre páginas
Scenario 2: Idioma no disponible temporalmente
Given un visitante intentando cambiar de idioma
When el servicio de traducción no está disponible
Then se muestra un mensaje informativo sobre la situación
And se mantiene el idioma actual funcionando
And se proporciona información en el idioma disponible
</td><td>EP01</td>
  </tr>
    <tr>
    <td>US08</td><td>Historial médico </td><td>Como familiar de un adulto mayor quiero acceder al historial médico completo de mi familiar para conocer su evolución de salud y diagnósticos actuales</td><td>Scenario 1: Acceso exitoso al historial médico
    Given un familiar autenticado en el sistema
When navega a la sección "Historial Médico" de su familiar
Then puede ver diagnósticos actuales, evolución de salud y últimas actualizaciones
And la información está organizada cronológicamente
And puede filtrar por fechas o tipos de reportes
And toda la información es legible y está actualizada
Scenario 2: Sin permisos para acceder a reportes
Given un usuario intentando acceder a historial médico
When no tiene los permisos necesarios
Then se muestra un mensaje claro sobre restricciones de acceso
And se proporciona información sobre cómo obtener permisos
And puede contactar al administrador para resolver el acceso
</td><td>EP03</td>
  </tr>
    <tr>
    <td>US09</td><td>Agenda de citas Medicas</td><td>Como familiar de un adulto mayor quiero consultar la agenda de citas médicas de mi familiar para estar informado sobre sus próximos tratamientos</td><td>
    Scenario 1: Visualización exitosa de citas programadas
Given un familiar autenticado en el sistema
When accede a la agenda de citas de su familiar
Then puede ver todas las citas programadas con fecha, hora, médico y tipo de consulta
And puede filtrar por rangos de fechas
And recibe indicaciones claras sobre próximas citas importantes
And puede exportar o imprimir la agenda si es necesario
Scenario 2: No hay citas programadas
Given un familiar consultando la agenda de citas
When no hay citas programadas para su familiar
Then se muestra un mensaje informativo indicando que no hay citas
And se proporciona información sobre cómo programar nuevas citas
And puede contactar al personal médico si es necesario
</td><td>EP03</td>
  </tr>
    <tr>
    <td>US10</td><td>Consulta de información personal</td><td>Como familiar de un adulto mayor quiero ver la información de mi familiar para estar seguro de que esté correcto o actualizado.</td><td>
    Scenario 1: Visualización exitosa de información personal
Given un familiar autenticado en el sistema
When accede al perfil de información personal de su familiar
Then puede ver datos personales actualizados: nombre, edad, contacto de emergencia, alergias, medicamentos actuales
And puede identificar fácilmente si algún dato requiere actualización
And tiene acceso a opciones para solicitar modificaciones
Scenario 2: Información desactualizada detectada
Given un familiar revisando información personal
When identifica información que necesita actualización
Then puede marcar campos como "requiere actualización"
And puede enviar solicitudes de cambio con justificación
And recibe confirmación de que la solicitud fue recibida
    </td><td>EP03</td>
  </tr>
   <tr>
    <td>US11</td><td>Galería de fotos y actividades</td><td>Como familiar de un adulto mayor quiero ver fotos de las actividades diarias de mi familiar para sentirme conectado con su día a día y verificar su participación social</td><td>
    Scenario 1: Acceso exitoso a galería de actividades
Given un familiar autenticado en el sistema
When accede a la galería de fotos de su familiar
Then puede ver fotos organizadas por fecha y tipo de actividad
And cada foto incluye descripción de la actividad realizada
And puede filtrar por fechas o tipos de actividades
And las fotos se cargan correctamente y son de buena calidad
Scenario 2: Sin actividades recientes registradas
Given un familiar consultando la galería
When no hay fotos recientes de actividades
Then se muestra un mensaje informativo sobre la situación
And se proporciona información sobre la frecuencia de actualización de fotos
And puede contactar al personal para consultas específicas
</td><td>EP03</td>
  </tr>
   <tr>
    <td>US12</td><td>Registro de residentes</td><td>Como administrador de casa de reposo quiero crear y mantener perfiles completos de cada residente para centralizar toda su información personal y médica</td><td>
    Scenario 1: Creación exitosa de perfil de residente
Given un administrador autenticado en el sistema
When accede al formulario de registro de nuevo residente
And completa toda la información requerida (datos personales, médicos, contactos de emergencia)
Then el perfil se crea exitosamente
And se genera un ID único para el residente
And toda la información queda almacenada y accesible para consultas futuras
Scenario 2: Error en datos requeridos para registro
Given un administrador creando perfil de residente
When falta información crítica requerida
And intenta guardar el perfil incompleto
Then se muestran mensajes específicos de campos faltantes
And se mantiene la información ya ingresada
And puede completar los datos faltantes y continuar
    </td><td>EP04</td>
  </tr>
   <tr>
    <td>US13</td><td>Historial médico institucional</td><td>Como administrador quiero gestionar el historial médico completo de cada residente para asegurar continuidad en el cuidado y cumplir con regulaciones sanitarias
    </td><td>
    Scenario 1: Gestión exitosa de historial médico completo
    Given un administrador con permisos médicos
When accede al historial médico de un residente
Then puede ver, agregar y actualizar información médica completa
And puede registrar nuevos diagnósticos, tratamientos y evoluciones
And toda la información queda registrada con fecha, hora y responsable
And puede generar reportes médicos para autoridades sanitarias
Scenario 2: Acceso sin permisos médicos suficientes
Given un usuario intentando acceder a historial médico institucional
When no posee los permisos necesarios
Then se restringe el acceso con mensaje explicativo
And se proporciona información sobre cómo obtener permisos apropiados
And puede acceder solo a información no confidencial si corresponde
</td><td>EP04</td>
  </tr>
   <tr>
    <td>US14</td><td>Administración de medicamentos</td><td>Como administrador quiero controlar la administración de medicamentos de todos los residentes para garantizar cumplimiento de tratamientos y evitar errores médicos</td><td>
    Scenario 1: Control exitoso de administración de medicamentos
Given un administrador en el módulo de medicamentos
When registra la administración de medicamentos a residentes
Then puede marcar medicamentos como administrados con hora exacta
And puede registrar observaciones sobre efectos o reacciones
And el sistema alerta sobre próximas dosis programadas
And mantiene historial completo de administración por residente
Scenario 2: Medicamento no disponible en inventario
Given un administrador intentando registrar administración de medicamento
When el medicamento no está disponible en inventario
Then el sistema muestra alerta de falta de stock
And proporciona opciones para contactar a farmacia o proveedor
And permite registrar la situación para seguimiento
    </td><td>EP04</td>
  </tr>
   <tr>
    <td>US15</td><td>Gestión de visitas familiares</td><td>Como administrador quiero controlar y programar las visitas familiares a los residentes para mantener seguridad, orden y cumplir con los horarios establecidos</td><td>
    Scenario 1: Programación exitosa de visita familiar
Given un administrador en el módulo de visitas
When programa una nueva visita familiar
Then puede asignar fecha, hora, visitantes y residente a visitar
And el sistema verifica disponibilidad de horarios
And genera confirmación para la familia y actualiza agenda institucional
And envía recordatorios automáticos antes de la visita
Scenario 2: Conflicto de horarios en visitas
Given un administrador programando visita familiar
When el horario solicitado ya está ocupado
Then el sistema muestra horarios alternativos disponibles
And permite reprogramar o sugerir opciones similares
And notifica a la familia sobre el cambio de horario
</td><td>EP04</td>
  </tr>
   <tr>
    <td>US16</td><td>Recordatorios de citas y consultas</td><td> Como familiar quiero recibir recordatorios automáticos sobre citas médicas y consultas programadas de mi familiar para estar preparado y decidir si deseo acompañarlo</td><td>
    Scenario 1: Envío exitoso de recordatorios automáticos
Given el sistema con citas médicas programadas
When se acerca una cita médica (24 horas antes)
Then se envía recordatorio automático a familiares vía email/SMS
And el recordatorio incluye fecha, hora, médico y tipo de consulta
And los familiares pueden confirmar asistencia o reagendar
And el sistema registra la confirmación recibida
Scenario 2: Falla en envío de recordatorios
Given el sistema intentando enviar recordatorios
When falla el servicio de notificaciones
Then se registra el error en logs del sistema
And se intenta reenvío automático después de un tiempo
And se notifica al administrador sobre fallas en el sistema
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US17</td><td>Notificaciones de cambios en medicación</td><td>Como familiar quiero ser notificado inmediatamente sobre cualquier cambio en la medicación de mi familiar para estar informado sobre su tratamiento médico</td><td>
    Scenario 1: Notificación inmediata de cambio en medicación
Given un cambio en la medicación de un residente
When el médico actualiza el tratamiento farmacológico
Then se envía notificación inmediata a familiares autorizados
And la notificación incluye detalles del cambio y justificación médica
And los familiares pueden contactar al médico para consultas
And el cambio queda registrado en el historial médico
Scenario 2: Familiar no autorizado para recibir información médica
Given un cambio en medicación de residente
When un familiar no está autorizado para recibir información médica
Then no recibe notificación de cambios en medicación
And se respetan las preferencias de privacidad del residente
And solo familiares autorizados reciben las notificaciones
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US18</td><td>Recordatorios de visitas familiares</td><td>Como familiar quiero recibir recordatorios automáticos sobre mis visitas programadas al adulto mayor para no olvidar las citas y mantener regularidad en el contacto</td><td>
    Scenario 1: Recordatorio exitoso de visita programada
Given una visita familiar programada
When faltan 2 horas para la visita
Then se envía recordatorio automático al familiar
And el recordatorio incluye fecha, hora, nombre del residente y instrucciones de acceso
And el familiar puede confirmar asistencia o cancelar con anticipación
And el sistema actualiza el estado de la visita según la respuesta
Scenario 2: Cancelación de visita por emergencia
Given una visita familiar programada
When ocurre una emergencia que requiere cancelar la visita
Then se envía notificación inmediata de cancelación
And se proporciona explicación de la situación
And se ofrecen alternativas de reprogramación
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US19</td><td>Alertas de actualización de datos personales</td><td>Como familiar quiero recibir notificaciones automáticas cuando se actualice la información personal o de mi familiar para mantenerme informado de cualquier cambio en su perfil</td><td>
    Scenario 1: Notificación exitosa de actualización de datos
Given una actualización en datos personales del residente
When se modifica información como contacto de emergencia, estado de salud, o preferencias
Then se envía notificación automática a familiares autorizados
And la notificación especifica qué información fue actualizada
And incluye fecha y responsable de la actualización
And los familiares pueden revisar los cambios en el sistema
Scenario 2: Actualización sin autorización para notificar
Given una actualización en datos personales
When el familiar no tiene autorización para recibir cierto tipo de información
Then no recibe notificación sobre datos restringidos
And solo recibe información sobre cambios que está autorizado a conocer
And se respetan las políticas de privacidad establecidas
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US20</td><td>Preguntas sobre rutina de cuidados</td><td>Como familiar quiero hacer preguntas específicas sobre la rutina diaria y cuidados de mi familiar para entender mejor su día a día y resolver dudas puntuales</td><td>
    Scenario 1: Envío exitoso de pregunta sobre cuidados
Given un familiar autenticado en el sistema de comunicación
When redacta una pregunta específica sobre la rutina de cuidados de su familiar
Then puede enviar la consulta al personal de cuidadores asignado
And recibe confirmación de que la pregunta fue enviada
And el sistema establece un tiempo estimado de respuesta
And puede hacer seguimiento del estado de su consulta
Scenario 2: Canal de comunicación no disponible
Given un familiar intentando enviar pregunta sobre cuidados
When el sistema de comunicación no está disponible
Then se muestra mensaje sobre la situación temporal
And se proporcionan números de teléfono alternativos para emergencias
And se permite guardar la pregunta para envío posterior
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US21</td><td>Peticiones de modificación de cuidados</td><td>Como familiar quiero solicitar ajustes específicos en el cuidado de mi familiar basados en sus preferencias o necesidades particulares</td><td>
    Scenario 1: Solicitud exitosa de modificación de cuidados
Given un familiar con permisos para solicitar cambios
When envía una petición detallada de modificación en cuidados específicos
Then la solicitud se registra en el sistema con número de seguimiento
And se notifica al coordinador de cuidados correspondiente
And recibe confirmación con plazos estimados de evaluación
And puede hacer seguimiento del estado de su petición
Scenario 2: Solicitud que requiere aprobación médica
Given un familiar solicitando modificación que requiere aprobación médica
When la petición involucra aspectos médicos o terapéuticos
Then se deriva automáticamente al equipo médico
And se informa al familiar sobre el proceso de evaluación médica
And se establecen plazos específicos para respuesta médica
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US22</td><td>Seguimiento del bienestar emocional</td><td>Como familiar quiero comunicarme con el personal sobre el estado emocional y psicológico de mi familiar para asegurar su bienestar integral</td><td>
    Scenario 1: Comunicación exitosa sobre estado emocional
Given un familiar preocupado por el bienestar emocional de su familiar
When envía consulta sobre estado anímico, interacción social o adaptación
Then puede comunicarse directamente con el equipo de psicología/trabajo social
And recibe respuesta profesional sobre la situación emocional del residente
And se le proporcionan recomendaciones para apoyo emocional
And puede programar reuniones de seguimiento si es necesario
Scenario 2: Situación emocional que requiere atención inmediata
Given un familiar reportando cambios emocionales significativos
When la situación indica posible crisis emocional o depresión
Then se escalona automáticamente a atención psicológica prioritaria
And se notifica al equipo médico y de trabajo social
And se contacta al familiar para coordinar intervención
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US23</td><td>Planificación de eventos familiares</td><td>Como familiar quiero coordinar con el personal la organización de eventos especiales o celebraciones para mi familiar dentro de las instalaciones</td><td>
    Scenario 1: Coordinación exitosa de evento familiar
Given un familiar planificando evento especial para su familiar
When solicita coordinación para celebración de cumpleaños, aniversario u ocasión especial
Then puede especificar fecha, número de invitados, requerimientos especiales
And el personal evalúa viabilidad según protocolos institucionales
And se coordinan espacios, horarios y recursos necesarios
And recibe confirmación con detalles finales del evento
Scenario 2: Evento que no cumple con protocolos institucionales
Given un familiar solicitando evento que no cumple protocolos
When la solicitud involucra aspectos no permitidos por políticas institucionales
Then se explican las limitaciones y razones institucionales
And se ofrecen alternativas que cumplan con protocolos
And se proporcionan opciones modificadas para el evento
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US24</td><td>Registro de medicamentos en inventario</td><td>Como administrador quiero registrar todos los medicamentos que ingresan al inventario con sus datos completos para mantener un catálogo actualizado</td><td>
    Scenario 1: Registro exitoso de medicamentos
Given un administrador en el módulo de inventario de medicamentos
When registra nuevo medicamento con todos los datos requeridos (nombre, laboratorio, lote, fecha de vencimiento, cantidad)
Then el medicamento se añade correctamente al inventario
And se genera código de identificación único
And se actualiza el stock total disponible
And el sistema registra fecha y responsable del ingreso
Scenario 2: Medicamento duplicado en inventario
Given un administrador registrando medicamento
When intenta ingresar un medicamento que ya existe con el mismo lote
Then el sistema detecta la duplicación y muestra alerta
And permite actualizar cantidad del lote existente en lugar de crear duplicado
And mantiene integridad de datos en el inventario
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US25</td><td>Alertas de vencimiento</td><td>Como administrador quiero recibir alertas automáticas sobre medicamentos próximos a vencer para evitar pérdidas y riesgos de seguridad</td><td>
    Scenario 1: Alert generation for expiring medications
Given medicamentos en inventario próximos a vencer
When faltan 30 días para fecha de vencimiento
Then se genera alerta automática al administrador de farmacia
And la alerta incluye lista de medicamentos, cantidades y fechas exactas
And se sugieren acciones como uso prioritario o devolución a proveedor
And se programa seguimiento semanal hasta resolución
Scenario 2: Medicamentos ya vencidos en inventario
Given medicamentos que han superado su fecha de vencimiento
When el sistema detecta medicamentos vencidos
Then se bloquea automáticamente su uso en el sistema
And se genera alerta crítica para remoción inmediata
And se registra como pérdida en reportes de inventario
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US26</td><td>Eliminación de medicamentos</td><td>Como administrador quiero eliminar medicamentos del inventario de manera controlada para mantener la precisión del stock y cumplir con protocolos de disposición</td><td>
    Scenario 1: Eliminación controlada de medicamento
Given un administrador necesitando eliminar medicamento del inventario
When selecciona medicamento y especifica razón (vencido, dañado, usado)
Then debe proporcionar justificación y autorización apropiada
And el sistema registra la eliminación con fecha, cantidad y responsable
And se actualiza automáticamente el stock disponible
And se genera reporte de eliminación para auditoría
Scenario 2: Intento de eliminación sin autorización
Given un usuario intentando eliminar medicamento sin permisos suficientes
When no posee los permisos necesarios para eliminación
Then el sistema niega el acceso con mensaje explicativo
And se registra el intento en logs de seguridad
And se notifica al administrador sobre el intento no autorizado
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US27</td><td>Búsqueda y filtrado de inventario</td><td>Como administrador quiero filtrar y buscar medicamentos en el inventario para encontrar rápidamente información específica y generar reportes personalizados</td><td>
    Scenario 1: Búsqueda exitosa de medicamentos
Given un administrador en el módulo de inventario
When utiliza filtros de búsqueda por nombre, laboratorio, fecha de vencimiento o categoría
Then obtiene resultados precisos que coinciden con los criterios
And puede ordenar resultados por diferentes campos
And puede exportar los resultados filtrados para reportes
And la búsqueda es rápida y eficiente
Scenario 2: Búsqueda sin resultados
Given un administrador buscando medicamento específico
When los criterios de búsqueda no coinciden con ningún medicamento en inventario
Then se muestra mensaje claro de "sin resultados"
And se sugieren búsquedas alternativas o similares
And puede contactar a proveedores para disponibilidad
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US28</td><td>Información de medicamentos para personal</td><td>Como administrador quiero proporcionar información detallada sobre medicamentos al personal para asegurar administración segura y correcta</td><td>
    Scenario 1: Acceso exitoso a información detallada de medicamentos
Given personal autorizado consultando información de medicamento
When accede a detalles de medicamento específico
Then puede ver información completa: dosificación, contraindicaciones, efectos secundarios, interacciones
And la información está actualizada y es confiable
And puede acceder a protocolos de administración específicos
And tiene enlaces a recursos adicionales si necesita más información
Scenario 2: Medicamento con alertas especiales
Given personal consultando medicamento con requerimientos especiales
When el medicamento tiene alertas de seguridad o administración especial
Then se muestran prominentemente todas las alertas y precauciones
And se requiere confirmación de lectura antes de proceder
And se proporcionan protocolos específicos de manejo
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US29</td><td>Gestión de perfiles de empleados</td><td>Como administrador quiero registrar y mantener los perfiles completos del personal para tener información actualizada de todos los empleados.</td><td>
    Scenario 1: Registro exitoso de empleado
    Given un administrador de RRHH registrando nuevo empleado
When completa información personal, profesional, contactos de emergencia y rol asignado
Then el perfil se crea exitosamente en el sistema
And se genera ID de empleado único
And se asignan permisos según el rol especificado
And el empleado recibe credenciales de acceso al sistema
Scenario 2: Información incompleta de empleado
Given un administrador registrando empleado con información faltante
When faltan datos críticos como certificaciones requeridas o contactos de emergencia
Then el sistema indica específicamente qué información falta
And permite guardar como borrador para completar posteriormente
And no activa permisos hasta que toda la información requerida esté completa
    </td><td>EP08</td>
  </tr>
   <tr>
    <td>US30</td><td>Baja de personal</td><td>Como administrador quiero dar de baja empleados del sistema para mantener registros actualizados y gestionar finalizaciones de contratos.</td><td>
    Scenario 1: Proceso exitoso de baja de empleado
Given un administrador procesando baja de empleado
When especifica fecha de terminación, motivo y procedimientos de entrega
Then se desactivan automáticamente todos los accesos al sistema
And se genera reporte de finalización con tareas pendientes
And se actualiza la estructura organizacional
And se notifica a supervisores y equipos afectados
Scenario 2: Empleado con responsabilidades activas
Given un administrador intentando dar de baja empleado con responsabilidades activas
When el empleado tiene residentes asignados o tareas críticas pendientes
Then el sistema alerta sobre responsabilidades que requieren reasignación
And proporciona lista de tareas y residentes que deben transferirse
And requiere reasignación completa antes de procesar la baja
</td><td>EP08</td>
  </tr>
  <tr>
    <td>US31</td><td>Búsqueda y filtrado de empleados</td><td>Como administrador quiero filtrar y buscar empleados según diferentes criterios para encontrar rápidamente personal específico.</td><td>
    Scenario 1: Búsqueda exitosa de empleados
Given un administrador en el módulo de gestión de personal
When utiliza filtros por departamento, rol, turno, o estado de empleo
Then obtiene lista precisa de empleados que coinciden con criterios
And puede ver información básica de cada empleado en los resultados
And puede acceder a perfiles completos desde los resultados
And puede exportar la lista filtrada para reportes
Scenario 2: Filtros que no retornan resultados
Given un administrador aplicando filtros específicos
When la combinación de filtros no coincide con ningún empleado
Then se muestra mensaje claro indicando ausencia de resultados
And se sugiere modificar criterios de búsqueda
And se mantienen los filtros aplicados para fácil modificación
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US32</td><td>Gestión de horas extra</td><td>Como administrador quiero controlar las horas extra trabajadas por el personal para gestionar costos laborales y cumplir con regulaciones de trabajo</td><td>
    Scenario 1: Registro exitoso de horas extra
Given un administrador registrando horas extra de empleado
When especifica empleado, fecha, horas trabajadas y justificación
Then las horas se registran correctamente en el sistema
And se calculan automáticamente los montos según tarifas establecidas
And se actualiza el reporte mensual de horas extra
And se notifica al empleado sobre el registro
Scenario 2: Horas extra que exceden límites permitidos
Given un administrador registrando horas extra que exceden límites legales
When las horas superan los máximos permitidos por regulaciones laborales
Then el sistema muestra alerta sobre violación de límites
And requiere autorización especial y justificación
And se genera reporte para revisión de RRHH
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US33</td><td>Catálogo de servicios</td><td>Como administrador quiero gestionar la información sobre servicios disponibles para que familias conozcan las opciones de atención</td><td>
    Scenario 1: Gestión exitosa del catálogo de servicios
Given un administrador actualizando catálogo de servicios
When añade, modifica o elimina servicios disponibles
Then los cambios se reflejan inmediatamente en información visible para familias
And cada servicio incluye descripción, costo y disponibilidad
And se mantiene historial de cambios en servicios
And las familias reciben notificación de nuevos servicios disponibles
Scenario 2: Servicio temporalmente no disponible
Given un administrador marcando servicio como no disponible temporalmente
When un servicio no puede prestarse por mantenimiento o falta de personal
Then se actualiza automáticamente el estado en el catálogo
And se notifica a familias que habían solicitado ese servicio
And se proporciona información sobre cuándo estará nuevamente disponible
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US34</td><td>Gestión de horarios de atención</td><td>Como administrador quiero configurar los horarios de atención y servicios para informar claramente a familias sobre disponibilidad</td><td>
    Scenario 1: Configuración exitosa de horarios
Given un administrador configurando horarios de atención
When establece horarios por servicio, día de semana y disponibilidad de personal
Then los horarios se actualizan en toda la plataforma
And las familias pueden ver horarios actualizados al programar visitas o servicios
And se generan calendarios de disponibilidad automáticamente
And se sincroniza con sistemas de programación de citas
Scenario 2: Cambio de horarios por emergencia
Given un administrador modificando horarios por situación de emergencia
When debe cambiar horarios por situaciones imprevistas
Then puede realizar cambios inmediatos con notificación automática
And todas las partes afectadas reciben notificación instantánea
And se reprograman automáticamente citas afectadas
</td><td>EP09</td>
  </tr>
  <tr>
    <td>US35</td><td>Datos de contacto institucional</td><td>Como administrador quiero gestionar la información de contacto de la casa de reposo para que familias y autoridades tengan acceso a datos actualizados</td><td>
    Scenario 1: Actualización exitosa de información de contacto
Given un administrador actualizando datos de contacto institucional
When modifica teléfonos, emails, dirección o personas de contacto
Then la información se actualiza inmediatamente en toda la plataforma
And se refleja en landing page, aplicaciones y documentos oficiales
And se notifica automáticamente a familias sobre cambios importantes
And se mantiene historial de cambios para auditoría
Scenario 2: Información de contacto de emergencia
Given una situación que requiere contacto de emergencia
When familias necesitan contactar urgentemente a la institución
Then tienen acceso inmediato a números de emergencia 24/7
And pueden identificar fácilmente el contacto apropiado según la situación
And reciben respuesta rápida según protocolos de emergencia
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US36</td><td>Información del personal directivo</td><td>Como administrador quiero gestionar la información del personal directivo para transparencia hacia familias y autoridades</td><td>Scenario 1: Gestión de información de personal directivo
Given un administrador actualizando información de personal directivo
When modifica información de directores, coordinadores y personal clave
Then la información se presenta profesionalmente a familias y autoridades
And incluye credenciales, experiencia y áreas de responsabilidad
And se actualiza automáticamente en materiales institucionales
And mantiene información siempre actualizada y verificable
Scenario 2: Acceso a información directiva por autoridades
Given autoridades sanitarias requiriendo información del personal directivo
When necesitan verificar credenciales y responsabilidades del personal clave
Then pueden acceder a información completa y actualizada
And toda la documentación está organizada y es fácilmente verificable
And se proporciona información de contacto directo cuando es apropiado
</td><td>EP09</td>
  </tr>
  <tr>
    <td>US37</td><td>Historia institucional</td><td>Como administrador quiero gestionar la información histórica y reconocimientos de la casa de reposo para generar confianza y credibilidad</td><td>
    Scenario 1: Presentación de historia y reconocimientos institucionales
Given un administrador gestionando información histórica institucional
When actualiza historia, reconocimientos, certificaciones y logros
Then la información se presenta de manera atractiva y creíble
And incluye certificaciones vigentes y reconocimientos oficiales
And genera confianza en familias evaluando los servicios
And es fácilmente accesible para consulta de interesados
Scenario 2: Verificación de certificaciones por autoridades
Given autoridades verificando certificaciones institucionales
When requieren confirmar validez de licencias y reconocimientos
Then pueden acceder a información verificable y actualizada
And todos los documentos incluyen números de registro y fechas de vigencia
And se proporciona contacto directo con entidades certificadoras
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US38</td><td>Gestión de usuarios y permisos</td><td>Como administrador quiero saber quién tiene acceso al sistema y qué información puede ver cada usuario para proteger la privacidad de los datos</td><td>
    Scenario 1: Configuración exitosa de permisos de usuario
Given un administrador de sistema gestionando accesos
When asigna roles y permisos específicos a usuarios (familiares, personal, administradores)
Then cada usuario accede únicamente a información autorizada para su rol
And los permisos se aplican consistentemente en toda la plataforma
And se registra toda actividad de acceso para auditoría
And se pueden modificar permisos sin afectar otros aspectos del sistema
Scenario 2: Intento de acceso no autorizado
Given un usuario intentando acceder a información fuera de sus permisos
When intenta acceder a datos que no le corresponden según su rol
Then el sistema bloquea el acceso inmediatamente
And registra el intento en logs de seguridad
And notifica al administrador sobre el intento no autorizado
And proporciona mensaje claro sobre restricciones de acceso
</td><td>EP10</td>
  </tr>
  <tr>
    <td>US39</td><td>Protección de datos mediante cifrado</td><td>Como administrador quiero que toda la información sensible esté cifrada para proteger los datos personales y médicos de accesos no autorizados</td><td>
    Scenario 1: Cifrado exitoso de datos sensibles
Given el sistema almacenando información personal y médica
When se guardan datos sensibles de residentes y familias
Then toda la información se cifra automáticamente antes del almacenamiento
And las comunicaciones entre usuario y servidor están cifradas
And solo usuarios autorizados pueden descifrar información específica
And se mantienen estándares de seguridad médica requeridos
Scenario 2: Intento de acceso a datos cifrados sin autorización
Given un intento de acceso directo a datos cifrados
When alguien intenta acceder a información sin autorización apropiada
Then los datos permanecen completamente inaccesibles
And se registra el intento de acceso no autorizado
And se activan alertas de seguridad automáticas
And se notifica inmediatamente al equipo de seguridad
    </td><td>EP10</td>
  </tr>
  <tr>
    <td>US40</td><td>Terminos y condiciones</td><td>Como visitante de la landing page quiero poder acceder a los términos y condiciones de uso para conocer las políticas legales antes de contratar los servicios</td><td>
    Scenario 1: Acceso exitoso a términos y condiciones
Given un visitante en la landing page
When busca información legal sobre términos y condiciones de uso
Then puede acceder fácilmente a documento completo desde footer o header
And los términos están redactados claramente y son comprensibles
And incluyen políticas de privacidad, uso de datos y responsabilidades
And están actualizados con fecha de última modificación
Scenario 2: Aceptación requerida de términos actualizados
Given términos y condiciones que han sido actualizados
When un usuario existente ingresa al sistema después de la actualización
Then debe revisar y aceptar los nuevos términos antes de continuar
And se destacan claramente los cambios realizados
And puede comparar versión anterior si lo desea
    </td><td>EP01</td>
  </tr>
   <tr>
    <td>US41</td><td>Menú de navegación consistente</td><td>Como usuario quiero un menú de navegación claro y consistente en todas las páginas para encontrar fácilmente las funciones que necesito</td><td>
    Scenario 1: Navegación consistente en toda la plataforma
Given un usuario en cualquier página de la aplicación
When utiliza el menú de navegación
Then encuentra las mismas opciones organizadas de manera idéntica
And puede acceder a funciones principales desde cualquier página
And el menú se adapta apropiadamente a diferentes tamaños de pantalla
And indica claramente la ubicación actual del usuario
Scenario 2: Menú adaptado a permisos de usuario
Given usuarios con diferentes roles accediendo al sistema
When navegan por la plataforma
Then ven solo opciones de menú apropiadas para su rol
And las opciones restringidas no aparecen para evitar confusión
And pueden identificar fácilmente todas las funciones disponibles para ellos
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US42</td><td>Paleta de colores y tipografía</td><td>Como usuario quiero una interfaz con colores y tipografía consistentes para tener una experiencia visual agradable y fácil de leer</td><td>
    Scenario 1: Aplicación consistente de diseño visual
Given cualquier página de la plataforma Veyra
When un usuario navega por diferentes secciones
Then encuentra colores y tipografía consistentes en toda la experiencia
And el diseño refleja profesionalismo apropiado para servicios de salud
And el contraste de colores cumple estándares de accesibilidad
And la tipografía es legible en diferentes dispositivos y tamaños
Scenario 2: Adaptación para usuarios con necesidades especiales
Given usuarios con dificultades visuales
When acceden a la plataforma
Then pueden utilizar funciones de alto contraste o aumento de texto
And todos los elementos mantienen legibilidad en diferentes configuraciones
And los colores no son el único medio para transmitir información importante
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US43</td><td>Diseño de formularios usables</td><td>Como usuario quiero formularios claros y fáciles de completar para ingresar información sin confusión ni errores</td><td>
    Scenario 1: Completar formularios de manera eficiente
Given un usuario completando cualquier formulario en la plataforma
When ingresa información requerida
Then los campos están claramente etiquetados y organizados lógicamente
And recibe validación en tiempo real para campos incorrectos
And puede guardar progreso para completar posteriormente si es formulario largo
And recibe confirmación clara al completar exitosamente
Scenario 2: Formulario con errores de validación
Given un usuario enviando formulario con información incorrecta
When existen errores en los datos ingresados
Then recibe mensajes de error específicos y constructivos
And se mantiene toda la información correcta ya ingresada
And puede corregir errores fácilmente sin empezar desde cero
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US44</td><td>Patrones de diseño coherentes</td><td>Como usuario quiero que todas las pantallas sigan patrones de diseño similares para predecir dónde encontrar funciones y cómo interactuar</td><td>
    Scenario 1: Interacción predecible en toda la plataforma
Given un usuario familiarizado con una sección de la plataforma
When navega a nuevas secciones
Then encuentra patrones de interacción similares y predecibles
And botones, enlaces y controles funcionan de manera consistente
And puede aplicar conocimiento previo para usar nuevas funcionalidades
And la experiencia se siente uniforme y profesional
Scenario 2: Nuevos usuarios aprendiendo la interfaz
Given un nuevo usuario accediendo por primera vez
When explora diferentes funcionalidades
Then puede predecir cómo funcionarán nuevas secciones basándose en experiencia previa
And encuentra elementos de interfaz en ubicaciones esperadas
And puede desarrollar eficiencia rápidamente en el uso del sistema
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US45</td><td>Manejo de errores comprensible</td><td>Como usuario quiero que los errores se presenten de forma clara y con soluciones sugeridas para resolver problemas sin frustración</td><td>
    Scenario 1: Error del sistema con guía de resolución
Given un error técnico durante el uso de la plataforma
When ocurre un problema de sistema o conectividad
Then el usuario recibe mensaje claro explicando qué ocurrió
And se proporcionan pasos específicos para resolver el problema
And se ofrecen alternativas de contacto si el problema persiste
And se registra el error para mejora continua del sistema
Scenario 2: Error de usuario con orientación educativa
Given un usuario cometiendo error en el uso de la plataforma
When realiza una acción incorrecta o no permitida
Then recibe explicación clara sobre por qué no se pudo completar la acción
And se le orienta sobre la forma correcta de proceder
And puede corregir fácilmente su acción sin frustración
And aprende a evitar el mismo error en el futuro
    </td><td>EP11</td>
   </tr>
</table>

<h3 id="Technical"> Technical Stories</h3>
<table border="1" style="border-collapse: collapse; width: 100%;font-size: 12px; font-family: Arial, sans-serif;">
  <tr>
    <td>ID</td><td>Título</td><td>Historia de Usuario</td><td>Criterios de Aceptación
</td>
  </tr>
  <tr>
    <td>TS01</td><td>Eliminar  medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Delete para medicamentos  para asegurar que el administrador de la  casa de reposo pueda remover registros del inventario .</td><td>
    Scenario 1: Eliminación exitosa
Given un administrador autenticado con permisos y un medicamentoId existente
When envía DELETE /medicamentos/{medicamentoId}
Then el servicio responde 204 No Content, el registro queda  como eliminado  y se muestra 
que se borro en la base de datos .

Scenario 2: Eliminación fallida por inexistencia o falta de permisos
Given un usuario sin permisos o un medicamentoId inexistente
When intenta DELETE /medicamentos/{medicamentoId}
Then el servicio responde 403 si no tiene permisos, o 404 Not Found si el id no existe, y el intento queda registrado en logs.
    </td>
  </tr>
  <tr>
    <td>TS02</td><td>Agregar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Post  medicamentos  para permitir que el administrador de la casa de reposo pueda agregar más medicamentos. </td><td>
    Scenario 1: Creación exitosa
Given un administrador autenticado y un registro de datos válido en los campos obligatorios (nombre, lote, fechaVencimiento, cantidad)
When envía POST /medicamentos
Then el servicio responde 201 Created  y el medicamento queda persistido en base de datos.

Scenario 2: Error de validación o duplicado
Given un registro con campos faltantes o que coincide con un medicamento existente.
When envía POST /medicamentos
Then el servicio responde 400 Bad Request para validaciones o 409 Conflict si es duplicado, con mensajes de error detallados.
    </td>
  </tr>
  <tr>
    <td>TS03</td><td>Ver información detallada de los medicamentos</td><td>Como desarrollador backend en NovaPeru Tech quiero crear una función para ver la información a través de una Api para que </td><td>
    Scenario 1: Consulta exitosa
Given un usuario autenticado y autorizado y un medicamentoId válido
When solicita GET /medicamentos/{medicamentoId}
Then el servicio responde 200 OK con el JSON .
Scenario 2: Recurso no encontrado o sin permisos
Given un medicamentoId inexistente o un usuario sin autorización
When solicita GET /medicamentos/{medicamentoId}
Then el servicio responde 404 Not Found si no existe.
    </td>
  </tr>
  <tr>
    <td>TS04</td><td>Actualizar información de medicamentos</td><td>Como desarrollador de backend en NovaPeru Tech quiero crear una función para actualizar la información para asegurar que el administrador de la casa de reposos pueda mantener actualizada la inforción de cada medicamento</td><td>
    Scenario 1: Actualización exitosa con control de concurrencia
Given un usuario autorizado y un medicamentoId existente y registro de datos válido
When envía PUT/PATCH /medicamentos/{medicamentoId}
Then el servicio responde 200 OK, aplica los cambios, registra la modificación en la base de datos.

Scenario 2: Conflicto o validación fallida
Given registro de la nueva información no es valida .
When intenta PUT/PATCH /medicamentos/{medicamentoId}
Then el servicio responde  400 Bad Request para datos inválidos.
    </td>
  </tr>
  <tr>
    <td>TS05</td><td>Agregar pacientes</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para permitir que el administrador registre nuevos residentes con validaciones obligatorias y que se genere un ID único por residente.</td><td>
    Scenario 1: Registro exitoso de residente
Given administrador autenticado y ingresa  datos válidos
When envía POST /residents
Then el servicio responde 201 Created, retorna residentId y persiste el registro en la base de datos.

Scenario 2: Duplicado o campos faltantes
Given un registro con documento de identidad ya registrado o campos obligatorios faltantes
When envía POST /residents
Then el servicio responde 400 Bad Request si faltan datos, con detalles de error.
    </td>
  </tr>
  <tr>
    <td>TS06</td><td>Ver información detallada  de los pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET  que devuelva la información completa del residente para que el personal autorizado pueda consultar fácilmente el expediente.</td><td>
    Scenario 1: Consulta autorizada
Given personal autorizado  y residentId válido
When solicita GET /residents/{residentId}
Then recibe 200 OK con datos personales, contactos autorizados y resumen del historial médico.

Scenario 2: Sin permisos o recurso inexistente
Given usuario sin permisos para ver datos médicos o residentId no existente
When solicita GET /residents/{residentId}
Then el servicio responde  404 Not Found si el residente no existe.
    </td>
  </tr>
  <tr>
    <td>TS07</td><td>Eliminar paciente  </td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE  que realice una eliminación controlada  del residente.
    </td><td>
    Scenario 1: Baja controlada exitosa
Given administrador autenticado 
When envía DELETE /residents/{residentId}
Then el sistema marca inactive, revoca accesos asociados.

Scenario 2: Eliminación fallida
Given Administrador con responsabilidades activas
When intenta DELETE /residents/{residentId}
Then el servicio responde 409 Conflict y devuelve lista de acciones requeridas para completar la eliminación.
    </td>
  </tr>
  <tr>
    <td>TS08</td><td>Actualizar información de los pacientes </td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH  para actualizar campos del perfil del residente para que las modificaciones queden registradas y sean reversibles si es necesario</td><td>
    Scenario 1: Actualización válida y registrada
Given Administrador  autorizado y registro de datos permitidos  correcto
When envía PATCH /residents/{residentId}
Then el servicio responde 200 OK, aplica los cambios permitidos y guarda un registro de auditoría con diff de cambios.

Scenario 2: Intento de modificar campos restringidos o datos inválidos
Given registro de datos  que incluye campos de solo lectura o formato inválido
When envía PATCH /residents/{residentId}
Then el servicio responde 400 Bad Request para validaciones, sin aplicar cambios.
    </td>
  </tr>
  <tr>
    <td>TS09</td><td>Agregar información detallada de la casa de reposo</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que un administrador pueda registrar información institucional .
    </td><td>
    Scenario 1: Creación de información institucional exitosa
Given administrador autenticado y registro de datos  válido 
When envía POST /institution-info
Then el servicio responde 201 Created y los datos quedan disponibles  en la app.

Scenario 2: Error por falta de permisos o validación
Given usuario no administrador o registro de datos obligatorios faltantes
When envía POST /institution-info
Then el servicio responde  400 Bad Request si faltan campos.
    </td>
  </tr>
  <tr>
    <td>TS010</td><td>Actualizar información de la casa de reposo</td><td>
    Como desarrollador backend en NovaPeru tech quiero crear un endpoint PUT para mantener actualizados los datos institucionales.
    </td><td>
    Scenario 1: Actualización exitosa y auditada
Given administrador autenticado, payload válido y versión coincidente
When envía PUT/PATCH /institution-info/{id}
Then el servicio responde 200 OK, actualiza los datos y registra quien y cuándo realizó el cambio.

Scenario 2: Conflicto de versión o datos inválidos
Given versión desincronizada o registro de datos inválido
When intenta PUT/PATCH /institution-info/{id}
Then el servicio responde 400 Bad Request por validación.
    </td>
  </tr>
  <tr>
    <td>TS011</td><td>Agregar empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que registre nuevos empleados.</td><td>
    Scenario 1: Registro de empleado exitoso
Given Administrador autenticado y registro de datos válido 
When envía POST /employees
Then el servicio responde 201 Created, devuelve employeeId, asigna permisos iniciales y crea credenciales seguras.

Scenario 2: Error por email/ID duplicado o validación
Given email o documento ya registrado o campos inválidos
When envía POST /employees
Then el servicio responde 409 Conflict para duplicados o 400 Bad Request para validaciones.
    </td>
  </tr>
  <tr>
    <td>TS012</td><td>Eliminar empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE para que el administrador de la casa de reposo revoque persmisos. 
    </td><td>
    Scenario 1: Baja controlada exitosa
Given administrador autenticado y empleado sin tareas críticas pendientes
When envía DELETE /employees/{employeeId}
Then el servicio elmina empleado , registra la acción en base de datos.

Scenario 2: Baja bloqueada por responsabilidades activas o sin permisos
Given empleado con residentes/tareas asignadas o petición desde usuario sin permisos
When intenta DELETE /employees/{employeeId}
Then el servicio responde 409 Conflict indicando reasignaciones requeridas, o 403 Forbidden si el solicitante no está autorizado.
    </td>
  </tr>
  <tr>
    <td>TS013</td><td>Actualizar información del empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar datos de empleado.
    </td><td>
    Scenario 1: Actualización válida con auditoría
Given Administrador  autenticado y registra datos  válido
When envía PATCH /employees/{employeeId}
Then el servicio responde 200 OK y registra el cambio en la base de datos.

Scenario 2: Intento de actualizar datos inválidos
Given intento de registrar datos  inválido
When envía PATCH /employees/{employeeId}
Then el servicio responde 400 Bad Request para datos inválidos.
    </td>
  </tr>
  <tr>
    <td>TS014</td><td>Ver información del empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET que muestre el perfil del empleado para que el administrador pueda observar cuantos empleados tiene.
    </td><td>
    Scenario 1: Consulta autorizada del perfil
Given usuario autorizado  y employeeId válido
When solicita GET /employees/{employeeId}
Then el servicio responde 200 OK , se filtran según permisos.

Scenario 2: empleado no existe
Given  employeeId inexistente
When solicita GET /employees/{employeeId}
Then el servicio responde  404 Not Found si no existe.
    </td>
  </tr>
  <tr>
    <td>TS015</td><td>Consumir Api de Medicamentos</td><td>
    Como desarrollador backend en NovaPeru tech quiero consumir la API externa de medicamentos mediante un servicio de integración , para disponer de información confiable y actualizada de medicamentos en el sistema.
    </td><td>
    Scenario 1: Sincronización exitosa y segura
Given credenciales válidas para la API externa y conectividad estable
When se ejecuta sincronización programada o petición 
Then los datos externos se mapean y normalizan al modelo interno, se guardan cambios.

Scenario 2: Fallo externo
Given timeout en la API externa o respuesta que no cumple el esquema esperado
When intenta sincronizar
Then el servicio  registra la incidencia en logs y no sobrescribe datos locales hasta validación.
    </td>
  </tr>
  <tr>
    <td>TS016</td><td>Consumir Api de google maps</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de integración con Google Maps que proporcione  verificación de direcciones y datos de localización para manejar errores.</td><td>
    Scenario 1: Geocoding verificado vía proxy
Given API key protegida en backend y request válido (dirección)
When solicita geocoding a través del proxy GET /maps/proxy?address=...
Then el proxy devuelve datos normalizados (lat/lng, formato) y la API key no se expone al frontend.

Scenario 2: Rate limit o error del proveedor
Given Google Maps devuelve 429 o falla por timeout
When realiza la petición al proxy
Then el proxy responde 429 o 503 con mensaje controlado, aplica política de backoff y utiliza cache fallback si existe.
    </td>
  </tr>
  <tr>
    <td>TS017</td><td>Nofitifación de visitas</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de notificaciones para enviar recordatorios y alertas de visitas vía email/SMS</td><td>
    Scenario 1: Envío de recordatorio exitoso
Given visita programada y contactos válidos con preferencias de notificación
When falta el tiempo configurado (p.ej. 2 horas) y la cola procesa el job
Then se envía notificación vía canal configurado (email/SMS/push), el sistema registra el estado delivered y actualiza el registro de visita.

Scenario 2: Fallo en entrega y reintentos
Given fallo de entrega
When el worker intenta enviar la notificación
Then el sistema aplica reintentos configurados .
    </td>
  </tr>
  <tr>
    <td>TS018</td><td>Buscar y filtrar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET con parámetros de búsqueda  facilitar consultas rápidas y generación de reportes. </td><td>
    Scenario 1: Búsqueda paginada exitosa
Given parámetros válidos 
When solicita GET /medicamentos
Then el servicio responde 200 OK con lista .

Scenario 2: Parámetros inválidos o sin resultados
Given parámetros inválidos  o criterio que no retorna matches
When solicita GET /medicamentos
Then el servicio responde 400 Bad Request para parámetros inválidos o 200 OK con items: [] y totalItems: 0 si no hay resultados.
    </td>
  </tr>
  <tr>
    <td>TS019</td><td>BUsccar y filtrar residentes</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET con filtros para que administradores y personal autorizado encuentren residentes fácilmente.</td><td>
    Scenario 1: Consulta filtrada y autorizada
Given filtros válidos  y usuario autorizado
When solicita GET /residents?nombre=X&habitacion=Y
Then el servicio responde 200 OK con resultados paginados y campos conforme a permisos del solicitante.

Scenario 2: Intento sin permisos o parámetros inválidos
Given usuario sin permiso para ver datos sensibles o parámetros mal formados
When solicita GET /residents?
Then el servicio responde 400 Bad Request si los parámetros son inválidos.
    </td>
  </tr>
  <tr>
    <td>TS020</td><td>Buscar y filtrar empleados</td><td>
    Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que permita buscar y filtrar por nombre, rol, turno que se pueda exportar para que vea el reporte de empleados el admnistrador o RRHH.</td><td>
        Scenario 1: Búsqueda y exportación permitida
Given parámetros válidos y usuarios con permiso de exportación
When solicita GET /employees?rol=cuidador&export=true
Then el servicio responde 200 OK iniciando exportación (CSV) y devuelve enlace de descarga cuando esté listo.

Scenario 2: Exportación denegada o sin resultados
Given  filtros que no arrojan resultados
When solicita GET /employees
Then el servicio responde 400 si no coincide .
    </td>
  </tr>
</table>


<h3 id="impactMapping">3.2. Impact Mapping</h3>

<img src="../images/Impact map 1.png" alt="Impact map 1" width="auto" height="auto"/>

<h3 id="productBacklog">3.3. Product Backlog.</h3>
<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr>
    <td>Ordern</td><td> User Story Id</td><td>Título</td><td>Descripción</td><td>Story Points(1/2/3/5/8)</td>
  </tr>
  <tr>
    <td>1</td><td></td><td></td><td></td><td></td>
  </tr>
  <tr>
    <td>2</td><td></td><td></td><td></td><td></td>
  </tr>
  <tr>
    <td>3</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>4</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>5</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>6</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>7</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>8</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>9</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>10</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>11</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>12</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>13</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>14</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>15</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>16</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>17</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>18</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>19</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>20</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>21</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>22</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>23</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>24</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>25</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>26</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>27</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>28</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>29</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>30</td><td></td><td></td><td></td><td></td>
  </tr>
      <tr>
    <td>31</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>32</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>33</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>34</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>35</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>36</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>37</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>38</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>39</td><td></td><td></td><td></td><td></td>
  </tr>
     <tr>
    <td>40</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>41</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>42</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>43</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>44</td><td></td><td></td><td></td><td></td>
  </tr>
   <tr>
    <td>45</td><td></td><td></td><td></td><td></td>
  </tr>
</table>
