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
    <td>US01</td><td>Menú de navegación</td><td>Como visitante de la Landing Page, quiero poder acceder a un menú de navegación en la parte superior de la página, para  explorar fácilmente las  secciones como "Log in", "Sign up", "Planes",  "Contacto",etc.</td><td>
   <strong>Escenario 1: Menú visible y navegable</strong> <br>
   <strong>Dado que</strong> el visitante se encuentra en la landing page, <br>
   <strong>Cuando</strong> la página carga por completo, <br>
   <strong>Y</strong> el visitante selecciona un enlace del menú, <br>
   <strong>Entonces</strong> el menú debe mostrarse en la parte superior con los enlaces principales ("Log in", "Sign up", "Planes", "Contacto"), <br>
    <strong>Y</strong> el visitante es redirigido correctamente a la sección correspondiente sin errores. <br><br>

  <strong>Escenario 2: Menú no carga o enlace roto</strong> <br>
    <strong>Dado que</strong> el visitante se encuentra en la landing page, <br>
    <strong>Cuando</strong> el menú no se visualiza correctamente o al intentar acceder a un enlace, el sistema arroja un **error de recurso no encontrado**, <br>
    <strong>Entonces</strong> el sistema muestra un mensaje amigable, <br>
    <strong>Y</strong> permite acceder a las secciones esenciales mediante enlaces alternativos sin bloquear la navegación. </td><td>EP01</td>
  </tr>
  <tr>
    <td>US02</td><td>Visualización de Planes </td><td>Como visitante de la Landing Page, quiero ver los planes de suscripción junto a su precio y características, para poder elegir el que mejor se adapte a mis necesidades.</td><td>
    <strong>Escenario 1: Visualización correcta de planes</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en la sección de planes de la landing page, <br>
    <strong>Cuando</strong> la página carga completamente, <br>
    <strong>Entonces</strong> debe ver al menos 2 planes de suscripción diferentes, <br>
    <strong>Y</strong> cada plan debe mostrar claramente: precio, características principales, duración y botón de selección, <br>
    <strong>Y</strong> debe poder comparar fácilmente las diferencias entre planes, <br>
    <strong>Y</strong> todos los elementos deben ser legibles y estar correctamente alineados. <br><br>
    
  <strong>Escenario 2: Error en carga de planes</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en la sección de planes, <br>
    <strong>Cuando</strong> ocurre un error en la carga de información de planes, <br>
    <strong>Entonces</strong> se muestra un mensaje de error amigable, <br>
    <strong>Y</strong> se proporciona una opción para recargar la información, <br>
    <strong>Y</strong> el visitante puede acceder a información de contacto como alternativa.
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US03</td><td>Selección de Plan en Landing Page</td><td>Como visitante de la landing Page, quiero seleccionar un plan y finalizar la confirmación en la misma pantalla, para agilizar y simplificar el registro.</td><td>
    <strong>Escenario 1: Selección y confirmación exitosa</strong> <br>
    <strong>Dado que</strong> un visitante está visualizando los planes disponibles, <br>
    <strong>Cuando</strong> selecciona un plan específico y **pulsa el botón** "Seleccionar", <br>
    <strong>Entonces</strong> es dirigido a un formulario de confirmación en la misma pantalla, <br>
    <strong>Y</strong> el formulario muestra el plan seleccionado con su precio, <br>
    <strong>Y</strong> puede completar sus datos y confirmar la selección, <br>
    <strong>Y</strong> recibe una confirmación inmediata del proceso. <br><br>
    
  <strong>Escenario 2: Selección sin completar datos requeridos</strong> <br>
    <strong>Dado que</strong> un visitante está en el formulario de confirmación de plan, <br>
    <strong>Cuando</strong> intenta confirmar sin completar campos obligatorios, <br>
    <strong>Entonces</strong> se muestran mensajes de validación específicos para cada campo faltante, <br>
    <strong>Y</strong> el formulario mantiene la información ya ingresada, <br>
    <strong>Y</strong> puede corregir y reenviar sin perder progreso.
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US04</td><td>Visualización de creadores</td><td>Como visitante de la Landing Page, quiero ver a los creadores de la aplicación, para conocer al equipo detrás del producto y generar confianza en el servicio.</td><td>
    <strong>Escenario 1: Acceso exitoso a información del equipo</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en la landing page, <br>
    <strong>Cuando</strong> navega a la sección "Sobre nosotros" o "Equipo", <br>
    <strong>Entonces</strong> puede ver información de cada creador incluyendo: nombre, foto, rol y breve descripción, <br>
    <strong>Y</strong> la información se presenta de manera profesional y organizada, <br>
    <strong>Y</strong> puede acceder a perfiles profesionales o redes sociales si están disponibles. <br><br>
    
  <strong>Escenario 2: Información de equipo no disponible</strong> <br>
    <strong>Dado que</strong> un visitante está intentando acceder a información del equipo, <br>
    <strong>Cuando</strong> la sección no carga correctamente, <br>
    <strong>Entonces</strong> se muestra un mensaje explicativo, <br>
    <strong>Y</strong> se proporciona información de contacto alternativa, <br>
    <strong>Y</strong> el visitante puede continuar navegando otras secciones sin problemas.
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US05</td><td>Redes sociales</td><td>Como visitante del landing page quiero poder acceder fácilmente a sus redes sociales de Veyra para conocer más sobre la empresa y tener canales adicionales de contacto </td><td>
    <strong>Escenario 1: Acceso exitoso a redes sociales</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en cualquier página de la landing page, <br>
    <strong>Cuando</strong> busca enlaces a redes sociales en el footer o header, <br>
    <strong>Entonces</strong> encuentra íconos claramente identificables de las principales redes sociales, <br>
    <strong>Y</strong> al **activar el ícono**, se abren las páginas oficiales de Veyra en una nueva pestaña, <br>
    <strong>Y</strong> los enlaces funcionan correctamente y dirigen al contenido apropiado. <br><br>
    
  <strong>Escenario 2: Enlaces de redes sociales no funcionales</strong> <br>
    <strong>Dado que</strong> un visitante está intentando acceder a redes sociales, <br>
    <strong>Cuando</strong> **interactúa con** un ícono de red social que no responde, <br>
    <strong>Entonces</strong> recibe un mensaje de error informativo, <br>
    <strong>Y</strong> se proporciona información de contacto alternativa, <br>
    <strong>Y</strong> puede continuar su navegación sin interrupciones.
    </td><td>EP02</td>
  </tr>
  <tr>
    <td>US06</td><td>Formulario de contacto</td><td>Como visitante del landing page quiero completar un formulario de contacto para enviar consultas específicas y recibir una respuesta personalizada de Veyra</td><td>
    <strong>Escenario 1: Envío exitoso de consulta</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en el formulario de contacto, <br>
    <strong>Cuando</strong> completa todos los campos requeridos (nombre, email, asunto, mensaje), <br>
    <strong>Y</strong> **pulsa el botón** "Enviar", <br>
    <strong>Entonces</strong> recibe una confirmación de que su mensaje fue enviado, <br>
    <strong>Y</strong> se le informa el tiempo estimado de respuesta, <br>
    <strong>Y</strong> recibe una copia de confirmación en su email. <br><br>
    
  <strong>Escenario 2: Formulario con datos inválidos</strong> <br>
    <strong>Dado que</strong> un visitante está completando el formulario de contacto, <br>
    <strong>Cuando</strong> ingresa un email inválido o deja campos obligatorios vacíos, <br>
    <strong>Y</strong> intenta enviar el formulario, <br>
    <strong>Entonces</strong> se muestran mensajes de validación específicos, <br>
    <strong>Y</strong> se mantiene la información correcta ya ingresada, <br>
    <strong>Y</strong> puede corregir y reenviar.
    </td><td>EP02</td>
  </tr>
  <tr>
    <td>US07</td><td>Cambio de idioma</td><td>Como visitante del Landing Page quiero en el menú un botón para cambiar de idioma entre español e inglés para  entender mejor de que trata Veyra</td><td>
    <strong>Escenario 1: Cambio exitoso de idioma</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en la landing page en español, <br>
    <strong>Cuando</strong> **selecciona la opción** de cambio de idioma y elige inglés, <br>
    <strong>Entonces</strong> toda la interfaz cambia al idioma seleccionado, <br>
    <strong>Y</strong> el contenido se mantiene equivalente en significado, <br>
    <strong>Y</strong> la preferencia de idioma se mantiene al navegar entre páginas. <br><br>
    
  <strong>Escenario 2: Idioma no disponible temporalmente</strong> <br>
    <strong>Dado que</strong> un visitante está intentando cambiar de idioma, <br>
    <strong>Cuando</strong> el servicio de traducción no está disponible, <br>
    <strong>Entonces</strong> se muestra un mensaje informativo sobre la situación, <br>
    <strong>Y</strong> se mantiene el idioma actual funcionando, <br>
    <strong>Y</strong> se proporciona información en el idioma disponible.
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US08</td><td>Historial médico </td><td>Como familiar de un adulto mayor quiero acceder al historial médico completo de mi familiar para conocer su evolución de salud y diagnósticos actuales</td><td>
    <strong>Escenario 1: Acceso exitoso al historial médico</strong> <br>
    <strong>Dado que</strong> un familiar está autenticado en el sistema, <br>
    <strong>Cuando</strong> navega a la sección "Historial Médico" de su familiar, <br>
    <strong>Entonces</strong> puede ver diagnósticos actuales, evolución de salud y últimas actualizaciones, <br>
    <strong>Y</strong> la información está organizada cronológicamente, <br>
    <strong>Y</strong> puede filtrar por fechas o tipos de reportes, <br>
    <strong>Y</strong> toda la información es legible y está actualizada. <br><br>
    
  <strong>Escenario 2: Sin permisos para acceder a reportes</strong> <br>
    <strong>Dado que</strong> un usuario está intentando acceder a historial médico, <br>
    <strong>Cuando</strong> no tiene los permisos necesarios, <br>
    <strong>Entonces</strong> se muestra un mensaje claro sobre restricciones de acceso, <br>
    <strong>Y</strong> se proporciona información sobre cómo obtener permisos, <br>
    <strong>Y</strong> puede contactar al administrador para resolver el acceso.
    </td><td>EP03</td>
  </tr>
  <tr>
    <td>US09</td><td>Agenda de citas Medicas</td><td>Como familiar de un adulto mayor quiero consultar la agenda de citas médicas de mi familiar para estar informado sobre sus próximos tratamientos</td><td>
    <strong>Escenario 1: Visualización exitosa de citas programadas</strong> <br>
    <strong>Dado que</strong> un familiar está autenticado en el sistema, <br>
    <strong>Cuando</strong> accede a la agenda de citas de su familiar, <br>
    <strong>Entonces</strong> puede ver todas las citas programadas con fecha, hora, médico y tipo de consulta, <br>
    <strong>Y</strong> puede filtrar por rangos de fechas, <br>
    <strong>Y</strong> recibe indicaciones claras sobre próximas citas importantes, <br>
    <strong>Y</strong> puede exportar o imprimir la agenda si es necesario. <br><br>
    
  <strong>Escenario 2: No hay citas programadas</strong> <br>
    <strong>Dado que</strong> un familiar está consultando la agenda de citas, <br>
    <strong>Cuando</strong> no hay citas programadas para su familiar, <br>
    <strong>Entonces</strong> se muestra un mensaje informativo indicando que no hay citas, <br>
    <strong>Y</strong> se proporciona información sobre cómo programar nuevas citas, <br>
    <strong>Y</strong> puede contactar al personal médico si es necesario.
    </td><td>EP03</td>
  </tr>
  <tr>
    <td>US10</td><td>Consulta de información personal</td><td>Como familiar de un adulto mayor quiero ver la información de mi familiar para estar seguro de que esté correcto o actualizado.</td><td>
    <strong>Escenario 1: Visualización exitosa de información personal</strong> <br>
    <strong>Dado que</strong> un familiar está autenticado en el sistema, <br>
    <strong>Cuando</strong> accede al perfil de información personal de su familiar, <br>
    <strong>Entonces</strong> puede ver datos personales actualizados: nombre, edad, contacto de emergencia, alergias, medicamentos actuales, <br>
    <strong>Y</strong> puede identificar fácilmente si algún dato requiere actualización, <br>
    <strong>Y</strong> tiene acceso a opciones para solicitar modificaciones. <br><br>
    
  <strong>Escenario 2: Información desactualizada detectada</strong> <br>
    <strong>Dado que</strong> un familiar está revisando información personal, <br>
    <strong>Cuando</strong> identifica información que necesita actualización, <br>
    <strong>Entonces</strong> puede marcar campos como "requiere actualización", <br>
    <strong>Y</strong> puede enviar solicitudes de cambio con justificación, <br>
    <strong>Y</strong> recibe confirmación de que la solicitud fue recibida.
    </td><td>EP03</td>
  </tr>
  <tr>
    <td>US11</td><td>Galería de fotos y actividades</td><td>Como familiar de un adulto mayor quiero ver fotos de las actividades diarias de mi familiar para sentirme conectado con su día a día y verificar su participación social</td><td>
    <strong>Escenario 1: Acceso exitoso a galería de actividades</strong> <br>
    <strong>Dado que</strong> un familiar está autenticado en el sistema, <br>
    <strong>Cuando</strong> accede a la galería de fotos de su familiar, <br>
    <strong>Entonces</strong> puede ver fotos organizadas por fecha y tipo de actividad, <br>
    <strong>Y</strong> cada foto incluye descripción de la actividad realizada, <br>
    <strong>Y</strong> puede filtrar por fechas o tipos de actividades, <br>
    <strong>Y</strong> las fotos se cargan correctamente y son de buena calidad. <br><br>
    
  <strong>Escenario 2: Sin actividades recientes registradas</strong> <br>
    <strong>Dado que</strong> un familiar está consultando la galería, <br>
    <strong>Cuando</strong> no hay fotos recientes de actividades, <br>
    <strong>Entonces</strong> se muestra un mensaje informativo sobre la situación, <br>
    <strong>Y</strong> se proporciona información sobre la frecuencia de actualización de fotos, <br>
    <strong>Y</strong> puede contactar al personal para consultas específicas.
    </td><td>EP03</td>
  </tr>
  <tr>
    <td>US12</td><td>Registro de residentes</td><td>Como administrador de casa de reposo quiero crear y mantener perfiles completos de cada residente para centralizar toda su información personal y médica</td><td>
    <strong>Escenario 1: Creación exitosa de perfil de residente</strong> <br>
    <strong>Dado que</strong> un administrador está autenticado en el sistema, <br>
    <strong>Cuando</strong> accede al formulario de registro de nuevo residente, <br>
    <strong>Y</strong> completa toda la información requerida (datos personales, médicos, contactos de emergencia), <br>
    <strong>Entonces</strong> el perfil se crea exitosamente, <br>
    <strong>Y</strong> se genera un ID único para el residente, <br>
    <strong>Y</strong> toda la información queda almacenada y accesible para consultas futuras. <br><br>
    
  <strong>Escenario 2: Error en datos requeridos para registro</strong> <br>
    <strong>Dado que</strong> un administrador está creando un perfil de residente, <br>
    <strong>Cuando</strong> falta información crítica requerida, <br>
    <strong>Y</strong> intenta guardar el perfil incompleto, <br>
    <strong>Entonces</strong> se muestran mensajes específicos de campos faltantes, <br>
    <strong>Y</strong> se mantiene la información ya ingresada, <br>
    <strong>Y</strong> puede completar los datos faltantes y continuar.
    </td><td>EP04</td>
  </tr>
  <tr>
    <td>US13</td><td>Historial médico institucional</td><td>Como administrador quiero gestionar el historial médico completo de cada residente para asegurar continuidad en el cuidado y cumplir con regulaciones sanitarias
    </td><td>
    <strong>Escenario 1: Gestión exitosa de historial médico completo</strong> <br>
    <strong>Dado que</strong> un administrador tiene permisos médicos, <br>
    <strong>Cuando</strong> accede al historial médico de un residente, <br>
    <strong>Entonces</strong> puede ver, agregar y actualizar información médica completa, <br>
    <strong>Y</strong> puede registrar nuevos diagnósticos, tratamientos y evoluciones, <br>
    <strong>Y</strong> toda la información queda registrada con fecha, hora y responsable, <br>
    <strong>Y</strong> puede generar reportes médicos para autoridades sanitarias. <br><br>
    
  <strong>Escenario 2: Acceso sin permisos médicos suficientes</strong> <br>
    <strong>Dado que</strong> un usuario está intentando acceder a historial médico institucional, <br>
    <strong>Cuando</strong> no posee los permisos necesarios, <br>
    <strong>Entonces</strong> se restringe el acceso con mensaje explicativo, <br>
    <strong>Y</strong> se proporciona información sobre cómo obtener permisos apropiados, <br>
    <strong>Y</strong> puede acceder solo a información no confidencial si corresponde.
    </td><td>EP04</td>
  </tr>
  <tr>
    <td>US14</td><td>Administración de medicamentos</td><td>Como administrador quiero controlar la administración de medicamentos de todos los residentes para garantizar cumplimiento de tratamientos y evitar errores médicos</td><td>
    <strong>Escenario 1: Control exitoso de administración de medicamentos</strong> <br>
    <strong>Dado que</strong> un administrador se encuentra en el módulo de medicamentos, <br>
    <strong>Cuando</strong> registra la administración de medicamentos a residentes, <br>
    <strong>Entonces</strong> puede marcar medicamentos como administrados con hora exacta, <br>
    <strong>Y</strong> puede registrar observaciones sobre efectos o reacciones, <br>
    <strong>Y</strong> el sistema alerta sobre próximas dosis programadas, <br>
    <strong>Y</strong> mantiene historial completo de administración por residente. <br><br>
    
  <strong>Escenario 2: Medicamento no disponible en inventario</strong> <br>
    <strong>Dado que</strong> un administrador está intentando registrar la administración de medicamento, <br>
    <strong>Cuando</strong> el medicamento no está disponible en inventario, <br>
    <strong>Entonces</strong> el sistema muestra alerta de falta de stock, <br>
    <strong>Y</strong> proporciona opciones para contactar a farmacia o proveedor, <br>
    <strong>Y</strong> permite registrar la situación para seguimiento.
    </td><td>EP04</td>
  </tr>
  <tr>
    <td>US15</td><td>Gestión de visitas familiares</td><td>Como administrador quiero controlar y programar las visitas familiares a los residentes para mantener seguridad, orden y cumplir con los horarios establecidos</td><td>
    <strong>Escenario 1: Programación exitosa de visita familiar</strong> <br>
    <strong>Dado que</strong> un administrador se encuentra en el módulo de visitas, <br>
    <strong>Cuando</strong> programa una nueva visita familiar, <br>
    <strong>Entonces</strong> puede asignar fecha, hora, visitantes y residente a visitar, <br>
    <strong>Y</strong> el sistema verifica disponibilidad de horarios, <br>
    <strong>Y</strong> genera confirmación para la familia y actualiza agenda institucional, <br>
    <strong>Y</strong> envía recordatorios automáticos antes de la visita. <br><br>
    
  <strong>Escenario 2: Conflicto de horarios en visitas</strong> <br>
    <strong>Dado que</strong> un administrador está programando una visita familiar, <br>
    <strong>Cuando</strong> el horario solicitado ya está ocupado, <br>
    <strong>Entonces</strong> el sistema muestra horarios alternativos disponibles, <br>
    <strong>Y</strong> permite reprogramar o sugerir opciones similares, <br>
    <strong>Y</strong> notifica a la familia sobre el cambio de horario.
    </td><td>EP04</td>
  </tr>
  <tr>
    <td>US16</td><td>Recordatorios de citas y consultas</td><td> Como familiar quiero recibir recordatorios automáticos sobre citas médicas y consultas programadas de mi familiar para estar preparado y decidir si deseo acompañarlo</td><td>
    <strong>Escenario 1: Envío exitoso de recordatorios automáticos</strong> <br>
    <strong>Dado que</strong> el sistema tiene citas médicas programadas, <br>
    <strong>Cuando</strong> se acerca una cita médica (24 horas antes), <br>
    <strong>Entonces</strong> se envía recordatorio automático a familiares vía email/SMS, <br>
    <strong>Y</strong> el recordatorio incluye fecha, hora, médico y tipo de consulta, <br>
    <strong>Y</strong> los familiares pueden confirmar asistencia o reagendar, <br>
    <strong>Y</strong> el sistema registra la confirmación recibida. <br><br>
    
  <strong>Escenario 2: Falla en envío de recordatorios</strong> <br>
    <strong>Dado que</strong> el sistema está intentando enviar recordatorios, <br>
    <strong>Cuando</strong> falla el servicio de notificaciones, <br>
    <strong>Entonces</strong> se registra el error en logs del sistema, <br>
    <strong>Y</strong> se intenta reenvío automático después de un tiempo, <br>
    <strong>Y</strong> se notifica al administrador sobre fallas en el sistema.
    </td><td>EP05</td>
  </tr>
  <tr>
    <td>US17</td><td>Notificaciones de cambios en medicación</td><td>Como familiar quiero ser notificado inmediatamente sobre cualquier cambio en la medicación de mi familiar para estar informado sobre su tratamiento médico</td><td>
    <strong>Escenario 1: Notificación inmediata de cambio en medicación</strong> <br>
    <strong>Dado que</strong> ha ocurrido un cambio en la medicación de un residente, <br>
    <strong>Cuando</strong> el médico actualiza el tratamiento farmacológico, <br>
    <strong>Entonces</strong> se envía notificación inmediata a familiares autorizados, <br>
    <strong>Y</strong> la notificación incluye detalles del cambio y justificación médica, <br>
    <strong>Y</strong> los familiares pueden contactar al médico para consultas, <br>
    <strong>Y</strong> el cambio queda registrado en el historial médico. <br><br>
    
  <strong>Escenario 2: Familiar no autorizado para recibir información médica</strong> <br>
    <strong>Dado que</strong> ha ocurrido un cambio en la medicación de un residente, <br>
    <strong>Cuando</strong> un familiar no está autorizado para recibir información médica, <br>
    <strong>Entonces</strong> no recibe notificación de cambios en medicación, <br>
    <strong>Y</strong> se respetan las preferencias de privacidad del residente, <br>
    <strong>Y</strong> solo familiares autorizados reciben las notificaciones.
    </td><td>EP05</td>
  </tr>
  <tr>
    <td>US18</td><td>Recordatorios de visitas familiares</td><td>Como familiar quiero recibir recordatorios automáticos sobre mis visitas programadas al adulto mayor para no olvidar las citas y mantener regularidad en el contacto</td><td>
    <strong>Escenario 1: Recordatorio exitoso de visita programada</strong> <br>
    <strong>Dado que</strong> hay una visita familiar programada, <br>
    <strong>Cuando</strong> faltan 2 horas para la visita, <br>
    <strong>Entonces</strong> se envía recordatorio automático al familiar, <br>
    <strong>Y</strong> el recordatorio incluye fecha, hora, nombre del residente e instrucciones de acceso, <br>
    <strong>Y</strong> el familiar puede confirmar asistencia o cancelar con anticipación, <br>
    <strong>Y</strong> el sistema actualiza el estado de la visita según la respuesta. <br><br>
    
  <strong>Escenario 2: Cancelación de visita por emergencia</strong> <br>
    <strong>Dado que</strong> hay una visita familiar programada, <br>
    <strong>Cuando</strong> ocurre una emergencia que requiere cancelar la visita, <br>
    <strong>Entonces</strong> se envía notificación inmediata de cancelación, <br>
    <strong>Y</strong> se proporciona explicación de la situación, <br>
    <strong>Y</strong> se ofrecen alternativas de reprogramación.
    </td><td>EP05</td>
  </tr>
  <tr>
    <td>US19</td><td>Alertas de actualización de datos personales</td><td>Como familiar quiero recibir notificaciones automáticas cuando se actualice la información personal o de mi familiar para mantenerme informado de cualquier cambio en su perfil</td><td>
    <strong>Escenario 1: Notificación exitosa de actualización de datos</strong> <br>
    <strong>Dado que</strong> ha ocurrido una actualización en los datos personales del residente, <br>
    <strong>Cuando</strong> se modifica información como contacto de emergencia, estado de salud, o preferencias, <br>
    <strong>Entonces</strong> se envía notificación automática a familiares autorizados, <br>
    <strong>Y</strong> la notificación especifica qué información fue actualizada, <br>
    <strong>Y</strong> incluye fecha y responsable de la actualización, <br>
    <strong>Y</strong> los familiares pueden revisar los cambios en el sistema. <br><br>
    
  <strong>Escenario 2: Actualización sin autorización para notificar</strong> <br>
    <strong>Dado que</strong> ha ocurrido una actualización en los datos personales, <br>
    <strong>Cuando</strong> el familiar no tiene autorización para recibir cierto tipo de información, <br>
    <strong>Entonces</strong> no recibe notificación sobre datos restringidos, <br>
    <strong>Y</strong> solo recibe información sobre cambios que está autorizado a conocer, <br>
    <strong>Y</strong> se respetan las políticas de privacidad establecidas.
    </td><td>EP05</td>
  </tr>
  <tr>
    <td>US20</td><td>Preguntas sobre rutina de cuidados</td><td>Como familiar quiero hacer preguntas específicas sobre la rutina diaria y cuidados de mi familiar para entender mejor su día a día y resolver dudas puntuales</td><td>
    <strong>Escenario 1: Envío exitoso de pregunta sobre cuidados</strong> <br>
    <strong>Dado que</strong> un familiar está autenticado en el sistema de comunicación, <br>
    <strong>Cuando</strong> redacta una pregunta específica sobre la rutina de cuidados de su familiar, <br>
    <strong>Entonces</strong> puede enviar la consulta al personal de cuidadores asignado, <br>
    <strong>Y</strong> recibe confirmación de que la pregunta fue enviada, <br>
    <strong>Y</strong> el sistema establece un tiempo estimado de respuesta, <br>
    <strong>Y</strong> puede hacer seguimiento del estado de su consulta. <br><br>
    
  <strong>Escenario 2: Canal de comunicación no disponible</strong> <br>
    <strong>Dado que</strong> un familiar está intentando enviar una pregunta sobre cuidados, <br>
    <strong>Cuando</strong> el sistema de comunicación no está disponible, <br>
    <strong>Entonces</strong> se muestra mensaje sobre la situación temporal, <br>
    <strong>Y</strong> se proporcionan números de teléfono alternativos para emergencias, <br>
    <strong>Y</strong> se permite guardar la pregunta para envío posterior.
    </td><td>EP06</td>
  </tr>
  <tr>
    <td>US21</td><td>Peticiones de modificación de cuidados</td><td>Como familiar quiero solicitar ajustes específicos en el cuidado de mi familiar basados en sus preferencias o necesidades particulares</td><td>
    <strong>Escenario 1: Solicitud exitosa de modificación de cuidados</strong> <br>
    <strong>Dado que</strong> un familiar tiene permisos para solicitar cambios, <br>
    <strong>Cuando</strong> envía una petición detallada de modificación en cuidados específicos, <br>
    <strong>Entonces</strong> la solicitud se registra en el sistema con número de seguimiento, <br>
    <strong>Y</strong> se notifica al coordinador de cuidados correspondiente, <br>
    <strong>Y</strong> recibe confirmación con plazos estimados de evaluación, <br>
    <strong>Y</strong> puede hacer seguimiento del estado de su petición. <br><br>
    
  <strong>Escenario 2: Solicitud que requiere aprobación médica</strong> <br>
    <strong>Dado que</strong> un familiar está solicitando una modificación que requiere aprobación médica, <br>
    <strong>Cuando</strong> la petición involucra aspectos médicos o terapéuticos, <br>
    <strong>Entonces</strong> se deriva automáticamente al equipo médico, <br>
    <strong>Y</strong> se informa al familiar sobre el proceso de evaluación médica, <br>
    <strong>Y</strong> se establecen plazos específicos para respuesta médica.
    </td><td>EP06</td>
  </tr>
  <tr>
    <td>US22</td><td>Seguimiento del bienestar emocional</td><td>Como familiar quiero comunicarme con el personal sobre el estado emocional y psicológico de mi familiar para asegurar su bienestar integral</td><td>
    <strong>Escenario 1: Comunicación exitosa sobre estado emocional</strong> <br>
    <strong>Dado que</strong> un familiar está preocupado por el bienestar emocional de su familiar, <br>
    <strong>Cuando</strong> envía consulta sobre estado anímico, interacción social o adaptación, <br>
    <strong>Entonces</strong> puede comunicarse directamente con el equipo de psicología/trabajo social, <br>
    <strong>Y</strong> recibe respuesta profesional sobre la situación emocional del residente, <br>
    <strong>Y</strong> se le proporcionan recomendaciones para apoyo emocional, <br>
    <strong>Y</strong> puede programar reuniones de seguimiento si es necesario. <br><br>
    
  <strong>Escenario 2: Situación emocional que requiere atención inmediata</strong> <br>
    <strong>Dado que</strong> un familiar está reportando cambios emocionales significativos, <br>
    <strong>Cuando</strong> la situación indica posible crisis emocional o depresión, <br>
    <strong>Entonces</strong> se escalona automáticamente a atención psicológica prioritaria, <br>
    <strong>Y</strong> se notifica al equipo médico y de trabajo social, <br>
    <strong>Y</strong> se contacta al familiar para coordinar intervención.
    </td><td>EP06</td>
  </tr>
  <tr>
    <td>US23</td><td>Planificación de eventos familiares</td><td>Como familiar quiero coordinar con el personal la organización de eventos especiales o celebraciones para mi familiar dentro de las instalaciones</td><td>
    <strong>Escenario 1: Coordinación exitosa de evento familiar</strong> <br>
    <strong>Dado que</strong> un familiar está planificando un evento especial para su familiar, <br>
    <strong>Cuando</strong> solicita coordinación para celebración de cumpleaños, aniversario u ocasión especial, <br>
    <strong>Entonces</strong> puede especificar fecha, número de invitados, requerimientos especiales, <br>
    <strong>Y</strong> el personal evalúa viabilidad según protocolos institucionales, <br>
    <strong>Y</strong> se coordinan espacios, horarios y recursos necesarios, <br>
    <strong>Y</strong> recibe confirmación con detalles finales del evento. <br><br>
    
  <strong>Escenario 2: Evento que no cumple con protocolos institucionales</strong> <br>
    <strong>Dado que</strong> un familiar está solicitando un evento que no cumple protocolos, <br>
    <strong>Cuando</strong> la solicitud involucra aspectos no permitidos por políticas institucionales, <br>
    <strong>Entonces</strong> se explican las limitaciones y razones institucionales, <br>
    <strong>Y</strong> se ofrecen alternativas que cumplan con protocolos, <br>
    <strong>Y</strong> se proporcionan opciones modificadas para el evento.
    </td><td>EP06</td>
  </tr>
  <tr>
    <td>US24</td><td>Registro de medicamentos en inventario</td><td>Como administrador quiero registrar todos los medicamentos que ingresan al inventario con sus datos completos para mantener un catálogo actualizado</td><td>
    <strong>Escenario 1: Registro exitoso de medicamentos</strong> <br>
    <strong>Dado que</strong> un administrador se encuentra en el módulo de inventario de medicamentos, <br>
    <strong>Cuando</strong> registra un nuevo medicamento con todos los datos requeridos (nombre, laboratorio, lote, fecha de vencimiento, cantidad), <br>
    <strong>Entonces</strong> el medicamento se añade correctamente al inventario, <br>
    <strong>Y</strong> se genera un código de identificación único, <br>
    <strong>Y</strong> se actualiza el stock total disponible, <br>
    <strong>Y</strong> el sistema registra fecha y responsable del ingreso. <br><br>
    
  <strong>Escenario 2: Medicamento duplicado en inventario</strong> <br>
    <strong>Dado que</strong> un administrador está registrando un medicamento, <br>
    <strong>Cuando</strong> intenta ingresar un medicamento que ya existe con el mismo lote, <br>
    <strong>Entonces</strong> el sistema detecta la duplicación y muestra alerta, <br>
    <strong>Y</strong> permite actualizar la cantidad del lote existente en lugar de crear un duplicado, <br>
    <strong>Y</strong> mantiene la integridad de datos en el inventario.
    </td><td>EP07</td>
  </tr>
  <tr>
    <td>US25</td><td>Alertas de vencimiento</td><td>Como administrador quiero recibir alertas automáticas sobre medicamentos próximos a vencer para evitar pérdidas y riesgos de seguridad</td><td>
    <strong>Escenario 1: Generación de alerta por medicamentos próximos a vencer</strong> <br>
    <strong>Dado que</strong> hay medicamentos en inventario próximos a vencer, <br>
    <strong>Cuando</strong> faltan 30 días para la fecha de vencimiento, <br>
    <strong>Entonces</strong> se genera alerta automática al administrador de farmacia, <br>
    <strong>Y</strong> la alerta incluye lista de medicamentos, cantidades y fechas exactas, <br>
    <strong>Y</strong> se sugieren acciones como uso prioritario o devolución a proveedor, <br>
    <strong>Y</strong> se programa seguimiento semanal hasta resolución. <br><br>
    
  <strong>Escenario 2: Medicamentos ya vencidos en inventario</strong> <br>
    <strong>Dado que</strong> hay medicamentos que han superado su fecha de vencimiento, <br>
    <strong>Cuando</strong> el sistema detecta medicamentos vencidos, <br>
    <strong>Entonces</strong> se bloquea automáticamente su uso en el sistema, <br>
    <strong>Y</strong> se genera alerta crítica para remoción inmediata, <br>
    <strong>Y</strong> se registra como pérdida en reportes de inventario.
    </td><td>EP07</td>
  </tr>
  <tr>
    <td>US26</td><td>Eliminación de medicamentos</td><td>Como administrador quiero eliminar medicamentos del inventario de manera controlada para mantener la precisión del stock y cumplir con protocolos de disposición</td><td>
    <strong>Escenario 1: Eliminación controlada de medicamento</strong> <br>
    <strong>Dado que</strong> un administrador necesita eliminar un medicamento del inventario, <br>
    <strong>Cuando</strong> selecciona el medicamento y especifica la razón (vencido, dañado, usado), <br>
    <strong>Entonces</strong> debe proporcionar justificación y autorización apropiada, <br>
    <strong>Y</strong> el sistema registra la eliminación con fecha, cantidad y responsable, <br>
    <strong>Y</strong> se actualiza automáticamente el stock disponible, <br>
    <strong>Y</strong> se genera reporte de eliminación para auditoría. <br><br>
    
  <strong>Escenario 2: Intento de eliminación sin autorización</strong> <br>
    <strong>Dado que</strong> un usuario está intentando eliminar un medicamento sin permisos suficientes, <br>
    <strong>Cuando</strong> no posee los permisos necesarios para eliminación, <br>
    <strong>Entonces</strong> el sistema niega el acceso con mensaje explicativo, <br>
    <strong>Y</strong> se registra el intento en logs de seguridad, <br>
    <strong>Y</strong> se notifica al administrador sobre el intento no autorizado.
    </td><td>EP07</td>
  </tr>
  <tr>
    <td>US27</td><td>Búsqueda y filtrado de inventario</td><td>Como administrador quiero filtrar y buscar medicamentos en el inventario para encontrar rápidamente información específica y generar reportes personalizados</td><td>
    <strong>Escenario 1: Búsqueda exitosa de medicamentos</strong> <br>
    <strong>Dado que</strong> un administrador se encuentra en el módulo de inventario, <br>
    <strong>Cuando</strong> utiliza filtros de búsqueda por nombre, laboratorio, fecha de vencimiento o categoría, <br>
    <strong>Entonces</strong> obtiene resultados precisos que coinciden con los criterios, <br>
    <strong>Y</strong> puede ordenar resultados por diferentes campos, <br>
    <strong>Y</strong> puede exportar los resultados filtrados para reportes, <br>
    <strong>Y</strong> la búsqueda es rápida y eficiente. <br><br>
    
  <strong>Escenario 2: Búsqueda sin resultados</strong> <br>
    <strong>Dado que</strong> un administrador está buscando un medicamento específico, <br>
    <strong>Cuando</strong> los criterios de búsqueda no coinciden con ningún medicamento en inventario, <br>
    <strong>Entonces</strong> se muestra un mensaje claro de "sin resultados", <br>
    <strong>Y</strong> se sugieren búsquedas alternativas o similares, <br>
    <strong>Y</strong> se mantienen los filtros aplicados para fácil modificación.
    </td><td>EP07</td>
  </tr>
  <tr>
    <td>US28</td><td>Información de medicamentos para personal</td><td>Como administrador quiero proporcionar información detallada sobre medicamentos al personal para asegurar administración segura y correcta</td><td>
    <strong>Escenario 1: Acceso exitoso a información detallada de medicamentos</strong> <br>
    <strong>Dado que</strong> personal autorizado está consultando información de medicamento, <br>
    <strong>Cuando</strong> accede a detalles de medicamento específico, <br>
    <strong>Entonces</strong> puede ver información completa: dosificación, contraindicaciones, efectos secundarios, interacciones, <br>
    <strong>Y</strong> la información está actualizada y es confiable, <br>
    <strong>Y</strong> puede acceder a protocolos de administración específicos, <br>
    <strong>Y</strong> tiene enlaces a recursos adicionales si necesita más información. <br><br>
    
  <strong>Escenario 2: Medicamento con alertas especiales</strong> <br>
    <strong>Dado que</strong> personal está consultando un medicamento con requerimientos especiales, <br>
    <strong>Cuando</strong> el medicamento tiene alertas de seguridad o administración especial, <br>
    <strong>Entonces</strong> se muestran prominentemente todas las alertas y precauciones, <br>
    <strong>Y</strong> se requiere confirmación de lectura antes de proceder, <br>
    <strong>Y</strong> se proporcionan protocolos específicos de manejo.
    </td><td>EP07</td>
  </tr>
  <tr>
    <td>US29</td><td>Gestión de perfiles de empleados</td><td>Como administrador quiero registrar y mantener los perfiles completos del personal para tener información actualizada de todos los empleados.</td><td>
    <strong>Escenario 1: Registro exitoso de empleado</strong> <br>
    <strong>Dado que</strong> un administrador de RRHH está registrando un nuevo empleado, <br>
    <strong>Cuando</strong> completa información personal, profesional, contactos de emergencia y rol asignado, <br>
    <strong>Entonces</strong> el perfil se crea exitosamente en el sistema, <br>
    <strong>Y</strong> se genera ID de empleado único, <br>
    <strong>Y</strong> se asignan permisos según el rol especificado, <br>
    <strong>Y</strong> el empleado recibe credenciales de acceso al sistema. <br><br>
    
  <strong>Escenario 2: Información incompleta de empleado</strong> <br>
    <strong>Dado que</strong> un administrador está registrando un empleado con información faltante, <br>
    <strong>Cuando</strong> faltan datos críticos como certificaciones requeridas o contactos de emergencia, <br>
    <strong>Entonces</strong> el sistema indica específicamente qué información falta, <br>
    <strong>Y</strong> permite guardar como borrador para completar posteriormente, <br>
    <strong>Y</strong> no activa permisos hasta que toda la información requerida esté completa.
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US30</td><td>Baja de personal</td><td>Como administrador quiero dar de baja empleados del sistema para mantener registros actualizados y gestionar finalizaciones de contratos.</td><td>
    <strong>Escenario 1: Proceso exitoso de baja de empleado</strong> <br>
    <strong>Dado que</strong> un administrador está procesando la baja de un empleado, <br>
    <strong>Cuando</strong> especifica fecha de terminación, motivo y procedimientos de entrega, <br>
    <strong>Entonces</strong> se desactivan automáticamente todos los accesos al sistema, <br>
    <strong>Y</strong> se genera un reporte de finalización con tareas pendientes, <br>
    <strong>Y</strong> se actualiza la estructura organizacional, <br>
    <strong>Y</strong> se notifica a supervisores y equipos afectados. <br><br>
    
  <strong>Escenario 2: Empleado con responsabilidades activas</strong> <br>
    <strong>Dado que</strong> un administrador está intentando dar de baja a un empleado con responsabilidades activas, <br>
    <strong>Cuando</strong> el empleado tiene residentes asignados o tareas críticas pendientes, <br>
    <strong>Entonces</strong> el sistema alerta sobre responsabilidades que requieren reasignación, <br>
    <strong>Y</strong> proporciona una lista de tareas y residentes que deben transferirse, <br>
    <strong>Y</strong> requiere reasignación completa antes de procesar la baja.
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US31</td><td>Búsqueda y filtrado de empleados</td><td>Como administrador quiero filtrar y buscar empleados según diferentes criterios para encontrar rápidamente personal específico.</td><td>
    <strong>Escenario 1: Búsqueda exitosa de empleados</strong> <br>
    <strong>Dado que</strong> un administrador se encuentra en el módulo de gestión de personal, <br>
    <strong>Cuando</strong> utiliza filtros por departamento, rol, turno, o estado de empleo, <br>
    <strong>Entonces</strong> obtiene una lista precisa de empleados que coinciden con criterios, <br>
    <strong>Y</strong> puede ver información básica de cada empleado en los resultados, <br>
    <strong>Y</strong> puede acceder a perfiles completos desde los resultados, <br>
    <strong>Y</strong> puede exportar la lista filtrada para reportes. <br><br>
    
  <strong>Escenario 2: Filtros que no retornan resultados</strong> <br>
    <strong>Dado que</strong> un administrador está aplicando filtros específicos, <br>
    <strong>Cuando</strong> la combinación de filtros no coincide con ningún empleado, <br>
    <strong>Entonces</strong> se muestra un mensaje claro indicando ausencia de resultados, <br>
    <strong>Y</strong> se sugiere modificar criterios de búsqueda, <br>
    <strong>Y</strong> se mantienen los filtros aplicados para fácil modificación.
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US32</td><td>Gestión de horas extra</td><td>Como administrador quiero controlar las horas extra trabajadas por el personal para gestionar costos laborales y cumplir con regulaciones de trabajo</td><td>
    <strong>Escenario 1: Registro exitoso de horas extra</strong> <br>
    <strong>Dado que</strong> un administrador está registrando horas extra de empleado, <br>
    <strong>Cuando</strong> especifica empleado, fecha, horas trabajadas y justificación, <br>
    <strong>Entonces</strong> las horas se registran correctamente en el sistema, <br>
    <strong>Y</strong> se calculan automáticamente los montos según tarifas establecidas, <br>
    <strong>Y</strong> se actualiza el reporte mensual de horas extra, <br>
    <strong>Y</strong> se notifica al empleado sobre el registro. <br><br>
    
  <strong>Escenario 2: Horas extra que exceden límites permitidos</strong> <br>
    <strong>Dado que</strong> un administrador está registrando horas extra que exceden límites legales, <br>
    <strong>Cuando</strong> las horas superan los máximos permitidos por regulaciones laborales, <br>
    <strong>Entonces</strong> el sistema muestra alerta sobre violación de límites, <br>
    <strong>Y</strong> requiere autorización especial y justificación, <br>
    <strong>Y</strong> se genera reporte para revisión de RRHH.
    </td><td>EP08</td>
  </tr>
  <tr>
    <td>US33</td><td>Gestión de horarios de atención</td><td>Como administrador quiero configurar los horarios de atención y servicios para informar claramente a familias sobre disponibilidad</td><td>
    <strong>Escenario 1: Configuración exitosa de horarios</strong> <br>
    <strong>Dado que</strong> un administrador está configurando horarios de atención, <br>
    <strong>Cuando</strong> establece horarios por servicio, día de semana y disponibilidad de personal, <br>
    <strong>Entonces</strong> los horarios se actualizan en toda la plataforma, <br>
    <strong>Y</strong> las familias pueden ver horarios actualizados al programar visitas o servicios, <br>
    <strong>Y</strong> se generan calendarios de disponibilidad automáticamente, <br>
    <strong>Y</strong> se sincroniza con sistemas de programación de citas. <br><br>
    
  <strong>Escenario 2: Cambio de horarios por emergencia</strong> <br>
    <strong>Dado que</strong> un administrador está modificando horarios por situación de emergencia, <br>
    <strong>Cuando</strong> debe cambiar horarios por situaciones imprevistas, <br>
    <strong>Entonces</strong> puede realizar cambios inmediatos con notificación automática, <br>
    <strong>Y</strong> todas las partes afectadas reciben notificación instantánea, <br>
    <strong>Y</strong> se reprograman automáticamente citas afectadas.
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US34</td><td>Datos de contacto institucional</td><td>Como administrador quiero gestionar la información de contacto de la casa de reposo para que familias y autoridades tengan acceso a datos actualizados</td><td>
    <strong>Escenario 1: Actualización exitosa de información de contacto</strong> <br>
    <strong>Dado que</strong> un administrador está actualizando datos de contacto institucional, <br>
    <strong>Cuando</strong> modifica teléfonos, emails, dirección o personas de contacto, <br>
    <strong>Entonces</strong> la información se actualiza inmediatamente en toda la plataforma, <br>
    <strong>Y</strong> se refleja en landing page, aplicaciones y documentos oficiales, <br>
    <strong>Y</strong> se notifica automáticamente a familias sobre cambios importantes, <br>
    <strong>Y</strong> se mantiene historial de cambios para auditoría. <br><br>
    
  <strong>Escenario 2: Información de contacto de emergencia</strong> <br>
    <strong>Dado que</strong> hay una situación que requiere contacto de emergencia, <br>
    <strong>Cuando</strong> familias necesitan contactar urgentemente a la institución, <br>
    <strong>Entonces</strong> tienen acceso inmediato a números de emergencia 24/7, <br>
    <strong>Y</strong> pueden identificar fácilmente el contacto apropiado según la situación, <br>
    <strong>Y</strong> reciben respuesta rápida según protocolos de emergencia.
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US35</td><td>Información del personal directivo</td><td>Como administrador quiero gestionar la información del personal directivo para transparencia hacia familias y autoridades</td><td>
    <strong>Escenario 1: Gestión de información de personal directivo</strong> <br>
    <strong>Dado que</strong> un administrador está actualizando información de personal directivo, <br>
    <strong>Cuando</strong> modifica información de directores, coordinadores y personal clave, <br>
    <strong>Entonces</strong> la información se presenta profesionalmente a familias y autoridades, <br>
    <strong>Y</strong> incluye credenciales, experiencia y áreas de responsabilidad, <br>
    <strong>Y</strong> se actualiza automáticamente en materiales institucionales, <br>
    <strong>Y</strong> mantiene información siempre actualizada y verificable. <br><br>
    
  <strong>Escenario 2: Acceso a información directiva por autoridades</strong> <br>
    <strong>Dado que</strong> autoridades sanitarias están requiriendo información del personal directivo, <br>
    <strong>Cuando</strong> necesitan verificar credenciales y responsabilidades del personal clave, <br>
    <strong>Entonces</strong> pueden acceder a información completa y actualizada, <br>
    <strong>Y</strong> toda la documentación está organizada y es fácilmente verificable, <br>
    <strong>Y</strong> se proporciona información de contacto directo cuando es apropiado.
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US36</td><td>Historia institucional</td><td>Como administrador quiero gestionar la información histórica y reconocimientos de la casa de reposo para generar confianza y credibilidad</td><td>
    <strong>Escenario 1: Presentación de historia y reconocimientos institucionales</strong> <br>
    <strong>Dado que</strong> un administrador está gestionando información histórica institucional, <br>
    <strong>Cuando</strong> actualiza historia, reconocimientos, certificaciones y logros, <br>
    <strong>Entonces</strong> la información se presenta de manera atractiva y creíble, <br>
    <strong>Y</strong> incluye certificaciones vigentes y reconocimientos oficiales, <br>
        <strong>Y</strong> genera confianza en familias evaluando los servicios, <br>
        <strong>Y</strong> es fácilmente accesible para consulta de interesados. <br><br>
    
  <strong>Escenario 2: Verificación de certificaciones por autoridades</strong> <br>
    <strong>Dado que</strong> autoridades están verificando certificaciones institucionales, <br>
    <strong>Cuando</strong> requieren confirmar validez de licencias y reconocimientos, <br>
    <strong>Entonces</strong> pueden acceder a información verificable y actualizada, <br>
    <strong>Y</strong> todos los documentos incluyen números de registro y fechas de vigencia, <br>
    <strong>Y</strong> se proporciona contacto directo con entidades certificadoras.
    </td><td>EP09</td>
  </tr>
  <tr>
    <td>US37</td><td>Gestión de usuarios y permisos</td><td>Como administrador quiero saber quién tiene acceso al sistema y qué información puede ver cada usuario para proteger la privacidad de los datos</td><td>
    <strong>Escenario 1: Configuración exitosa de permisos de usuario</strong> <br>
    <strong>Dado que</strong> un administrador de sistema está gestionando accesos, <br>
    <strong>Cuando</strong> asigna roles y permisos específicos a usuarios (familiares, personal, administradores), <br>
    <strong>Entonces</strong> cada usuario accede únicamente a información autorizada para su rol, <br>
    <strong>Y</strong> los permisos se aplican consistentemente en toda la plataforma, <br>
    <strong>Y</strong> se registra toda actividad de acceso para auditoría, <br>
    <strong>Y</strong> se pueden modificar permisos sin afectar otros aspectos del sistema. <br><br>
    
  <strong>Escenario 2: Intento de acceso no autorizado</strong> <br>
    <strong>Dado que</strong> un usuario está intentando acceder a información fuera de sus permisos, <br>
    <strong>Cuando</strong> intenta acceder a datos que no le corresponden según su rol, <br>
    <strong>Entonces</strong> el sistema bloquea el acceso inmediatamente, <br>
    <strong>Y</strong> registra el intento en logs de seguridad, <br>
    <strong>Y</strong> notifica al administrador sobre el intento no autorizado, <br>
    <strong>Y</strong> proporciona mensaje claro sobre restricciones de acceso.
    </td><td>EP10</td>
  </tr>
  <tr>
    <td>US38</td><td>Protección de datos mediante cifrado</td><td>Como administrador quiero que toda la información sensible esté cifrada para proteger los datos personales y médicos de accesos no autorizados</td><td>
    <strong>Escenario 1: Cifrado exitoso de datos sensibles</strong> <br>
    <strong>Dado que</strong> el sistema está almacenando información personal y médica, <br>
    <strong>Cuando</strong> se guardan datos sensibles de residentes y familias, <br>
    <strong>Entonces</strong> toda la información se cifra automáticamente antes del almacenamiento, <br>
    <strong>Y</strong> las comunicaciones entre usuario y servidor están cifradas, <br>
    <strong>Y</strong> solo usuarios autorizados pueden descifrar información específica, <br>
    <strong>Y</strong> se mantienen estándares de seguridad médica requeridos. <br><br>
    
  <strong>Escenario 2: Intento de acceso a datos cifrados sin autorización</strong> <br>
    <strong>Dado que</strong> hay un intento de acceso directo a datos cifrados, <br>
    <strong>Cuando</strong> alguien intenta acceder a información sin autorización apropiada, <br>
    <strong>Entonces</strong> los datos permanecen completamente inaccesibles, <br>
    <strong>Y</strong> se registra el intento de acceso no autorizado, <br>
    <strong>Y</strong> se activan alertas de seguridad automáticas, <br>
    <strong>Y</strong> se notifica inmediatamente al equipo de seguridad.
    </td><td>EP10</td>
  </tr>
  <tr>
    <td>US39</td><td>Terminos y condiciones</td><td>Como visitante de la landing page quiero poder acceder a los términos y condiciones de uso para conocer las políticas legales antes de contratar los servicios</td><td>
    <strong>Escenario 1: Acceso exitoso a términos y condiciones</strong> <br>
    <strong>Dado que</strong> un visitante se encuentra en la landing page, <br>
    <strong>Cuando</strong> busca información legal sobre términos y condiciones de uso, <br>
    <strong>Entonces</strong> puede acceder fácilmente a documento completo desde footer o header, <br>
    <strong>Y</strong> los términos están redactados claramente y son comprensibles, <br>
    <strong>Y</strong> incluyen políticas de privacidad, uso de datos y responsabilidades, <br>
    <strong>Y</strong> están actualizados con fecha de última modificación. <br><br>
    
  <strong>Escenario 2: Aceptación requerida de términos actualizados</strong> <br>
    <strong>Dado que</strong> los términos y condiciones han sido actualizados, <br>
    <strong>Cuando</strong> un usuario existente ingresa al sistema después de la actualización, <br>
    <strong>Entonces</strong> debe revisar y aceptar los nuevos términos antes de continuar, <br>
    <strong>Y</strong> se destacan claramente los cambios realizados, <br>
    <strong>Y</strong> puede comparar versión anterior si lo desea.
    </td><td>EP01</td>
  </tr>
  <tr>
    <td>US40</td><td>Menú de navegación consistente</td><td>Como usuario quiero un menú de navegación claro y consistente en todas las páginas para encontrar fácilmente las funciones que necesito</td><td>
    <strong>Escenario 1: Navegación consistente en toda la plataforma</strong> <br>
    <strong>Dado que</strong> un usuario se encuentra en cualquier página de la aplicación, <br>
    <strong>Cuando</strong> utiliza el menú de navegación, <br>
    <strong>Entonces</strong> encuentra las mismas opciones organizadas de manera idéntica, <br>
    <strong>Y</strong> puede acceder a funciones principales desde cualquier página, <br>
    <strong>Y</strong> el menú se adapta apropiadamente a diferentes tamaños de pantalla, <br>
    <strong>Y</strong> indica claramente la ubicación actual del usuario. <br><br>
    
  <strong>Escenario 2: Menú adaptado a permisos de usuario</strong> <br>
    <strong>Dado que</strong> usuarios con diferentes roles acceden al sistema, <br>
    <strong>Cuando</strong> navegan por la plataforma, <br>
    <strong>Entonces</strong> ven solo opciones de menú apropiadas para su rol, <br>
    <strong>Y</strong> las opciones restringidas no aparecen para evitar confusión, <br>
    <strong>Y</strong> pueden identificar fácilmente todas las funciones disponibles para ellos.
    </td><td>EP11</td>
  </tr>
  <tr>
    <td>US41</td><td>Paleta de colores y tipografía</td><td>Como usuario quiero una interfaz con colores y tipografía consistentes para tener una experiencia visual agradable y fácil de leer</td><td>
    <strong>Escenario 1: Aplicación consistente de diseño visual</strong> <br>
    <strong>Dado que</strong> se muestra cualquier página de la plataforma Veyra, <br>
    <strong>Cuando</strong> un usuario navega por diferentes secciones, <br>
    <strong>Entonces</strong> encuentra colores y tipografía consistentes en toda la experiencia, <br>
    <strong>Y</strong> el diseño refleja profesionalismo apropiado para servicios de salud, <br>
    <strong>Y</strong> el contraste de colores cumple estándares de accesibilidad, <br>
    <strong>Y</strong> la tipografía es legible en diferentes dispositivos y tamaños. <br><br>
    
  <strong>Escenario 2: Adaptación para usuarios con necesidades especiales</strong> <br>
    <strong>Dado que</strong> usuarios con dificultades visuales acceden a la plataforma, <br>
    <strong>Cuando</strong> acceden a la plataforma, <br>
    <strong>Entonces</strong> pueden utilizar funciones de alto contraste o aumento de texto, <br>
    <strong>Y</strong> todos los elementos mantienen legibilidad en diferentes configuraciones, <br>
    <strong>Y</strong> los colores no son el único medio para transmitir información importante.
    </td><td>EP11</td>
  </tr>
  <tr>
    <td>US42</td><td>Diseño de formularios usables</td><td>Como usuario quiero formularios claros y fáciles de completar para ingresar información sin confusión ni errores</td><td>
    <strong>Escenario 1: Completar formularios de manera eficiente</strong> <br>
    <strong>Dado que</strong> un usuario está completando cualquier formulario en la plataforma, <br>
    <strong>Cuando</strong> ingresa información requerida, <br>
    <strong>Entonces</strong> los campos están claramente etiquetados y organizados lógicamente, <br>
    <strong>Y</strong> recibe validación en tiempo real para campos incorrectos, <br>
    <strong>Y</strong> puede guardar progreso para completar posteriormente si es formulario largo, <br>
    <strong>Y</strong> recibe confirmación clara al completar exitosamente. <br><br>
    
  <strong>Escenario 2: Formulario con errores de validación</strong> <br>
    <strong>Dado que</strong> un usuario está enviando formulario con información incorrecta, <br>
    <strong>Cuando</strong> existen errores en los datos ingresados, <br>
    <strong>Entonces</strong> recibe mensajes de error específicos y constructivos, <br>
    <strong>Y</strong> se mantiene toda la información correcta ya ingresada, <br>
    <strong>Y</strong> puede corregir errores fácilmente sin empezar desde cero.
    </td><td>EP11</td>
  </tr>
  <tr>
    <td>US43</td><td>Patrones de diseño coherentes</td><td>Como usuario quiero que todas las pantallas sigan patrones de diseño similares para predecir dónde encontrar funciones y cómo interactuar</td><td>
    <strong>Escenario 1: Interacción predecible en toda la plataforma</strong> <br>
    <strong>Dado que</strong> un usuario está familiarizado con una sección de la plataforma, <br>
    <strong>Cuando</strong> navega a nuevas secciones, <br>
    <strong>Entonces</strong> encuentra patrones de interacción similares y predecibles, <br>
    <strong>Y</strong> botones, enlaces y controles funcionan de manera consistente, <br>
    <strong>Y</strong> puede aplicar conocimiento previo para usar nuevas funcionalidades, <br>
    <strong>Y</strong> la experiencia se siente uniforme y profesional. <br><br>
    
  <strong>Escenario 2: Nuevos usuarios aprendiendo la interfaz</strong> <br>
  <strong>Dado que</strong> un nuevo usuario está accediendo por primera vez, <br>
  <strong>Cuando</strong> explora diferentes funcionalidades, <br>
  <strong>Entonces</strong> puede predecir cómo funcionarán nuevas secciones basándose en experiencia previa, <br>
   <strong>Y</strong> encuentra elementos de interfaz en ubicaciones esperadas, <br>
   <strong>Y</strong> puede desarrollar eficiencia rápidamente en el uso del sistema.
   </td><td>EP11</td>
  </tr>
  <tr>
    <td>US44</td><td>Manejo de errores comprensible</td><td>Como usuario quiero que los errores se presenten de forma clara y con soluciones sugeridas para resolver problemas sin frustración</td><td>
    <strong>Escenario 1: Error del sistema con guía de resolución</strong> <br>
    <strong>Dado que</strong> ocurre un error técnico durante el uso de la plataforma, <br>
    <strong>Cuando</strong> ocurre un problema de sistema o conectividad, <br>
    <strong>Entonces</strong> el usuario recibe mensaje claro explicando qué ocurrió, <br>
    <strong>Y</strong> se proporcionan pasos específicos para resolver el problema, <br>
    <strong>Y</strong> se ofrecen alternativas de contacto si el problema persiste, <br>
    <strong>Y</strong> se registra el error para mejora continua del sistema. <br><br>
    
  <strong>Escenario 2: Error de usuario con orientación educativa</strong> <br>
    <strong>Dado que</strong> un usuario comete un error en el uso de la plataforma, <br>
    <strong>Cuando</strong> realiza una acción incorrecta o no permitida, <br>
    <strong>Entonces</strong> recibe explicación clara sobre por qué no se pudo completar la acción, <br>
    <strong>Y</strong> se le orienta sobre la forma correcta de proceder, <br>
    <strong>Y</strong> puede corregir fácilmente su acción sin frustración, <br>
    <strong>Y</strong> aprende a evitar el mismo error en el futuro.
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
