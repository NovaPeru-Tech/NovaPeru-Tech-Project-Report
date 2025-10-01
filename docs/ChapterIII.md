# Capítulo III: Requirements Specification

## 3.1. User Stories
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
   <strong>Escenario 1 : Menú visible y navegable</strong> <br>
Dado un visitante en la landing page
cuando la página carga por completo y el visitante hace clic (o toca) un enlace del menú
entonces el menú está visible en la parte superior con los enlaces principales ("Log in", "Sign up", "Planes", "Contacto") y el visitante es redirigido a la sección correspondiente sin errores. <br> <br>

<strong>Escenario 2 : Menú no carga o enlace roto</strong> <br>
Dado un visitante en la landing page
cuando el menú no se renderiza por fallo de recursos  o al hacer clic en un enlace la ruta devuelve error/404
entonces se muestra un mensaje amigable  y el visitante puede acceder a las secciones esenciales mediante enlaces alternativos  sin bloquear la exploración. </td><td>EP01</td>
  </tr>
  <tr>
    <td>US02</td><td>Visualización de Planes </td><td>Como visitante de la Landing Page, quiero ver los planes de suscripción junto a su precio y características, para poder elegir el que mejor se adapte a mis necesidades.</td><td>
    Escenario 1: Visualización correcta de planes
Dado un visitante en la sección de planes de la landing page
cuando la página carga completamente
entonces debe ver al menos 2 planes de suscripción diferentes
y cada plan debe mostrar claramente: precio, características principales, duración y botón de selección
y debe poder comparar fácilmente las diferencias entre planes
y todos los elementos deben ser legibles y estar correctamente alineados
Escenario 2: Error en carga de planes
Dado un visitante en la sección de planes
cuando ocurre un error en la carga de información de planes
entonces se muestra un mensaje de error amigable
y se proporciona una opción para recargar la información
y el visitante puede acceder a información de contacto como alternativa
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US03</td><td>Selección de Plan en Landing Page</td><td>Como visitante de la landing Page, quiero seleccionar un plan y finalizar la confirmación en la misma pantalla, para agilizar y simplificar el registro.</td><td>
    Escenario 1: Selección y confirmación exitosa
    Dado un visitante visualizando los planes disponibles
cuando selecciona un plan específico y hace clic en "Seleccionar"
entonces es dirigido a un formulario de confirmación en la misma pantalla
y el formulario muestra el plan seleccionado con su precio
y puede completar sus datos y confirmar la selección
y recibe una confirmación inmediata del proceso
Escenario 2: Selección sin completar datos requeridos
Dado un visitante en el formulario de confirmación de plan
cuando intenta confirmar sin completar campos obligatorios
entonces se muestran mensajes de validación específicos para cada campo faltante
y el formulario mantiene la información ya ingresada
y puede corregir y reenviar sin perder progreso
</td><td>EP01</td>
  </tr>
    <tr>
    <td>US04</td><td>Visualización de creadores</td><td>Como visitante de la Landing Page, quiero ver a los creadores de la aplicación, para conocer al equipo detrás del producto y generar confianza en el servicio.</td><td>
    Escenario 1: Acceso exitoso a información del equipo
Dado un visitante en la landing page
cuando navega a la sección "Sobre nosotros" o "Equipo"
entonces puede ver información de cada creador incluyendo: nombre, foto, rol y breve descripción
y la información se presenta de manera profesional y organizada
y puede acceder a perfiles profesionales o redes sociales si están disponibles
Escenario 2: Información de equipo no disponible
Dado un visitante intentando acceder a información del equipo
cuando la sección no carga correctamente
entonces se muestra un mensaje explicativo
y se proporciona información de contacto alternativa
y el visitante puede continuar navegando otras secciones sin problemas
    </td><td>EP01</td>
  </tr>
    <tr>
    <td>US05</td><td>Redes sociales</td><td>Como visitante del landing page quiero poder acceder fácilmente a sus redes sociales de Veyra para conocer más sobre la empresa y tener canales adicionales de contacto </td><td>
    Escenario 1: Acceso exitoso a redes sociales
Dado un visitante en cualquier página de la landing page
cuando busca enlaces a redes sociales en el footer o header
entonces encuentra íconos claramente identificables de las principales redes sociales
y al hacer clic, se abren en nueva pestaña las páginas oficiales de Veyra
y los enlaces funcionan correctamente y dirigen al contenido apropiado
Escenario 2: Enlaces de redes sociales no funcionales
Dado un visitante intentando acceder a redes sociales
cuando hace clic en un ícono de red social que no funciona
entonces recibe un mensaje de error informativo
y se proporciona información de contacto alternativa
y puede continuar su navegación sin interrupciones
</td><td>EP02</td>
  </tr>
    <tr>
    <td>US06</td><td>Formulario de contacto</td><td>Como visitante del landing page quiero completar un formulario de contacto para enviar consultas específicas y recibir una respuesta personalizada de Veyra</td><td>
    Escenario 1: Envío exitoso de consulta
    Dado un visitante en el formulario de contacto
cuando completa todos los campos requeridos (nombre, email, asunto, mensaje)
y hace clic en "Enviar"
entonces recibe una confirmación de que su mensaje fue enviado
y se le informa el tiempo estimado de respuesta
y recibe una copia de confirmación en su email
Escenario 2: Formulario con datos inválidos
Dado un visitante completando el formulario de contacto
cuando ingresa un email inválido o deja campos obligatorios vacíos
y intenta enviar el formulario
entonces se muestran mensajes de validación específicos
y se mantiene la información correcta ya ingresada
y puede corregir errores y reenviar
</td><td>EP02</td>
  </tr>
    <tr>
    <td>US07</td><td>Cambio de idioma</td><td>Como visitante del Landing Page quiero en el menú un botón para cambiar de idioma entre español e inglés para  entender mejor de que trata Veyra</td><td>
    Escenario 1: Cambio exitoso de idioma
Dado un visitante en la landing page en español
cuando hace clic en el botón de cambio de idioma y selecciona inglés
entonces toda la interfaz cambia al idioma seleccionado
y el contenido se mantiene equivalente en significado
y la preferencia de idioma se mantiene al navegar entre páginas
Escenario 2: Idioma no disponible temporalmente
Dado un visitante intentando cambiar de idioma
cuando el servicio de traducción no está disponible
entonces se muestra un mensaje informativo sobre la situación
y se mantiene el idioma actual funcionando
y se proporciona información en el idioma disponible
</td><td>EP01</td>
  </tr>
    <tr>
    <td>US08</td><td>Historial médico </td><td>Como familiar de un adulto mayor quiero acceder al historial médico completo de mi familiar para conocer su evolución de salud y diagnósticos actuales</td><td>Escenario 1: Acceso exitoso al historial médico
    Dado un familiar autenticado en el sistema
cuando navega a la sección "Historial Médico" de su familiar
entonces puede ver diagnósticos actuales, evolución de salud y últimas actualizaciones
y la información está organizada cronológicamente
y puede filtrar por fechas o tipos de reportes
y toda la información es legible y está actualizada
Escenario 2: Sin permisos para acceder a reportes
Dado un usuario intentando acceder a historial médico
cuando no tiene los permisos necesarios
entonces se muestra un mensaje claro sobre restricciones de acceso
y se proporciona información sobre cómo obtener permisos
y puede contactar al administrador para resolver el acceso
</td><td>EP03</td>
  </tr>
    <tr>
    <td>US09</td><td>Agenda de citas Medicas</td><td>Como familiar de un adulto mayor quiero consultar la agenda de citas médicas de mi familiar para estar informado sobre sus próximos tratamientos</td><td>
    Escenario 1: Visualización exitosa de citas programadas
Dado un familiar autenticado en el sistema
cuando accede a la agenda de citas de su familiar
entonces puede ver todas las citas programadas con fecha, hora, médico y tipo de consulta
y puede filtrar por rangos de fechas
y recibe indicaciones claras sobre próximas citas importantes
y puede exportar o imprimir la agenda si es necesario
Escenario 2: No hay citas programadas
Dado un familiar consultando la agenda de citas
cuando no hay citas programadas para su familiar
entonces se muestra un mensaje informativo indicando que no hay citas
y se proporciona información sobre cómo programar nuevas citas
y puede contactar al personal médico si es necesario
</td><td>EP03</td>
  </tr>
    <tr>
    <td>US10</td><td>Consulta de información personal</td><td>Como familiar de un adulto mayor quiero ver la información de mi familiar para estar seguro de que esté correcto o actualizado.</td><td>
    Escenario 1: Visualización exitosa de información personal
Dado un familiar autenticado en el sistema
cuando accede al perfil de información personal de su familiar
entonces puede ver datos personales actualizados: nombre, edad, contacto de emergencia, alergias, medicamentos actuales
y puede identificar fácilmente si algún dato requiere actualización
y tiene acceso a opciones para solicitar modificaciones
Escenario 2: Información desactualizada detectada
Dado un familiar revisando información personal
cuando identifica información que necesita actualización
entonces puede marcar campos como "requiere actualización"
y puede enviar solicitudes de cambio con justificación
y recibe confirmación de que la solicitud fue recibida
    </td><td>EP03</td>
  </tr>
   <tr>
    <td>US11</td><td>Galería de fotos y actividades</td><td>Como familiar de un adulto mayor quiero ver fotos de las actividades diarias de mi familiar para sentirme conectado con su día a día y verificar su participación social</td><td>
    Escenario 1: Acceso exitoso a galería de actividades
Dado un familiar autenticado en el sistema
cuando accede a la galería de fotos de su familiar
entonces puede ver fotos organizadas por fecha y tipo de actividad
y cada foto incluye descripción de la actividad realizada
y puede filtrar por fechas o tipos de actividades
y las fotos se cargan correctamente y son de buena calidad
Escenario 2: Sin actividades recientes registradas
Dado un familiar consultando la galería
cuando no hay fotos recientes de actividades
entonces se muestra un mensaje informativo sobre la situación
y se proporciona información sobre la frecuencia de actualización de fotos
y puede contactar al personal para consultas específicas
</td><td>EP03</td>
  </tr>
   <tr>
    <td>US12</td><td>Registro de residentes</td><td>Como administrador de casa de reposo quiero crear y mantener perfiles completos de cada residente para centralizar toda su información personal y médica</td><td>
    Escenario 1: Creación exitosa de perfil de residente
Dado un administrador autenticado en el sistema
cuando accede al formulario de registro de nuevo residente
y completa toda la información requerida (datos personales, médicos, contactos de emergencia)
entonces el perfil se crea exitosamente
y se genera un ID único para el residente
y toda la información queda almacenada y accesible para consultas futuras
Escenario 2: Error en datos requeridos para registro
Dado un administrador creando perfil de residente
cuando falta información crítica requerida
y intenta guardar el perfil incompleto
entonces se muestran mensajes específicos de campos faltantes
y se mantiene la información ya ingresada
y puede completar los datos faltantes y continuar
    </td><td>EP04</td>
  </tr>
   <tr>
    <td>US13</td><td>Historial médico institucional</td><td>Como administrador quiero gestionar el historial médico completo de cada residente para asegurar continuidad en el cuidado y cumplir con regulaciones sanitarias
    </td><td>
    Escenario 1: Gestión exitosa de historial médico completo
    Dado un administrador con permisos médicos
cuando accede al historial médico de un residente
entonces puede ver, agregar y actualizar información médica completa
y puede registrar nuevos diagnósticos, tratamientos y evoluciones
y toda la información queda registrada con fecha, hora y responsable
y puede generar reportes médicos para autoridades sanitarias
Escenario 2: Acceso sin permisos médicos suficientes
Dado un usuario intentando acceder a historial médico institucional
cuando no posee los permisos necesarios
entonces se restringe el acceso con mensaje explicativo
y se proporciona información sobre cómo obtener permisos apropiados
y puede acceder solo a información no confidencial si corresponde
</td><td>EP04</td>
  </tr>
   <tr>
    <td>US14</td><td>Administración de medicamentos</td><td>Como administrador quiero controlar la administración de medicamentos de todos los residentes para garantizar cumplimiento de tratamientos y evitar errores médicos</td><td>
    Escenario 1: Control exitoso de administración de medicamentos
Dado un administrador en el módulo de medicamentos
cuando registra la administración de medicamentos a residentes
entonces puede marcar medicamentos como administrados con hora exacta
y puede registrar observaciones sobre efectos o reacciones
y el sistema alerta sobre próximas dosis programadas
y mantiene historial completo de administración por residente
Escenario 2: Medicamento no disponible en inventario
Dado un administrador intentando registrar administración de medicamento
cuando el medicamento no está disponible en inventario
entonces el sistema muestra alerta de falta de stock
y proporciona opciones para contactar a farmacia o proveedor
y permite registrar la situación para seguimiento
    </td><td>EP04</td>
  </tr>
   <tr>
    <td>US15</td><td>Gestión de visitas familiares</td><td>Como administrador quiero controlar y programar las visitas familiares a los residentes para mantener seguridad, orden y cumplir con los horarios establecidos</td><td>
    Escenario 1: Programación exitosa de visita familiar
Dado un administrador en el módulo de visitas
cuando programa una nueva visita familiar
entonces puede asignar fecha, hora, visitantes y residente a visitar
y el sistema verifica disponibilidad de horarios
y genera confirmación para la familia y actualiza agenda institucional
y envía recordatorios automáticos antes de la visita
Escenario 2: Conflicto de horarios en visitas
Dado un administrador programando visita familiar
cuando el horario solicitado ya está ocupado
entonces el sistema muestra horarios alternativos disponibles
y permite reprogramar o sugerir opciones similares
y notifica a la familia sobre el cambio de horario
</td><td>EP04</td>
  </tr>
   <tr>
    <td>US16</td><td>Recordatorios de citas y consultas</td><td> Como familiar quiero recibir recordatorios automáticos sobre citas médicas y consultas programadas de mi familiar para estar preparado y decidir si deseo acompañarlo</td><td>
    Escenario 1: Envío exitoso de recordatorios automáticos
Dado el sistema con citas médicas programadas
cuando se acerca una cita médica (24 horas antes)
entonces se envía recordatorio automático a familiares vía email/SMS
y el recordatorio incluye fecha, hora, médico y tipo de consulta
y los familiares pueden confirmar asistencia o reagendar
y el sistema registra la confirmación recibida
Escenario 2: Falla en envío de recordatorios
Dado el sistema intentando enviar recordatorios
cuando falla el servicio de notificaciones
entonces se registra el error en logs del sistema
y se intenta reenvío automático después de un tiempo
y se notifica al administrador sobre fallas en el sistema
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US17</td><td>Notificaciones de cambios en medicación</td><td>Como familiar quiero ser notificado inmediatamente sobre cualquier cambio en la medicación de mi familiar para estar informado sobre su tratamiento médico</td><td>
    Escenario 1: Notificación inmediata de cambio en medicación
Dado un cambio en la medicación de un residente
cuando el médico actualiza el tratamiento farmacológico
entonces se envía notificación inmediata a familiares autorizados
y la notificación incluye detalles del cambio y justificación médica
y los familiares pueden contactar al médico para consultas
y el cambio queda registrado en el historial médico
Escenario 2: Familiar no autorizado para recibir información médica
Dado un cambio en medicación de residente
cuando un familiar no está autorizado para recibir información médica
entonces no recibe notificación de cambios en medicación
y se respetan las preferencias de privacidad del residente
y solo familiares autorizados reciben las notificaciones
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US18</td><td>Recordatorios de visitas familiares</td><td>Como familiar quiero recibir recordatorios automáticos sobre mis visitas programadas al adulto mayor para no olvidar las citas y mantener regularidad en el contacto</td><td>
    Escenario 1: Recordatorio exitoso de visita programada
Dado una visita familiar programada
cuando faltan 2 horas para la visita
entonces se envía recordatorio automático al familiar
y el recordatorio incluye fecha, hora, nombre del residente y instrucciones de acceso
y el familiar puede confirmar asistencia o cancelar con anticipación
y el sistema actualiza el estado de la visita según la respuesta
Escenario 2: Cancelación de visita por emergencia
Dado una visita familiar programada
cuando ocurre una emergencia que requiere cancelar la visita
entonces se envía notificación inmediata de cancelación
y se proporciona explicación de la situación
y se ofrecen alternativas de reprogramación
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US19</td><td>Alertas de actualización de datos personales</td><td>Como familiar quiero recibir notificaciones automáticas cuando se actualice la información personal o de mi familiar para mantenerme informado de cualquier cambio en su perfil</td><td>
    Escenario 1: Notificación exitosa de actualización de datos
Dado una actualización en datos personales del residente
cuando se modifica información como contacto de emergencia, estado de salud, o preferencias
entonces se envía notificación automática a familiares autorizados
y la notificación especifica qué información fue actualizada
y incluye fecha y responsable de la actualización
y los familiares pueden revisar los cambios en el sistema
Escenario 2: Actualización sin autorización para notificar
Dado una actualización en datos personales
cuando el familiar no tiene autorización para recibir cierto tipo de información
entonces no recibe notificación sobre datos restringidos
y solo recibe información sobre cambios que está autorizado a conocer
y se respetan las políticas de privacidad establecidas
    </td><td>EP05</td>
  </tr>
   <tr>
    <td>US20</td><td>Preguntas sobre rutina de cuidados</td><td>Como familiar quiero hacer preguntas específicas sobre la rutina diaria y cuidados de mi familiar para entender mejor su día a día y resolver dudas puntuales</td><td>
    Escenario 1: Envío exitoso de pregunta sobre cuidados
Dado un familiar autenticado en el sistema de comunicación
cuando redacta una pregunta específica sobre la rutina de cuidados de su familiar
entonces puede enviar la consulta al personal de cuidadores asignado
y recibe confirmación de que la pregunta fue enviada
y el sistema establece un tiempo estimado de respuesta
y puede hacer seguimiento del estado de su consulta
Escenario 2: Canal de comunicación no disponible
Dado un familiar intentando enviar pregunta sobre cuidados
cuando el sistema de comunicación no está disponible
entonces se muestra mensaje sobre la situación temporal
y se proporcionan números de teléfono alternativos para emergencias
y se permite guardar la pregunta para envío posterior
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US21</td><td>Peticiones de modificación de cuidados</td><td>Como familiar quiero solicitar ajustes específicos en el cuidado de mi familiar basados en sus preferencias o necesidades particulares</td><td>
    Escenario 1: Solicitud exitosa de modificación de cuidados
Dado un familiar con permisos para solicitar cambios
cuando envía una petición detallada de modificación en cuidados específicos
entonces la solicitud se registra en el sistema con número de seguimiento
 y se notifica al coordinador de cuidados correspondiente
y recibe confirmación con plazos estimados de evaluación
y puede hacer seguimiento del estado de su petición
Escenario 2: Solicitud que requiere aprobación médica
Dado un familiar solicitando modificación que requiere aprobación médica
cuando la petición involucra aspectos médicos o terapéuticos
entonces se deriva automáticamente al equipo médico
y se informa al familiar sobre el proceso de evaluación médica
y se establecen plazos específicos para respuesta médica
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US22</td><td>Seguimiento del bienestar emocional</td><td>Como familiar quiero comunicarme con el personal sobre el estado emocional y psicológico de mi familiar para asegurar su bienestar integral</td><td>
    Escenario 1: Comunicación exitosa sobre estado emocional
Dado un familiar preocupado por el bienestar emocional de su familiar
cuando envía consulta sobre estado anímico, interacción social o adaptación
entonces puede comunicarse directamente con el equipo de psicología/trabajo social
y recibe respuesta profesional sobre la situación emocional del residente
y se le proporcionan recomendaciones para apoyo emocional
y puede programar reuniones de seguimiento si es necesario
Escenario 2: Situación emocional que requiere atención inmediata
Dado un familiar reportando cambios emocionales significativos
cuando la situación indica posible crisis emocional o depresión
entonces se escalona automáticamente a atención psicológica prioritaria
y se notifica al equipo médico y de trabajo social
y se contacta al familiar para coordinar intervención
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US23</td><td>Planificación de eventos familiares</td><td>Como familiar quiero coordinar con el personal la organización de eventos especiales o celebraciones para mi familiar dentro de las instalaciones</td><td>
    Escenario 1: Coordinación exitosa de evento familiar
Dado un familiar planificando evento especial para su familiar
cuando solicita coordinación para celebración de cumpleaños, aniversario u ocasión especial
entonces puede especificar fecha, número de invitados, requerimientos especiales
y el personal evalúa viabilidad según protocolos institucionales
y se coordinan espacios, horarios y recursos necesarios
y recibe confirmación con detalles finales del evento
Escenario 2: Evento que no cumple con protocolos institucionales
Dado un familiar solicitando evento que no cumple protocolos
cuando la solicitud involucra aspectos no permitidos por políticas institucionales
entonces se explican las limitaciones y razones institucionales
y se ofrecen alternativas que cumplan con protocolos
y se proporcionan opciones modificadas para el evento
    </td><td>EP06</td>
  </tr>
   <tr>
    <td>US24</td><td>Registro de medicamentos en inventario</td><td>Como administrador quiero registrar todos los medicamentos que ingresan al inventario con sus datos completos para mantener un catálogo actualizado</td><td>
    Escenario 1: Registro exitoso de medicamentos
Dado un administrador en el módulo de inventario de medicamentos
cuando registra nuevo medicamento con todos los datos requeridos (nombre, laboratorio, lote, fecha de vencimiento, cantidad)
entonces el medicamento se añade correctamente al inventario
y se genera código de identificación único
y se actualiza el stock total disponible
y el sistema registra fecha y responsable del ingreso
Escenario 2: Medicamento duplicado en inventario
Dado un administrador registrando medicamento
cuando intenta ingresar un medicamento que ya existe con el mismo lote
entonces el sistema detecta la duplicación y muestra alerta
y permite actualizar cantidad del lote existente en lugar de crear duplicado
y mantiene integridad de datos en el inventario
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US25</td><td>Alertas de vencimiento</td><td>Como administrador quiero recibir alertas automáticas sobre medicamentos próximos a vencer para evitar pérdidas y riesgos de seguridad</td><td>
    Escenario 1: Alert generation for expiring medications
Dado medicamentos en inventario próximos a vencer
cuando faltan 30 días para fecha de vencimiento
entonces se genera alerta automática al administrador de farmacia
y la alerta incluye lista de medicamentos, cantidades y fechas exactas
y se sugieren acciones como uso prioritario o devolución a proveedor
y se programa seguimiento semanal hasta resolución
Escenario 2: Medicamentos ya vencidos en inventario
Dado medicamentos que han superado su fecha de vencimiento
cuando el sistema detecta medicamentos vencidos
entonces se bloquea automáticamente su uso en el sistema
y se genera alerta crítica para remoción inmediata
y se registra como pérdida en reportes de inventario
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US26</td><td>Eliminación de medicamentos</td><td>Como administrador quiero eliminar medicamentos del inventario de manera controlada para mantener la precisión del stock y cumplir con protocolos de disposición</td><td>
    Escenario 1: Eliminación controlada de medicamento
Dado un administrador necesitando eliminar medicamento del inventario
cuando selecciona medicamento y especifica razón (vencido, dañado, usado)
entonces debe proporcionar justificación y autorización apropiada
y el sistema registra la eliminación con fecha, cantidad y responsable
y se actualiza automáticamente el stock disponible
y se genera reporte de eliminación para auditoría
Escenario 2: Intento de eliminación sin autorización
Dado un usuario intentando eliminar medicamento sin permisos suficientes
cuando no posee los permisos necesarios para eliminación
entonces el sistema niega el acceso con mensaje explicativo
y se registra el intento en logs de seguridad
y se notifica al administrador sobre el intento no autorizado
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US27</td><td>Búsqueda y filtrado de inventario</td><td>Como administrador quiero filtrar y buscar medicamentos en el inventario para encontrar rápidamente información específica y generar reportes personalizados</td><td>
    Escenario 1: Búsqueda exitosa de medicamentos
Dado un administrador en el módulo de inventario
cuando utiliza filtros de búsqueda por nombre, laboratorio, fecha de vencimiento o categoría
entonces obtiene resultados precisos que coinciden con los criterios
y puede ordenar resultados por diferentes campos
y puede exportar los resultados filtrados para reportes
y la búsqueda es rápida y eficiente
Escenario 2: Búsqueda sin resultados
Dado un administrador buscando medicamento específico
cuando los criterios de búsqueda no coinciden con ningún medicamento en inventario
entonces se muestra mensaje claro de "sin resultados"
y se sugieren búsquedas alternativas o similares
y puede contactar a proveedores para disponibilidad
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US28</td><td>Información de medicamentos para personal</td><td>Como administrador quiero proporcionar información detallada sobre medicamentos al personal para asegurar administración segura y correcta</td><td>
    Escenario 1: Acceso exitoso a información detallada de medicamentos
Dado personal autorizado consultando información de medicamento
cuando accede a detalles de medicamento específico
entonces puede ver información completa: dosificación, contraindicaciones, efectos secundarios, interacciones
y la información está actualizada y es confiable
y puede acceder a protocolos de administración específicos
y tiene enlaces a recursos adicionales si necesita más información
Escenario 2: Medicamento con alertas especiales
Dado personal consultando medicamento con requerimientos especiales
cuando el medicamento tiene alertas de seguridad o administración especial
entonces se muestran prominentemente todas las alertas y precauciones
y se requiere confirmación de lectura antes de proceder
y se proporcionan protocolos específicos de manejo
    </td><td>EP07</td>
  </tr>
   <tr>
    <td>US29</td><td>Gestión de perfiles de empleados</td><td>Como administrador quiero registrar y mantener los perfiles completos del personal para tener información actualizada de todos los empleados.</td><td>
    Escenario 1: Registro exitoso de empleado
    Dado un administrador de RRHH registrando nuevo empleado
cuando completa información personal, profesional, contactos de emergencia y rol asignado
entonces el perfil se crea exitosamente en el sistema
y se genera ID de empleado único
y se asignan permisos según el rol especificado
y el empleado recibe credenciales de acceso al sistema
Escenario 2: Información incompleta de empleado
Dado un administrador registrando empleado con información faltante
cuando faltan datos críticos como certificaciones requeridas o contactos de emergencia
entonces el sistema indica específicamente qué información falta
y permite guardar como borrador para completar posteriormente
y no activa permisos hasta que toda la información requerida esté completa
    </td><td>EP08</td>
  </tr>
   <tr>
    <td>US30</td><td>Baja de personal</td><td>Como administrador quiero dar de baja empleados del sistema para mantener registros actualizados y gestionar finalizaciones de contratos.</td><td>
    Escenario 1: Proceso exitoso de baja de empleado
Dado un administrador procesando baja de empleado
cuando especifica fecha de terminación, motivo y procedimientos de entrega
entonces se desactivan automáticamente todos los accesos al sistema
y se genera reporte de finalización con tareas pendientes
y se actualiza la estructura organizacional
y se notifica a supervisores y equipos afectados
Escenario 2: Empleado con responsabilidades activas
Dado un administrador intentando dar de baja empleado con responsabilidades activas
cuando el empleado tiene residentes asignados o tareas críticas pendientes
entonces el sistema alerta sobre responsabilidades que requieren reasignación
y proporciona lista de tareas y residentes que deben transferirse
y requiere reasignación completa antes de procesar la baja
</td><td>EP08</td>
  </tr>
  <tr>
    <td>US31</td><td>Búsqueda y filtrado de empleados</td><td>Como administrador quiero filtrar y buscar empleados según diferentes criterios para encontrar rápidamente personal específico.</td><td>
    Escenario 1: Búsqueda exitosa de empleados
Dado un administrador en el módulo de gestión de personal
cuando utiliza filtros por departamento, rol, turno, o estado de empleo
entonces obtiene lista precisa de empleados que coinciden con criterios
y puede ver información básica de cada empleado en los resultados
y puede acceder a perfiles completos desde los resultados
y puede exportar la lista filtrada para reportes
Escenario 2: Filtros que no retornan resultados
Dado un administrador aplicando filtros específicos
cuando la combinación de filtros no coincide con ningún empleado
entonces se muestra mensaje claro indicando ausencia de resultados
y se sugiere modificar criterios de búsqueda
y se mantienen los filtros aplicados para fácil modificación
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US32</td><td>Gestión de horas extra</td><td>Como administrador quiero controlar las horas extra trabajadas por el personal para gestionar costos laborales y cumplir con regulaciones de trabajo</td><td>
    Escenario 1: Registro exitoso de horas extra
Dado un administrador registrando horas extra de empleado
cuando especifica empleado, fecha, horas trabajadas y justificación
entonces las horas se registran correctamente en el sistema
y se calculan automáticamente los montos según tarifas establecidas
y se actualiza el reporte mensual de horas extra
y se notifica al empleado sobre el registro
Escenario 2: Horas extra que exceden límites permitidos
Dado un administrador registrando horas extra que exceden límites legales
cuando las horas superan los máximos permitidos por regulaciones laborales
entonces el sistema muestra alerta sobre violación de límites
y requiere autorización especial y justificación
y se genera reporte para revisión de RRHH
    </td><td>EP08</td>
  </tr>
  <tr>
  <tr>
    <td>US33</td><td>Gestión de horarios de atención</td><td>Como administrador quiero configurar los horarios de atención y servicios para informar claramente a familias sobre disponibilidad</td><td>
    Escenario 1: Configuración exitosa de horarios
Dado un administrador configurando horarios de atención
cuando establece horarios por servicio, día de semana y disponibilidad de personal
entonces los horarios se actualizan en toda la plataforma
y las familias pueden ver horarios actualizados al programar visitas o servicios
y se generan calendarios de disponibilidad automáticamente
y se sincroniza con sistemas de programación de citas
Escenario 2: Cambio de horarios por emergencia
Dado un administrador modificando horarios por situación de emergencia
cuando debe cambiar horarios por situaciones imprevistas
entonces puede realizar cambios inmediatos con notificación automática
y todas las partes afectadas reciben notificación instantánea
y se reprograman automáticamente citas afectadas
</td><td>EP09</td>
  </tr>
  <tr>
    <td>US34</td><td>Datos de contacto institucional</td><td>Como administrador quiero gestionar la información de contacto de la casa de reposo para que familias y autoridades tengan acceso a datos actualizados</td><td>
    Escenario 1: Actualización exitosa de información de contacto
Dado un administrador actualizando datos de contacto institucional
cuando modifica teléfonos, emails, dirección o personas de contacto
entonces la información se actualiza inmediatamente en toda la plataforma
y se refleja en landing page, aplicaciones y documentos oficiales
y se notifica automáticamente a familias sobre cambios importantes
y se mantiene historial de cambios para auditoría
Escenario 2: Información de contacto de emergencia
Dado una situación que requiere contacto de emergencia
cuando familias necesitan contactar urgentemente a la institución
entonces tienen acceso inmediato a números de emergencia 24/7
y pueden identificar fácilmente el contacto apropiado según la situación
y reciben respuesta rápida según protocolos de emergencia
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US35</td><td>Información del personal directivo</td><td>Como administrador quiero gestionar la información del personal directivo para transparencia hacia familias y autoridades</td><td>Escenario 1: Gestión de información de personal directivo
Dado un administrador actualizando información de personal directivo
cuando modifica información de directores, coordinadores y personal clave
entonces la información se presenta profesionalmente a familias y autoridades
y incluye credenciales, experiencia y áreas de responsabilidad
y se actualiza automáticamente en materiales institucionales
y mantiene información siempre actualizada y verificable
Escenario 2: Acceso a información directiva por autoridades
Dado autoridades sanitarias requiriendo información del personal directivo
cuando necesitan verificar credenciales y responsabilidades del personal clave
entonces pueden acceder a información completa y actualizada
y toda la documentación está organizada y es fácilmente verificable
y se proporciona información de contacto directo cuando es apropiado
</td><td>EP09</td>
  </tr>
  <tr>
    <td>US36</td><td>Historia institucional</td><td>Como administrador quiero gestionar la información histórica y reconocimientos de la casa de reposo para generar confianza y credibilidad</td><td>
    Escenario 1: Presentación de historia y reconocimientos institucionales
Dado un administrador gestionando información histórica institucional
cuando actualiza historia, reconocimientos, certificaciones y logros
entonces la información se presenta de manera atractiva y creíble
y incluye certificaciones vigentes y reconocimientos oficiales
y genera confianza en familias evaluando los servicios
y es fácilmente accesible para consulta de interesados
Escenario 2: Verificación de certificaciones por autoridades
Dado autoridades verificando certificaciones institucionales
cuando requieren confirmar validez de licencias y reconocimientos
entonces pueden acceder a información verificable y actualizada
y todos los documentos incluyen números de registro y fechas de vigencia
y se proporciona contacto directo con entidades certificadoras
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US37</td><td>Gestión de usuarios y permisos</td><td>Como administrador quiero saber quién tiene acceso al sistema y qué información puede ver cada usuario para proteger la privacidad de los datos</td><td>
    Escenario 1: Configuración exitosa de permisos de usuario
Dado un administrador de sistema gestionando accesos
cuando asigna roles y permisos específicos a usuarios (familiares, personal, administradores)
entonces cada usuario accede únicamente a información autorizada para su rol
y los permisos se aplican consistentemente en toda la plataforma
y se registra toda actividad de acceso para auditoría
y se pueden modificar permisos sin afectar otros aspectos del sistema
Escenario 2: Intento de acceso no autorizado
Dado un usuario intentando acceder a información fuera de sus permisos
cuando intenta acceder a datos que no le corresponden según su rol
entonces el sistema bloquea el acceso inmediatamente
y registra el intento en logs de seguridad
y notifica al administrador sobre el intento no autorizado
y proporciona mensaje claro sobre restricciones de acceso
</td><td>EP10</td>
  </tr>
  <tr>
    <td>US38</td><td>Protección de datos mediante cifrado</td><td>Como administrador quiero que toda la información sensible esté cifrada para proteger los datos personales y médicos de accesos no autorizados</td><td>
    Escenario 1: Cifrado exitoso de datos sensibles
Dado el sistema almacenando información personal y médica
cuando se guardan datos sensibles de residentes y familias
entonces toda la información se cifra automáticamente antes del almacenamiento
y las comunicaciones entre usuario y servidor están cifradas
y solo usuarios autorizados pueden descifrar información específica
y se mantienen estándares de seguridad médica requeridos
Escenario 2: Intento de acceso a datos cifrados sin autorización
Dado un intento de acceso directo a datos cifrados
cuando alguien intenta acceder a información sin autorización apropiada
entonces los datos permanecen completamente inaccesibles
y se registra el intento de acceso no autorizado
y se activan alertas de seguridad automáticas
y se notifica inmediatamente al equipo de seguridad
    </td><td>EP10</td>
  </tr>
  <tr>
    <td>US39</td><td>Terminos y condiciones</td><td>Como visitante de la landing page quiero poder acceder a los términos y condiciones de uso para conocer las políticas legales antes de contratar los servicios</td><td>
    Escenario 1: Acceso exitoso a términos y condiciones
Dado un visitante en la landing page
cuando busca información legal sobre términos y condiciones de uso
entonces puede acceder fácilmente a documento completo desde footer o header
y los términos están redactados claramente y son comprensibles
y incluyen políticas de privacidad, uso de datos y responsabilidades
y están actualizados con fecha de última modificación
Escenario 2: Aceptación requerida de términos actualizados
Dado términos y condiciones que han sido actualizados
cuando un usuario existente ingresa al sistema después de la actualización
entonces debe revisar y aceptar los nuevos términos antes de continuar
y se destacan claramente los cambios realizados
y puede comparar versión anterior si lo desea
    </td><td>EP01</td>
  </tr>
   <tr>
    <td>US40</td><td>Menú de navegación consistente</td><td>Como usuario quiero un menú de navegación claro y consistente en todas las páginas para encontrar fácilmente las funciones que necesito</td><td>
    Escenario 1: Navegación consistente en toda la plataforma
Dado un usuario en cualquier página de la aplicación
cuando utiliza el menú de navegación
entonces encuentra las mismas opciones organizadas de manera idéntica
y puede acceder a funciones principales desde cualquier página
y el menú se adapta apropiadamente a diferentes tamaños de pantalla
y indica claramente la ubicación actual del usuario
Escenario 2: Menú adaptado a permisos de usuario
Dado usuarios con diferentes roles accediendo al sistema
cuando navegan por la plataforma
entonces ven solo opciones de menú apropiadas para su rol
y las opciones restringidas no aparecen para evitar confusión
y pueden identificar fácilmente todas las funciones disponibles para ellos
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US41</td><td>Paleta de colores y tipografía</td><td>Como usuario quiero una interfaz con colores y tipografía consistentes para tener una experiencia visual agradable y fácil de leer</td><td>
    Escenario 1: Aplicación consistente de diseño visual
Dado cualquier página de la plataforma Veyra
cuando un usuario navega por diferentes secciones
entonces encuentra colores y tipografía consistentes en toda la experiencia
y el diseño refleja profesionalismo apropiado para servicios de salud
y el contraste de colores cumple estándares de accesibilidad
y la tipografía es legible en diferentes dispositivos y tamaños
Escenario 2: Adaptación para usuarios con necesidades especiales
Dado usuarios con dificultades visuales
cuando acceden a la plataforma
entonces pueden utilizar funciones de alto contraste o aumento de texto
y todos los elementos mantienen legibilidad en diferentes configuraciones
y los colores no son el único medio para transmitir información importante
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US42</td><td>Diseño de formularios usables</td><td>Como usuario quiero formularios claros y fáciles de completar para ingresar información sin confusión ni errores</td><td>
    Escenario 1: Completar formularios de manera eficiente
Dado un usuario completando cualquier formulario en la plataforma
cuando ingresa información requerida
entonces los campos están claramente etiquetados y organizados lógicamente
y recibe validación en tiempo real para campos incorrectos
y puede guardar progreso para completar posteriormente si es formulario largo
y recibe confirmación clara al completar exitosamente
Escenario 2: Formulario con errores de validación
Dado un usuario enviando formulario con información incorrecta
cuando existen errores en los datos ingresados
entonces recibe mensajes de error específicos y constructivos
y se mantiene toda la información correcta ya ingresada
y puede corregir errores fácilmente sin empezar desde cero
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US43</td><td>Patrones de diseño coherentes</td><td>Como usuario quiero que todas las pantallas sigan patrones de diseño similares para predecir dónde encontrar funciones y cómo interactuar</td><td>
    Escenario 1: Interacción predecible en toda la plataforma
Dado un usuario familiarizado con una sección de la plataforma
cuando navega a nuevas secciones
entonces encuentra patrones de interacción similares y predecibles
y botones, enlaces y controles funcionan de manera consistente
y puede aplicar conocimiento previo para usar nuevas funcionalidades
y la experiencia se siente uniforme y profesional
Escenario 2: Nuevos usuarios aprendiendo la interfaz
Dado un nuevo usuario accediendo por primera vez
cuando explora diferentes funcionalidades
entonces puede predecir cómo funcionarán nuevas secciones basándose en experiencia previa
y encuentra elementos de interfaz en ubicaciones esperadas
y puede desarrollar eficiencia rápidamente en el uso del sistema
    </td><td>EP11</td>
  </tr>
   <tr>
    <td>US44</td><td>Manejo de errores comprensible</td><td>Como usuario quiero que los errores se presenten de forma clara y con soluciones sugeridas para resolver problemas sin frustración</td><td>
    Escenario 1: Error del sistema con guía de resolución
Dado un error técnico durante el uso de la plataforma
cuando ocurre un problema de sistema o conectividad
entonces el usuario recibe mensaje claro explicando qué ocurrió
y se proporcionan pasos específicos para resolver el problema
y se ofrecen alternativas de contacto si el problema persiste
y se registra el error para mejora continua del sistema
Escenario 2: Error de usuario con orientación educativa
Dado un usuario cometiendo error en el uso de la plataforma
cuando realiza una acción incorrecta o no permitida
entonces recibe explicación clara sobre por qué no se pudo completar la acción
y se le orienta sobre la forma correcta de proceder
y puede corregir fácilmente su acción sin frustración
y aprende a evitar el mismo error en el futuro
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
    Escenario 1: Eliminación exitosa
Dado un administrador autenticado con permisos y un medicamentoId existente
cuando envía DELETE /medicamentos/{medicamentoId}
entonces el servicio responde 204 No Content, el registro queda  como eliminado  y se muestra 
que se borro en la base de datos .

Escenario 2: Eliminación fallida por inexistencia o falta de permisos
Dado un usuario sin permisos o un medicamentoId inexistente
cuando intenta DELETE /medicamentos/{medicamentoId}
entonces el servicio responde 403 si no tiene permisos, o 404 Not Found si el id no existe, y el intento queda registrado en logs.
    </td>
  </tr>
  <tr>
    <td>TS02</td><td>Agregar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Post  medicamentos  para permitir que el administrador de la casa de reposo pueda agregar más medicamentos. </td><td>
    Escenario 1: Creación exitosa
Dado un administrador autenticado y un registro de datos válido en los campos obligatorios (nombre, lote, fechaVencimiento, cantidad)
cuando envía POST /medicamentos
entonces el servicio responde 201 Created  y el medicamento queda persistido en base de datos.

Escenario 2: Error de validación o duplicado
Dado un registro con campos faltantes o que coincide con un medicamento existente.
cuando envía POST /medicamentos
entonces el servicio responde 400 Bad Request para validaciones o 409 Conflict si es duplicado, con mensajes de error detallados.
    </td>
  </tr>
  <tr>
    <td>TS03</td><td>Ver información detallada de los medicamentos</td><td>Como desarrollador backend en NovaPeru Tech quiero crear una función para ver la información a través de una Api para que </td><td>
    Escenario 1: Consulta exitosa
Dado un usuario autenticado y autorizado y un medicamentoId válido
cuando solicita GET /medicamentos/{medicamentoId}
entonces el servicio responde 200 OK con el JSON .
Escenario 2: Recurso no encontrado o sin permisos
Dado un medicamentoId inexistente o un usuario sin autorización
cuando solicita GET /medicamentos/{medicamentoId}
entonces el servicio responde 404 Not Found si no existe.
    </td>
  </tr>
  <tr>
    <td>TS04</td><td>Actualizar información de medicamentos</td><td>Como desarrollador de backend en NovaPeru Tech quiero crear una función para actualizar la información para asegurar que el administrador de la casa de reposos pueda mantener actualizada la inforción de cada medicamento</td><td>
    Escenario 1: Actualización exitosa con control de concurrencia
Dado un usuario autorizado y un medicamentoId existente y registro de datos válido
cuando envía PUT/PATCH /medicamentos/{medicamentoId}
entonces el servicio responde 200 OK, aplica los cambios, registra la modificación en la base de datos.

Escenario 2: Conflicto o validación fallida
Dado registro de la nueva información no es valida .
cuando intenta PUT/PATCH /medicamentos/{medicamentoId}
entonces el servicio responde  400 Bad Request para datos inválidos.
    </td>
  </tr>
  <tr>
    <td>TS05</td><td>Agregar pacientes</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para permitir que el administrador registre nuevos residentes con validaciones obligatorias y que se genere un ID único por residente.</td><td>
    Escenario 1: Registro exitoso de residente
Dado administrador autenticado y ingresa  datos válidos
cuando envía POST /residents
entonces el servicio responde 201 Created, retorna residentId y persiste el registro en la base de datos.

Escenario 2: Duplicado o campos faltantes
Dado un registro con documento de identidad ya registrado o campos obligatorios faltantes
cuando envía POST /residents
entonces el servicio responde 400 Bad Request si faltan datos, con detalles de error.
    </td>
  </tr>
  <tr>
    <td>TS06</td><td>Ver información detallada  de los pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET  que devuelva la información completa del residente para que el personal autorizado pueda consultar fácilmente el expediente.</td><td>
    Escenario 1: Consulta autorizada
Dado personal autorizado  y residentId válido
cuando solicita GET /residents/{residentId}
entonces recibe 200 OK con datos personales, contactos autorizados y resumen del historial médico.

Escenario 2: Sin permisos o recurso inexistente
Dado usuario sin permisos para ver datos médicos o residentId no existente
cuando solicita GET /residents/{residentId}
entonces el servicio responde  404 Not Found si el residente no existe.
    </td>
  </tr>
  <tr>
    <td>TS07</td><td>Eliminar paciente  </td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE  que realice una eliminación controlada  del residente.
    </td><td>
    Escenario 1: Baja controlada exitosa
Dado administrador autenticado 
cuando envía DELETE /residents/{residentId}
entonces el sistema marca inactive, revoca accesos asociados.

Escenario 2: Eliminación fallida
Dado Administrador con responsabilidades activas
cuando intenta DELETE /residents/{residentId}
entonces el servicio responde 409 Conflict y devuelve lista de acciones requeridas para completar la eliminación.
    </td>
  </tr>
  <tr>
    <td>TS08</td><td>Actualizar información de los pacientes </td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH  para actualizar campos del perfil del residente para que las modificaciones queden registradas y sean reversibles si es necesario</td><td>
    Escenario 1: Actualización válida y registrada
Dado Administrador  autorizado y registro de datos permitidos  correcto
cuando envía PATCH /residents/{residentId}
entonces el servicio responde 200 OK, aplica los cambios permitidos y guarda un registro de auditoría con diff de cambios.

Escenario 2: Intento de modificar campos restringidos o datos inválidos
Dado registro de datos  que incluye campos de solo lectura o formato inválido
cuando envía PATCH /residents/{residentId}
entonces el servicio responde 400 Bad Request para validaciones, sin aplicar cambios.
    </td>
  </tr>
  <tr>
    <td>TS09</td><td>Agregar información detallada de la casa de reposo</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que un administrador pueda registrar información institucional .
    </td><td>
    Escenario 1: Creación de información institucional exitosa
Dado administrador autenticado y registro de datos  válido 
cuando envía POST /institution-info
entonces el servicio responde 201 Created y los datos quedan disponibles  en la app.

Escenario 2: Error por falta de permisos o validación
Dado usuario no administrador o registro de datos obligatorios faltantes
cuando envía POST /institution-info
entonces el servicio responde  400 Bad Request si faltan campos.
    </td>
  </tr>
  <tr>
    <td>TS010</td><td>Actualizar información de la casa de reposo</td><td>
    Como desarrollador backend en NovaPeru tech quiero crear un endpoint PUT para mantener actualizados los datos institucionales.
    </td><td>
    Escenario 1: Actualización exitosa y auditada
Dado administrador autenticado, payload válido y versión coincidente
cuando envía PUT/PATCH /institution-info/{id}
entonces el servicio responde 200 OK, actualiza los datos y registra quien y cuándo realizó el cambio.

Escenario 2: Conflicto de versión o datos inválidos
Dado versión desincronizada o registro de datos inválido
cuando intenta PUT/PATCH /institution-info/{id}
entonces el servicio responde 400 Bad Request por validación.
    </td>
  </tr>
  <tr>
    <td>TS011</td><td>Agregar empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que registre nuevos empleados.</td><td>
    Escenario 1: Registro de empleado exitoso
Dado Administrador autenticado y registro de datos válido 
cuando envía POST /employees
entonces el servicio responde 201 Created, devuelve employeeId, asigna permisos iniciales y crea credenciales seguras.

Escenario 2: Error por email/ID duplicado o validación
Dado email o documento ya registrado o campos inválidos
cuando envía POST /employees
entonces el servicio responde 409 Conflict para duplicados o 400 Bad Request para validaciones.
    </td>
  </tr>
  <tr>
    <td>TS012</td><td>Eliminar empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE para que el administrador de la casa de reposo revoque persmisos. 
    </td><td>
    Escenario 1: Baja controlada exitosa
Dado administrador autenticado y empleado sin tareas críticas pendientes
cuando envía DELETE /employees/{employeeId}
entonces el servicio elmina empleado , registra la acción en base de datos.

Escenario 2: Baja bloqueada por responsabilidades activas o sin permisos
Dado empleado con residentes/tareas asignadas o petición desde usuario sin permisos
cuando intenta DELETE /employees/{employeeId}
entonces el servicio responde 409 Conflict indicando reasignaciones requeridas, o 403 Forbidden si el solicitante no está autorizado.
    </td>
  </tr>
  <tr>
    <td>TS013</td><td>Actualizar información del empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar datos de empleado.
    </td><td>
    Escenario 1: Actualización válida con auditoría
Dado Administrador  autenticado y registra datos  válido
cuando envía PATCH /employees/{employeeId}
entonces el servicio responde 200 OK y registra el cambio en la base de datos.

Escenario 2: Intento de actualizar datos inválidos
Dado intento de registrar datos  inválido
cuando envía PATCH /employees/{employeeId}
entonces el servicio responde 400 Bad Request para datos inválidos.
    </td>
  </tr>
  <tr>
    <td>TS014</td><td>Ver información del empleado</td><td>
    Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET que muestre el perfil del empleado para que el administrador pueda observar cuantos empleados tiene.
    </td><td>
    Escenario 1: Consulta autorizada del perfil
Dado usuario autorizado  y employeeId válido
cuando solicita GET /employees/{employeeId}
entonces el servicio responde 200 OK , se filtran según permisos.

Escenario 2: empleado no existe
Dado  employeeId inexistente
cuando solicita GET /employees/{employeeId}
entonces el servicio responde  404 Not Found si no existe.
    </td>
  </tr>
  <tr>
    <td>TS015</td><td>Consumir Api de Medicamentos</td><td>
    Como desarrollador backend en NovaPeru tech quiero consumir la API externa de medicamentos mediante un servicio de integración , para disponer de información confiable y actualizada de medicamentos en el sistema.
    </td><td>
    Escenario 1: Sincronización exitosa y segura
Dado credenciales válidas para la API externa y conectividad estable
cuando se ejecuta sincronización programada o petición 
entonces los datos externos se mapean y normalizan al modelo interno, se guardan cambios.

Escenario 2: Fallo externo
Dado timeout en la API externa o respuesta que no cumple el esquema esperado
cuando intenta sincronizar
entonces el servicio  registra la incidencia en logs y no sobrescribe datos locales hasta validación.
    </td>
  </tr>
  <tr>
    <td>TS016</td><td>Consumir Api de google maps</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de integración con Google Maps que proporcione  verificación de direcciones y datos de localización para manejar errores.</td><td>
    Escenario 1: Geocoding verificado vía proxy
Dado API key protegida en backend y request válido (dirección)
cuando solicita geocoding a través del proxy GET /maps/proxy?address=...
entonces el proxy devuelve datos normalizados (lat/lng, formato) y la API key no se expone al frontend.

Escenario 2: Rate limit o error del proveedor
Dado Google Maps devuelve 429 o falla por timeout
cuando realiza la petición al proxy
entonces el proxy responde 429 o 503 con mensaje controlado, aplica política de backoff y utiliza cache fallback si existe.
    </td>
  </tr>
  <tr>
    <td>TS017</td><td>Nofitifación de visitas</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de notificaciones para enviar recordatorios y alertas de visitas vía email/SMS</td><td>
    Escenario 1: Envío de recordatorio exitoso
Dado visita programada y contactos válidos con preferencias de notificación
cuando falta el tiempo configurado (p.ej. 2 horas) y la cola procesa el job
entonces se envía notificación vía canal configurado (email/SMS/push), el sistema registra el estado delivered y actualiza el registro de visita.

Escenario 2: Fallo en entrega y reintentos
Dado fallo de entrega
cuando el worker intenta enviar la notificación
entonces el sistema aplica reintentos configurados .
    </td>
  </tr>
  <tr>
    <td>TS018</td><td>Buscar y filtrar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET con parámetros de búsqueda  facilitar consultas rápidas y generación de reportes. </td><td>
    Escenario 1: Búsqueda paginada exitosa
Dado parámetros válidos 
cuando solicita GET /medicamentos
entonces el servicio responde 200 OK con lista .

Escenario 2: Parámetros inválidos o sin resultados
Dado parámetros inválidos  o criterio que no retorna matches
cuando solicita GET /medicamentos
entonces el servicio responde 400 Bad Request para parámetros inválidos o 200 OK con items: [] y totalItems: 0 si no hay resultados.
    </td>
  </tr>
  <tr>
    <td>TS019</td><td>BUsccar y filtrar residentes</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET con filtros para que administradores y personal autorizado encuentren residentes fácilmente.</td><td>
    Escenario 1: Consulta filtrada y autorizada
Dado filtros válidos  y usuario autorizado
cuando solicita GET /residents?nombre=X&habitacion=Y
entonces el servicio responde 200 OK con resultados paginados y campos conforme a permisos del solicitante.

Escenario 2: Intento sin permisos o parámetros inválidos
Dado usuario sin permiso para ver datos sensibles o parámetros mal formados
cuando solicita GET /residents?
entonces el servicio responde 400 Bad Request si los parámetros son inválidos.
    </td>
  </tr>
  <tr>
    <td>TS020</td><td>Buscar y filtrar empleados</td><td>
    Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que permita buscar y filtrar por nombre, rol, turno que se pueda exportar para que vea el reporte de empleados el admnistrador o RRHH.</td><td>
        Escenario 1: Búsqueda y exportación permitida
Dado parámetros válidos y usuarios con permiso de exportación
cuando solicita GET /employees?rol=cuidador&export=true
entonces el servicio responde 200 OK iniciando exportación (CSV) y devuelve enlace de descarga cuando esté listo.

Escenario 2: Exportación denegada o sin resultados
Dado  filtros que no arrojan resultados
cuando solicita GET /employees
entonces el servicio responde 400 si no coincide .
    </td>
  </tr>
</table>


## 3.2. Impact Mapping

<img src="../images/Impact map 1.png" alt="Impact map 1" width="auto" height="auto"/>

## 3.3. Product Backlog

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr>
    <td>Orden</td><td>User Story Id</td><td>Título</td><td>Descripción</td><td>Story Points (1/2/3/5/8)</td>
  </tr>
  <tr><td>1</td><td>US01</td><td>Menú de navegación</td><td>Permitir al visitante acceder a un menú en la parte superior de la página con enlaces a 'Log in', 'Sign up', 'Planes', 'Contacto', etc.</td><td>1</td></tr>
  <tr><td>2</td><td>US02</td><td>Visualización de Planes</td><td>Mostrar planes de suscripción con precio, características y duración, permitiendo compararlos fácilmente.</td><td>2</td></tr>
  <tr><td>3</td><td>US03</td><td>Selección de Plan en Landing Page</td><td>Permitir seleccionar un plan en la landing page y completar un formulario de confirmación en la misma pantalla.</td><td>3</td></tr>
  <tr><td>4</td><td>US04</td><td>Visualización de creadores</td><td>Mostrar información de los creadores del producto en la sección 'Sobre nosotros' con nombre, foto, rol y descripción.</td><td>2</td></tr>
  <tr><td>5</td><td>US05</td><td>Redes sociales</td><td>Incluir iconos/enlaces a las redes sociales de Veyra en el footer o header para que el usuario los abra en nuevas pestañas.</td><td>1</td></tr>
  <tr><td>6</td><td>US06</td><td>Formulario de contacto</td><td>Crear un formulario de contacto con campos (nombre, email, asunto, mensaje) que envíe consultas y muestre mensajes de validación.</td><td>3</td></tr>
  <tr><td>7</td><td>US07</td><td>Cambio de idioma</td><td>Agregar botón en el menú para alternar entre español e inglés, actualizando toda la interfaz al idioma seleccionado.</td><td>3</td></tr>
  <tr><td>8</td><td>US39</td><td>Términos y condiciones</td><td>Agregar acceso a un documento de términos y condiciones con políticas de uso y privacidad.</td><td>2</td></tr>
  <tr><td>9</td><td>US08</td><td>Historial médico</td><td>Permitir a un familiar autenticado acceder al historial médico del residente, mostrando diagnósticos, evolución .</td><td>5</td></tr>
  <tr><td>10</td><td>US09</td><td>Agenda de citas Médicas</td><td>Permitir a un familiar ver las citas médicas programadas de su familiar, con detalle de fecha, hora, médico .</td><td>5</td></tr>
  <tr><td>11</td><td>US10</td><td>Consulta de información personal</td><td>Mostrar al familiar la información personal actualizada del residente, permitiéndole solicitar modificaciones en caso de datos incorrectos.</td><td>3</td></tr>
  <tr><td>12</td><td>US11</td><td>Galería de fotos y actividades</td><td>Presentar al familiar una galería de fotos organizadas por fecha y tipo de actividad, con descripciones y opciones de filtrado.</td><td>3</td></tr>
  <tr><td>13</td><td>US12</td><td>Registro de residentes</td><td>Permitir a un administrador crear un perfil completo para cada residente (datos personales, médicos, contactos).</td><td>3</td></tr>
  <tr><td>14</td><td>US13</td><td>Historial médico institucional</td><td>Permitir a un administrador con permisos médicos ver y editar el historial médico completo del residente, registrar diagnósticos y generar reportes.</td><td>8</td></tr>
  <tr><td>15</td><td>US14</td><td>Administración de medicamentos</td><td>Implementar gestión de administración de medicamentos para llevar un mayor control.</td><td>5</td></tr>
  <tr><td>16</td><td>US15</td><td>Gestión de visitas familiares</td><td>Permitir a un administrador programar visitas familiares asignando fecha, hora, visitantes y residente, con verificación de disponibilidad.</td><td>5</td></tr>
  <tr><td>17</td><td>US16</td><td>Recordatorios de citas y consultas</td><td>Enviar recordatorios automáticos a familiares antes de las citas médicas programadas.</td><td>3</td></tr>
  <tr><td>18</td><td>US17</td><td>Notificaciones de cambios en medicación</td><td>Enviar notificación inmediata a familiares autorizados cuando se actualice la medicación de un residente, incluyendo detalles del cambio.</td><td>3</td></tr>
  <tr><td>19</td><td>US18</td><td>Recordatorios de visitas familiares</td><td>Enviar recordatorios automáticos a familiares 2 horas antes de visitas programadas, con confirmación o cancelación anticipada.</td><td>3</td></tr>
  <tr><td>20</td><td>US19</td><td>Alertas de actualización de datos personales</td><td>Notificar automáticamente a familiares autorizados cuando se actualice la información personal del residente, detallando los cambios.</td><td>3</td></tr>
  <tr><td>21</td><td>US20</td><td>Preguntas sobre rutina de cuidados</td><td>Permitir a un familiar enviar preguntas específicas sobre la rutina de cuidados del residente al personal asignado, con seguimiento del estado.</td><td>3</td></tr>
  <tr><td>22</td><td>US21</td><td>Peticiones de modificación de cuidados</td><td>Permitir a un familiar solicitar ajustes en el cuidado del residente, registrando la petición con seguimiento y notificación al equipo responsable.</td><td>3</td></tr>
  <tr><td>23</td><td>US22</td><td>Seguimiento del bienestar emocional</td><td>Permitir a un familiar cunicarse con la casa de reposo sobre el estado emocional del residente.</td><td>3</td></tr>
  <tr><td>24</td><td>US23</td><td>Planificación de eventos familiares</td><td>Permitir a un familiar coordinar eventos especiales para el residente (cumpleaños, aniversarios) indicando detalles, y gestionar según protocolos institucionales.</td><td>5</td></tr>
  <tr><td>25</td><td>US24</td><td>Registro de medicamentos en inventario</td><td>Permitir a un administrador registrar nuevos medicamentos en el inventario con información .</td><td>3</td></tr>
  <tr><td>26</td><td>US25</td><td>Alertas de vencimiento</td><td>Generar alertas automáticas para el administrador de farmacia cuando medicamentos en inventario estén próximos a vencer (30 días) o ya vencidos.</td><td>3</td></tr>
  <tr><td>27</td><td>US26</td><td>Eliminación de medicamentos</td><td>Permitir a un administrador eliminar medicamentos del inventario
    y saliendo un mensaje de eliminado correctamente.</td><td>3</td></tr>
  <tr><td>28</td><td>US27</td><td>Búsqueda y filtrado de inventario</td><td>Permitir al administrador buscar y filtrar medicamentos en el inventario por nombre, laboratorio, fecha de vencimiento o categoría.</td><td>3</td></tr>
  <tr><td>29</td><td>US28</td><td>Información de medicamentos para personal</td><td>Permitir al personal autorizado consultar información detallada de cada medicamento .</td><td>3</td></tr>
  <tr><td>30</td><td>US29</td><td>Gestión de perfiles de empleados</td><td>Permitir al administrador registrar y mantener perfiles completos de empleados, con datos personales, profesionales, contactos de emergencia y roles.</td><td>3</td></tr>
  <tr><td>31</td><td>US30</td><td>Baja de personal</td><td>Permitir al administrador procesar la baja de un empleado.</td><td>3</td></tr>
  <tr><td>32</td><td>US31</td><td>Búsqueda y filtrado de empleados</td><td>Permitir al administrador buscar y filtrar empleados según criterios (departamento, rol, estado), mostrando resultados precisos.</td><td>3</td></tr>
  <tr><td>33</td><td>US32</td><td>Gestión de horas extra</td><td>Permitir al administrador registrar horas extra de empleados y validando no superar el limite legal.</td><td>3</td></tr>
  <tr><td>34</td><td>US33</td><td>Gestión de horarios de atención</td><td>Permitir al administrador configurar los horarios de atención por servicio y día, sincronizando con citas programadas y notificando cambios urgentes.</td><td>3</td></tr>
  <tr><td>35</td><td>US34</td><td>Datos de contacto institucional</td><td>Permitir al administrador actualizar la información de contacto institucional (teléfono, email, dirección), reflejando cambios en la plataforma inmediatamente.</td><td>2</td></tr>
  <tr><td>36</td><td>US35</td><td>Información del personal directivo</td><td>Permitir al administrador gestionar la información del personal directivo.</td><td>2</td></tr>
  <tr><td>37</td><td>US36</td><td>Historia institucional</td><td>Permitir al administrador actualizar la historia, reconocimientos y certificaciones de la institución, presentando la información de forma creíble y consultable.</td><td>2</td></tr>
  <tr><td>38</td><td>US37</td><td>Gestión de usuarios y permisos</td><td>Permitir al administrador configurar roles y permisos de acceso para usuarios, asegurando que cada uno vea solo lo que corresponde a su rol.</td><td>5</td></tr>
  <tr><td>39</td><td>US38</td><td>Protección de datos mediante cifrado</td><td>Implementar cifrado automático de datos sensibles almacenados y en tránsito, garantizando que solo usuarios autorizados puedan descifrarlos.</td><td>5</td></tr>
  <tr><td>40</td><td>US40</td><td>Menú de navegación consistente</td><td>Asegurar que el menú de navegación sea claro y consistente en todas las páginas, adaptándose a permisos de usuario y dispositivos.</td><td>2</td></tr>
  <tr><td>41</td><td>US41</td><td>Paleta de colores y tipografía</td><td>Aplicar una paleta de colores y tipografía consistente y accesible en toda la interfaz, con opciones de alto contraste para usuarios con dificultades visuales.</td><td>2</td></tr>
  <tr><td>42</td><td>US42</td><td>Diseño de formularios usables</td><td>Diseñar formularios con campos bien etiquetados, validación en tiempo real y opción de guardar progreso, con mensajes claros de éxito o error.</td><td>3</td></tr>
  <tr><td>43</td><td>US43</td><td>Patrones de diseño coherentes</td><td>Garantizar que todas las pantallas compartan patrones de diseño similares (botones, controles), para que los usuarios encuentren las funciones donde esperan.</td><td>2</td></tr>
  <tr><td>44</td><td>US44</td><td>Manejo de errores comprensible</td><td>Mostrar errores del sistema o del usuario de forma clara y educativa, sugiriendo pasos para solucionar problemas y evitando frustraciones.</td><td>3</td></tr>
</table>
