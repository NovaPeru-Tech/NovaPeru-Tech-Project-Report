# Capítulo III: Requirements Specification

## 3.1. User Stories</em></h2>
<p>Para la especificación de requisitos de los usuarios, se desarrollaron las historias de usuario que describen cada requisito y funcionalidad que debe estar implementado en el desarrollo del producto final para satisfacer las necesidades del público objetivo. A continuación se presentan las historias de usuario relacionadas con la plataforma "Veyra". Esta sección reúne historias de usuario centradas en la experiencia de los distintos roles: el visitante, el familiar del adulto mayor y el administrador de la casa de reposo. Aquí se definen las necesidades clave para cada uno, desde la navegación inicial y contacto, hasta la gestión detallada de residentes, personal y medicamentos.</p>

  <table>
        <thead>
            <tr>
                <th>Story ID</th>
                <th>Título</th>
                <th>Descripción</th>
                <th>Criterios de Aceptación (Gherkin)</th>
            </tr>
        </thead>
        <tbody>
                <tr>
                <td>EP01</td>
                <td>Navegación en la Landing Page</td>
                <td>Como visitante quiero tener una experiencia fluida y completa en el sitio web para conocer los servicios y tomar decisiones informadas.</td>
                <td></td>
            </tr>
            <tr>
            <tr>
                <td>US01</td>
                <td>Menú de navegación</td>
                <td>Como visitante de la Landing Page, quiero poder acceder a un menú de navegación en la parte superior de la página, para explorar fácilmente las secciones como "Log in", "Sign up", "Planes", "Contacto",etc.</td>
                <td>
                    <strong>Escenario 1: Menú visible y navegable</strong><br>
                    <strong>Dado que</strong> el visitante está en la landing page,<br>
                    <strong>Cuando</strong> la página carga y selecciona un enlace del menú,<br>
                    <strong>Entonces</strong> el menú se muestra con enlaces principales ("Log in", "Sign up", "Planes", "Contacto") y redirige correctamente.<br><br>
                    <strong>Escenario 2: Menú no carga o enlace roto</strong><br>
                    <strong>Dado que</strong> el visitante está en la landing page,<br>
                    <strong>Cuando</strong> el menú no se visualiza o un enlace falla,<br>
                    <strong>Entonces</strong> se muestra un mensaje de error y se ofrecen enlaces alternativos.
                </td>
            </tr>
            <tr>
                <td>US02</td>
                <td>Visualización de Planes</td>
                <td>Como visitante de la Landing Page, quiero ver los planes de suscripción junto a su precio y características, para poder elegir el que mejor se adapte a mis necesidades.</td>
                <td>
                    <strong>Escenario 1: Visualización correcta de planes</strong><br>
                    <strong>Dado que</strong> un visitante está en la sección de planes,<br>
                    <strong>Cuando</strong> la página carga,<br>
                    <strong>Entonces</strong> ve al menos 2 planes con precio, características y botón de selección, y puede compararlos.<br><br>
                    <strong>Escenario 2: Error en carga de planes</strong><br>
                    <strong>Dado que</strong> un visitante está en la sección de planes,<br>
                    <strong>Cuando</strong> ocurre un error de carga,<br>
                    <strong>Entonces</strong> se muestra un mensaje de error, una opción de recarga y contacto alternativo.
                </td>
            </tr>
            <tr>
                <td>US03</td>
                <td>Selección de Plan en Landing Page</td>
                <td>Como visitante de la landing Page, quiero seleccionar un plan y finalizar la confirmación en la misma pantalla, para agilizar y simplificar el registro.</td>
                <td>
                    <strong>Escenario 1: Selección y confirmación exitosa</strong><br>
                    <strong>Dado que</strong> un visitante ve los planes disponibles,<br>
                    <strong>Cuando</strong> selecciona un plan y pulsa "Seleccionar",<br>
                    <strong>Entonces</strong> se muestra un formulario en la misma pantalla con el plan seleccionado para completar y confirmar.<br><br>
                    <strong>Escenario 2: Selección sin completar datos requeridos</strong><br>
                    <strong>Dado que</strong> un visitante está en el formulario de confirmación,<br>
                    <strong>Cuando</strong> intenta confirmar sin datos obligatorios,<br>
                    <strong>Entonces</strong> se muestran mensajes de validación específicos y mantiene los datos ingresados.
                </td>
            </tr>
            <tr>
                <td>US04</td>
                <td>Visualización de creadores</td>
                <td>Como visitante de la Landing Page, quiero ver a los creadores de la aplicación, para conocer al equipo detrás del producto y generar confianza en el servicio.</td>
                <td>
                    <strong>Escenario 1: Acceso exitoso a información del equipo</strong><br>
                    <strong>Dado que</strong> un visitante está en la landing page,<br>
                    <strong>Cuando</strong> navega a la sección "Equipo",<br>
                    <strong>Entonces</strong> ve la información de cada creador (nombre, foto, rol) y sus perfiles sociales si existen.<br><br>
                    <strong>Escenario 2: Información de equipo no disponible</strong><br>
                    <strong>Dado que</strong> un visitante está intentando acceder a la info del equipo,<br>
                    <strong>Cuando</strong> la sección no carga correctamente,<br>
                    <strong>Entonces</strong> se muestra un mensaje explicativo y contacto alternativo.
                </td>
            </tr>
            <tr>
                <td>US07</td>
                <td>Cambio de idioma</td>
                <td>Como visitante del Landing Page quiero en el menú un botón para cambiar de idioma entre español e inglés para entender mejor de que trata Veyra.</td>
                <td>
                    <strong>Escenario 1: Cambio exitoso de idioma</strong><br>
                    <strong>Dado que</strong> un visitante está en la landing page en español,<br>
                    <strong>Cuando</strong> selecciona la opción de cambio y elige inglés,<br>
                    <strong>Entonces</strong> toda la interfaz cambia a inglés y la preferencia se mantiene al navegar.<br><br>
                    <strong>Escenario 2: Idioma no disponible temporalmente</strong><br>
                    <strong>Dado que</strong> un visitante intenta cambiar de idioma,<br>
                    <strong>Cuando</strong> el servicio de traducción no está disponible,<br>
                    <strong>Entonces</strong> se muestra un mensaje informativo y se mantiene el idioma actual.
                </td>
            </tr>
            <tr>
                <td>US39</td>
                <td>Términos y condiciones</td>
                <td>Como visitante de la landing page quiero poder acceder a los términos y condiciones de uso para conocer las políticas legales antes de contratar los servicios.</td>
                <td>
                    <strong>Escenario 1: Acceso exitoso a términos y condiciones</strong><br>
                    <strong>Dado que</strong> un visitante se encuentra en la landing page,<br>
                    <strong>Cuando</strong> busca los términos y condiciones de uso,<br>
                    <strong>Entonces</strong> accede al documento completo (claro y actualizado) desde el footer o header.<br><br>
                    <strong>Escenario 2: Aceptación requerida de términos actualizados</strong><br>
                    <strong>Dado que</strong> los términos y condiciones han sido actualizados,<br>
                    <strong>Cuando</strong> un usuario existente ingresa al sistema,<br>
                    <strong>Entonces</strong> debe revisar y aceptar los nuevos términos (con cambios destacados) antes de continuar.
                </td>
            </tr>
        </tbody>
           <tr>
                <td>EP02</td>
                <td>Soporte y contacto</td>
                <td>Como visitante de la Landing Page, quiero poder contactar a Veyra fácilmente, para resolver dudas o interactuar.</td>
                <td></td>
            </tr>
            <tr>
                <td>US05</td>
                <td>Redes sociales</td>
                <td>Como visitante del landing page quiero poder acceder fácilmente a sus redes sociales de Veyra para conocer más sobre la empresa y tener canales adicionales de contacto.</td>
                <td>
                    <strong>Escenario 1: Acceso exitoso a redes sociales</strong><br>
                    <strong>Dado que</strong> un visitante está en la landing page,<br>
                    <strong>Cuando</strong> busca enlaces de redes sociales (footer/header) y activa un ícono,<br>
                    <strong>Entonces</strong> encuentra los íconos y se abre la página oficial en una nueva pestaña.<br><br>
                    <strong>Escenario 2: Enlaces de redes sociales no funcionales</strong><br>
                    <strong>Dado que</strong> un visitante intenta acceder a redes sociales,<br>
                    <strong>Cuando</strong> interactúa con un ícono que no responde,<br>
                    <strong>Entonces</strong> recibe un mensaje de error informativo y contacto alternativo.
                </td>
            </tr>
            <tr>
                <td>US06</td>
                <td>Formulario de contacto</td>
                <td>Como visitante del landing page quiero completar un formulario de contacto para enviar consultas específicas y recibir una respuesta personalizada de Veyra.</td>
                <td>
                    <strong>Escenario 1: Envío exitoso de consulta</strong><br>
                    <strong>Dado que</strong> un visitante está en el formulario de contacto,<br>
                    <strong>Cuando</strong> completa campos requeridos (nombre, email, asunto, mensaje) y pulsa "Enviar",<br>
                    <strong>Entonces</strong> recibe confirmación de envío, tiempo estimado de respuesta y copia por email.<br><br>
                    <strong>Escenario 2: Formulario con datos inválidos</strong><br>
                    <strong>Dado que</strong> un visitante está completando el formulario,<br>
                    <strong>Cuando</strong> ingresa un email inválido o deja campos obligatorios vacíos e intenta enviar,<br>
                    <strong>Entonces</strong> se muestran mensajes de validación específicos y se mantiene la información correcta.
                </td>
            </tr>
        </tbody>
          <tr>
                <td>EP03</td>
                <td>Acceso a Información</td>
                <td>Como familiar del adulto mayor quiero poder tener acceso a toda la información de mi familiar para estar informado de su estado.</td>
                <td></td>
            </tr>
            <tr>
                <td>US08</td>
                <td>Historial médico</td>
                <td>Como familiar de un adulto mayor quiero acceder al historial médico completo de mi familiar para conocer su evolución de salud y diagnósticos actuales.</td>
                <td>
                    <strong>Escenario 1: Acceso exitoso al historial médico</strong><br>
                    <strong>Dado que</strong> un familiar está autenticado,<br>
                    <strong>Cuando</strong> navega a la sección "Historial Médico",<br>
                    <strong>Entonces</strong> ve diagnósticos, evolución y actualizaciones, organizados cronológicamente y filtrables.<br><br>
                    <strong>Escenario 2: Sin permisos para acceder a reportes</strong><br>
                    <strong>Dado que</strong> un usuario intenta acceder al historial médico,<br>
                    <strong>Cuando</strong> no tiene los permisos necesarios,<br>
                    <strong>Entonces</strong> se muestra un mensaje de restricción e información para obtener permisos.
                </td>
            </tr>
            <tr>
                <td>US09</td>
                <td>Agenda de citas Medicas</td>
                <td>Como familiar de un adulto mayor quiero consultar la agenda de citas médicas de mi familiar para estar informado sobre sus próximos tratamientos.</td>
                <td>
                    <strong>Escenario 1: Visualización exitosa de citas programadas</strong><br>
                    <strong>Dado que</strong> un familiar está autenticado,<br>
                    <strong>Cuando</strong> accede a la agenda de citas,<br>
                    <strong>Entonces</strong> ve todas las citas programadas (fecha, hora, médico, tipo) y puede filtrar por fechas.<br><br>
                    <strong>Escenario 2: No hay citas programadas</strong><br>
                    <strong>Dado que</strong> un familiar consulta la agenda,<br>
                    <strong>Cuando</strong> no hay citas programadas,
                    <strong>Entonces</strong> se muestra un mensaje informativo indicando que no hay citas y cómo programar.
                </td>
            </tr>
            <tr>
                <td>US10</td>
                <td>Consulta de información personal</td>
                <td>Como familiar de un adulto mayor quiero ver la información de mi familiar para estar seguro de que esté correcto o actualizado.</td>
                <td>
                    <strong>Escenario 1: Visualización exitosa de información personal</strong><br>
                    <strong>Dado que</strong> un familiar está autenticado,<br>
                    <strong>Cuando</strong> accede al perfil de información personal,<br>
                    <strong>Entonces</strong> ve datos actualizados (nombre, edad, contacto emergencia, alergias, etc.) y tiene opciones para solicitar modificaciones.<br><br>
                    <strong>Escenario 2: Información desactualizada detectada</strong><br>
                    <strong>Dado que</strong> un familiar revisa información personal,<br>
                    <strong>Cuando</strong> identifica información que necesita actualización,<br>
                    <strong>Entonces</strong> puede marcar campos y enviar solicitudes de cambio con justificación.
                </td>
            </tr>
            <tr>
                <td>US11</td>
                <td>Galería de fotos y actividades</td>
                <td>Como familiar de un adulto mayor quiero ver fotos de las actividades diarias de mi familiar para sentirme conectado con su día a día y verificar su participación social.</td>
                <td>
                    <strong>Escenario 1: Acceso exitoso a galería de actividades</strong><br>
                    <strong>Dado que</strong> un familiar está autenticado,<br>
                    <strong>Cuando</strong> accede a la galería de fotos,<br>
                    <strong>Entonces</strong> ve fotos organizadas por fecha/actividad, con descripción, y puede filtrar.<br><br>
                    <strong>Escenario 2: Sin actividades recientes registradas</strong><br>
                    <strong>Dado que</strong> un familiar consulta la galería,<br>
                    <strong>Cuando</strong> no hay fotos recientes de actividades,<br>
                    <strong>Entonces</strong> se muestra un mensaje informativo y la frecuencia de actualización.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP04</td>
                <td>Gestión de adultos mayores</td>
                <td>Como administrador de casa de reposo quiero gestionar perfiles de los adultos mayores para tener un mayor control.</td>
                <td></td>
            </tr>
            <tr>
            <tr>
                <td>US12</td>
                <td>Registro de residentes</td>
                <td>Como administrador de casa de reposo quiero crear y mantener perfiles completos de cada residente para centralizar toda su información personal y médica.</td>
                <td>
                    <strong>Escenario 1: Creación exitosa de perfil de residente</strong><br>
                    <strong>Dado que</strong> un administrador está autenticado,<br>
                    <strong>Cuando</strong> completa el formulario de registro con toda la información requerida,<br>
                    <strong>Entonces</strong> el perfil se crea exitosamente y se genera un ID único.<br><br>
                    <strong>Escenario 2: Error en datos requeridos para registro</strong><br>
                    <strong>Dado que</strong> un administrador está creando un perfil,<br>
                    <strong>Cuando</strong> falta información crítica requerida e intenta guardar,<br>
                    <strong>Entonces</strong> se muestran mensajes específicos de campos faltantes y se mantiene la data ingresada.
                </td>
            </tr>
            <tr>
                <td>US13</td>
                <td>Historial médico institucional</td>
                <td>Como administrador quiero gestionar el historial médico completo de cada residente para asegurar continuidad en el cuidado y cumplir con regulaciones sanitarias.</td>
                <td>
                    <strong>Escenario 1: Gestión exitosa de historial médico completo</strong><br>
                    <strong>Dado que</strong> un administrador tiene permisos médicos,<br>
                    <strong>Cuando</strong> accede al historial médico de un residente,<br>
                    <strong>Entonces</strong> puede ver, agregar y actualizar información (diagnósticos, tratamientos), quedando registrado con fecha y responsable.<br><br>
                    <strong>Escenario 2: Acceso sin permisos médicos suficientes</strong><br>
                    <strong>Dado que</strong> un usuario intenta acceder al historial institucional,<br>
                    <strong>Cuando</strong> no posee los permisos necesarios,<br>
                    <strong>Entonces</strong> se restringe el acceso con un mensaje explicativo.
                </td>
            </tr>
            <tr>
                <td>US14</td>
                <td>Administración de medicamentos</td>
                <td>Como administrador quiero controlar la administración de medicamentos de todos los residentes para garantizar cumplimiento de tratamientos y evitar errores médicos.</td>
                <td>
                    <strong>Escenario 1: Control exitoso de administración de medicamentos</strong><br>
                    <strong>Dado que</strong> un administrador está en el módulo de medicamentos,<br>
                    <strong>Cuando</strong> registra la administración de medicamentos,<br>
                    <strong>Entonces</strong> puede marcarla con hora exacta, registrar observaciones y el sistema alerta sobre próximas dosis.<br><br>
                    <strong>Escenario 2: Medicamento no disponible en inventario</strong><br>
                    <strong>Dado que</strong> un administrador intenta registrar una administración,<br>
                    <strong>Cuando</strong> el medicamento no está disponible en inventario,<br>
                    <strong>Entonces</strong> el sistema muestra alerta de falta de stock y proporciona opciones de contacto.
                </td>
            </tr>
            <tr>
                <td>US15</td>
                <td>Gestión de visitas familiares</td>
                <td>Como administrador quiero controlar y programar las visitas familiares a los residentes para mantener seguridad, orden y cumplir con los horarios establecidos.</td>
                <td>
                    <strong>Escenario 1: Programación exitosa de visita familiar</strong><br>
                    <strong>Dado que</strong> un administrador está en el módulo de visitas,<br>
                    <strong>Cuando</strong> programa una nueva visita (fecha, hora, visitantes, residente),<br>
                    <strong>Entonces</strong> el sistema verifica disponibilidad, genera confirmación y envía recordatorios automáticos.<br><br>
                    <strong>Escenario 2: Conflicto de horarios en visitas</strong><br>
                    <strong>Dado que</strong> un administrador está programando una visita,<br>
                    <strong>Cuando</strong> el horario solicitado ya está ocupado,<br>
                    <strong>Entonces</strong> el sistema muestra horarios alternativos disponibles y permite reprogramar.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP05</td>
                <td>Notificaciones automáticas</td>
                <td>Como familiar de un adulto mayor, quiero recibir notificaciones automáticas sobre cambios en su estado o recordatorios importantes, para estar siempre informado sin tener que consultar manualmente la plataforma.</td>
                <td></td>
            </tr>
            <tr>
                <td>US16</td>
                <td>Recordatorios de citas y consultas</td>
                <td>Como familiar quiero recibir recordatorios automáticos sobre citas médicas y consultas programadas de mi familiar para estar preparado y decidir si deseo acompañarlo.</td>
                <td>
                    <strong>Escenario 1: Envío exitoso de recordatorios automáticos</strong><br>
                    <strong>Dado que</strong> el sistema tiene citas médicas programadas,<br>
                    <strong>Cuando</strong> se acerca una cita (ej. 24 horas antes),<br>
                    <strong>Entonces</strong> se envía recordatorio automático (email/SMS) a familiares con detalles, y pueden confirmar.<br><br>
                    <strong>Escenario 2: Falla en envío de recordatorios</strong><br>
                    <strong>Dado que</strong> el sistema intenta enviar recordatorios,<br>
                    <strong>Cuando</strong> falla el servicio de notificaciones,<br>
                    <strong>Entonces</strong> se registra el error, se intenta reenvío automático y se notifica al administrador.
                </td>
            </tr>
            <tr>
                <td>US17</td>
                <td>Notificaciones de cambios en medicación</td>
                <td>Como familiar quiero ser notificado inmediatamente sobre cualquier cambio en la medicación de mi familiar para estar informado sobre su tratamiento médico.</td>
                <td>
                    <strong>Escenario 1: Notificación inmediata de cambio en medicación</strong><br>
                    <strong>Dado que</strong> ha ocurrido un cambio en la medicación,<br>
                    <strong>Cuando</strong> el médico actualiza el tratamiento farmacológico,<br>
                    <strong>Entonces</strong> se envía notificación inmediata a familiares autorizados con detalles del cambio y justificación.<br><br>
                    <strong>Escenario 2: Familiar no autorizado para recibir información médica</strong><br>
                    <strong>Dado que</strong> ha ocurrido un cambio en la medicación,<br>
                    <strong>Cuando</strong> un familiar no está autorizado para recibir esa información,<br>
                    <strong>Entonces</strong> no recibe la notificación, respetando las preferencias de privacidad.
                </td>
            </tr>
            <tr>
                <td>US18</td>
                <td>Recordatorios de visitas familiares</td>
                <td>Como familiar quiero recibir recordatorios automáticos sobre mis visitas programadas al adulto mayor para no olvidar las citas y mantener regularidad en el contacto.</td>
                <td>
                    <strong>Escenario 1: Recordatorio exitoso de visita programada</strong><br>
                    <strong>Dado que</strong> hay una visita familiar programada,<br>
                    <strong>Cuando</strong> faltan 2 horas para la visita,<br>
                    <strong>Entonces</strong> se envía recordatorio automático al familiar (fecha, hora, residente) y puede confirmar/cancelar.<br><br>
                    <strong>Escenario 2: Cancelación de visita por emergencia</strong><br>
                    <strong>Dado que</strong> hay una visita familiar programada,<br>
                    <strong>Cuando</strong> ocurre una emergencia que requiere cancelar la visita,<br>
                    <strong>Entonces</strong> se envía notificación inmediata de cancelación con explicación y alternativas.
                </td>
            </tr>
            <tr>
                <td>US19</td>
                <td>Alertas de actualización de datos personales</td>
                <td>Como familiar quiero recibir notificaciones automáticas cuando se actualice la información personal o de mi familiar para mantenerme informado de cualquier cambio en su perfil.</td>
                <td>
                    <strong>Escenario 1: Notificación exitosa de actualización de datos</strong><br>
                    <strong>Dado que</strong> ha ocurrido una actualización en los datos personales del residente,<br>
                    <strong>Cuando</strong> se modifica información (ej. contacto de emergencia, estado de salud),<br>
                    <strong>Entonces</strong> se envía notificación a familiares autorizados especificando qué información fue actualizada.<br><br>
                    <strong>Escenario 2: Actualización sin autorización para notificar</strong><br>
                    <strong>Dado que</strong> ha ocurrido una actualización de datos,<br>
                    <strong>Cuando</strong> el familiar no tiene autorización para recibir ese tipo de información,<br>
                    <strong>Entonces</strong> no recibe notificación sobre datos restringidos, respetando la privacidad.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP06</td>
                <td>Comunicación con cuidadores</td>
                <td>Como familiar, quiero disponer de un canal de comunicación directo con los cuidadores o el personal de la casa de reposo, para hacer preguntas y recibir respuestas rápidas sobre el cuidado de mi adulto mayor.</td>
                <td></td>
            </tr>
            <tr>
                <td>US20</td>
                <td>Preguntas sobre rutina de cuidados</td>
                <td>Como familiar quiero hacer preguntas específicas sobre la rutina diaria y cuidados de mi familiar para entender mejor su día a día y resolver dudas puntuales.</td>
                <td>
                    <strong>Escenario 1: Envío exitoso de pregunta sobre cuidados</strong><br>
                    <strong>Dado que</strong> un familiar está autenticado en el sistema de comunicación,<br>
                    <strong>Cuando</strong> redacta y envía una pregunta específica sobre cuidados,<br>
                    <strong>Entonces</strong> la consulta se envía al personal asignado, recibe confirmación y tiempo estimado de respuesta.<br><br>
                    <strong>Escenario 2: Canal de comunicación no disponible</strong><br>
                    <strong>Dado que</strong> un familiar intenta enviar una pregunta,<br>
                    <strong>Cuando</strong> el sistema de comunicación no está disponible,<br>
                    <strong>Entonces</strong> se muestra un mensaje temporal y se proporcionan números de teléfono alternativos.
                </td>
            </tr>
            <tr>
                <td>US21</td>
                <td>Peticiones de modificación de cuidados</td>
                <td>Como familiar quiero solicitar ajustes específicos en el cuidado de mi familiar basados en sus preferencias o necesidades particulares.</td>
                <td>
                    <strong>Escenario 1: Solicitud exitosa de modificación de cuidados</strong><br>
                    <strong>Dado que</strong> un familiar (con permisos) solicita un cambio en cuidados,<br>
                    <strong>Cuando</strong> envía una petición detallada,<br>
                    <strong>Entonces</strong> la solicitud se registra con N° de seguimiento, se notifica al coordinador y recibe plazos de evaluación.<br><br>
                    <strong>Escenario 2: Solicitud que requiere aprobación médica</strong><br>
                    <strong>Dado que</strong> un familiar solicita una modificación,<br>
                    <strong>Cuando</strong> la petición involucra aspectos médicos o terapéuticos,<br>
                    <strong>Entonces</strong> se deriva automáticamente al equipo médico y se informa al familiar sobre el proceso.
                </td>
            </tr>
            <tr>
                <td>US22</td>
                <td>Seguimiento del bienestar emocional</td>
                <td>Como familiar quiero comunicarme con el personal sobre el estado emocional y psicológico de mi familiar para asegurar su bienestar integral.</td>
                <td>
                    <strong>Escenario 1: Comunicación exitosa sobre estado emocional</strong><br>
                    <strong>Dado que</strong> un familiar está preocupado por el bienestar emocional,<br>
                    <strong>Cuando</strong> envía consulta sobre estado anímico o adaptación,<br>
                    <strong>Entonces</strong> se comunica con psicología/trabajo social y recibe respuesta profesional y recomendaciones.<br><br>
                    <strong>Escenario 2: Situación emocional que requiere atención inmediata</strong><br>
                    <strong>Dado que</strong> un familiar reporta cambios emocionales significativos,<br>
                    <strong>Cuando</strong> la situación indica posible crisis emocional,<br>
                    <strong>Entonces</strong> se escalona a atención psicológica prioritaria y se coordina intervención con el familiar.
                </td>
            </tr>
            <tr>
                <td>US23</td>
                <td>Planificación de eventos familiares</td>
                <td>Como familiar quiero coordinar con el personal la organización de eventos especiales o celebraciones para mi familiar dentro de las instalaciones.</td>
                <td>
                    <strong>Escenario 1: Coordinación exitosa de evento familiar</strong><br>
                    <strong>Dado que</strong> un familiar planifica un evento especial (ej. cumpleaños),<br>
                    <strong>Cuando</strong> solicita coordinación especificando fecha, invitados y requerimientos,<br>
                    <strong>Entonces</strong> el personal evalúa viabilidad, coordina espacios/recursos y envía confirmación.<br><br>
                    <strong>Escenario 2: Evento que no cumple con protocolos institucionales</strong><br>
                    <strong>Dado que</strong> un familiar solicita un evento,<br>
                    <strong>Cuando</strong> la solicitud involucra aspectos no permitidos por políticas institucionales,<br>
                    <strong>Entonces</strong> se explican las limitaciones y se ofrecen alternativas que cumplan con protocolos.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP07</td>
                <td>Gestión de medicamentos</td>
                <td>Como administrador quiero gestionar los medicamentos de la casa de reposo para garantizar que cumplan con todos los controles necesarios.</td>
                <td></td>
            </tr>
            <tr>
                <td>US24</td>
                <td>Registro de medicamentos en inventario</td>
                <td>Como administrador quiero registrar todos los medicamentos que ingresan al inventario con sus datos completos para mantener un catálogo actualizado.</td>
                <td>
                    <strong>Escenario 1: Registro exitoso de medicamentos</strong><br>
                    <strong>Dado que</strong> un administrador está en el módulo de inventario,<br>
                    <strong>Cuando</strong> registra un nuevo medicamento con datos requeridos (nombre, lote, vencimiento, cantidad),<br>
                    <strong>Entonces</strong> se añade al inventario, se genera ID, se actualiza stock y se registra el ingreso (fecha, responsable).<br><br>
                    <strong>Escenario 2: Medicamento duplicado en inventario</strong><br>
                    <strong>Dado que</strong> un administrador está registrando un medicamento,<br>
                    <strong>Cuando</strong> intenta ingresar un medicamento que ya existe con el mismo lote,<br>
                    <strong>Entonces</strong> el sistema detecta la duplicación, muestra alerta y permite actualizar la cantidad del lote existente.
                </td>
            </tr>
            <tr>
                <td>US25</td>
                <td>Alertas de vencimiento</td>
                <td>Como administrador quiero recibir alertas automáticas sobre medicamentos próximos a vencer para evitar pérdidas y riesgos de seguridad.</td>
                <td>
                    <strong>Escenario 1: Generación de alerta por medicamentos próximos a vencer</strong><br>
                    <strong>Dado que</strong> hay medicamentos en inventario próximos a vencer,<br>
                    <strong>Cuando</strong> faltan 30 días para la fecha de vencimiento,<br>
                    <strong>Entonces</strong> se genera alerta automática al admin (lista, cantidades, fechas) y se sugieren acciones.<br><br>
                    <strong>Escenario 2: Medicamentos ya vencidos en inventario</strong><br>
                    <strong>Dado que</strong> hay medicamentos que han superado su fecha de vencimiento,<br>
                    <strong>Cuando</strong> el sistema detecta medicamentos vencidos,<br>
                    <strong>Entonces</strong> se bloquea automáticamente su uso, se genera alerta crítica y se registra la pérdida.
                </td>
            </tr>
            <tr>
                <td>US26</td>
                <td>Eliminación de medicamentos</td>
                <td>Como administrador quiero eliminar medicamentos del inventario de manera controlada para mantener la precisión del stock y cumplir con protocolos de disposición.</td>
                <td>
                    <strong>Escenario 1: Eliminación controlada de medicamento</strong><br>
                    <strong>Dado que</strong> un administrador necesita eliminar un medicamento,<br>
                    <strong>Cuando</strong> selecciona el medicamento, especifica la razón (vencido, dañado, usado) y justifica,<br>
                    <strong>Entonces</strong> el sistema registra la eliminación (fecha, cantidad, responsable), actualiza stock y genera reporte.<br><br>
                    <strong>Escenario 2: Intento de eliminación sin autorización</strong><br>
                    <strong>Dado que</strong> un usuario intenta eliminar un medicamento,<br>
                    <strong>Cuando</strong> no posee los permisos necesarios,<br>
                    <strong>Entonces</strong> el sistema niega el acceso, registra el intento y notifica al administrador.
                </td>
            </tr>
            <tr>
                <td>US27</td>
                <td>Búsqueda y filtrado de inventario</td>
                <td>Como administrador quiero filtrar y buscar medicamentos en el inventario para encontrar rápidamente información específica y generar reportes personalizados.</td>
                <td>
                    <strong>Escenario 1: Búsqueda exitosa de medicamentos</strong><br>
                    <strong>Dado que</strong> un administrador está en el módulo de inventario,<br>
                    <strong>Cuando</strong> utiliza filtros de búsqueda (nombre, laboratorio, vencimiento, categoría),<br>
                    <strong>Entonces</strong> obtiene resultados precisos, ordenables y puede exportarlos.<br><br>
                    <strong>Escenario 2: Búsqueda sin resultados</strong><br>
                    <strong>Dado que</strong> un administrador está buscando un medicamento,<br>
                    <strong>Cuando</strong> los criterios de búsqueda no coinciden,<br>
                    <strong>Entonces</strong> se muestra un mensaje "sin resultados" y se sugieren búsquedas alternativas.
                </td>
            </tr>
            <tr>
                <td>US28</td>
                <td>Información de medicamentos para personal</td>
                <td>Como administrador quiero proporcionar información detallada sobre medicamentos al personal para asegurar administración segura y correcta.</td>
                <td>
                    <strong>Escenario 1: Acceso exitoso a información detallada de medicamentos</strong><br>
                    <strong>Dado que</strong> personal autorizado está consultando información,<br>
                    <strong>Cuando</strong> accede a detalles de un medicamento específico,<br>
                    <strong>Entonces</strong> ve información completa (dosificación, contraindicaciones, etc.) y protocolos de administración.<br><br>
                    <strong>Escenario 2: Medicamento con alertas especiales</strong><br>
                    <strong>Dado que</strong> personal consulta un medicamento,<br>
                    <strong>Cuando</strong> este tiene alertas de seguridad o administración especial,<br>
                    <strong>Entonces</strong> se muestran las alertas prominentemente y se requiere confirmación de lectura.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP08</td>
                <td>Gestión de personal</td>
                <td>Como administrador de la casa de reposo, quiero gestionar la información del personal para organizar los turnos de trabajo de los cuidadores y garantizar que siempre haya atención adecuada disponible para los residentes.</td>
                <td></td>
            </tr>
            <tr>
                <td>US29</td>
                <td>Gestión de perfiles de empleados</td>
                <td>Como administrador quiero registrar y mantener los perfiles completos del personal para tener información actualizada de todos los empleados.</td>
                <td>
                    <strong>Escenario 1: Registro exitoso de empleado</strong><br>
                    <strong>Dado que</strong> un admin de RRHH registra un nuevo empleado,<br>
                    <strong>Cuando</strong> completa la información requerida (personal, profesional, rol, contacto),<br>
                    <strong>Entonces</strong> el perfil se crea, se genera ID de empleado y se asignan permisos según el rol.<br><br>
                    <strong>Escenario 2: Información incompleta de empleado</strong><br>
                    <strong>Dado que</strong> un admin registra un empleado,<br>
                    <strong>Cuando</strong> faltan datos críticos (ej. certificaciones requeridas),<br>
                    <strong>Entonces</strong> el sistema indica qué información falta y no activa permisos hasta que esté completa.
                </td>
            </tr>
            <tr>
                <td>US30</td>
                <td>Baja de personal</td>
                <td>Como administrador quiero dar de baja empleados del sistema para mantener registros actualizados y gestionar finalizaciones de contratos.</td>
                <td>
                    <strong>Escenario 1: Proceso exitoso de baja de empleado</strong><br>
                    <strong>Dado que</strong> un admin procesa la baja de un empleado,<br>
                    <strong>Cuando</strong> especifica fecha de terminación y motivo,<br>
                    <strong>Entonces</strong> se desactivan accesos, se genera reporte de finalización y se notifica a supervisores.<br><br>
                    <strong>Escenario 2: Empleado con responsabilidades activas</strong><br>
                    <strong>Dado que</strong> un admin intenta dar de baja a un empleado,<br>
                    <strong>Cuando</strong> el empleado tiene residentes asignados o tareas críticas pendientes,<br>
                    <strong>Entonces</strong> el sistema alerta sobre responsabilidades y requiere reasignación completa antes de procesar.
                </td>
            </tr>
            <tr>
                <td>US31</td>
                <td>Búsqueda y filtrado de empleados</td>
                <td>Como administrador quiero filtrar y buscar empleados según diferentes criterios para encontrar rápidamente personal específico.</td>
                <td>
                    <strong>Escenario 1: Búsqueda exitosa de empleados</strong><br>
                    <strong>Dado que</strong> un admin se encuentra en gestión de personal,<br>
                    <strong>Cuando</strong> utiliza filtros (departamento, rol, turno, estado),<br>
                    <strong>Entonces</strong> obtiene una lista precisa de empleados y puede exportarla.<br><br>
                    <strong>Escenario 2: Filtros que no retornan resultados</strong><br>
                    <strong>Dado que</strong> un admin aplica filtros específicos,<br>
                    <strong>Cuando</strong> la combinación de filtros no coincide,<br>
                    <strong>Entonces</strong> se muestra un mensaje "sin resultados" y se sugiere modificar criterios.
                </td>
            </tr>
            <tr>
                <td>US32</td>
                <td>Gestión de horas extra</td>
                <td>Como administrador quiero controlar las horas extra trabajadas por el personal para gestionar costos laborales y cumplir con regulaciones de trabajo.</td>
                <td>
                    <strong>Escenario 1: Registro exitoso de horas extra</strong><br>
                    <strong>Dado que</strong> un admin registra horas extra,<br>
                    <strong>Cuando</strong> especifica empleado, fecha, horas y justificación,<br>
                    <strong>Entonces</strong> las horas se registran, se calculan montos según tarifas y se notifica al empleado.<br><br>
                    <strong>Escenario 2: Horas extra que exceden límites permitidos</strong><br>
                    <strong>Dado que</strong> un admin registra horas extra,<br>
                    <strong>Cuando</strong> las horas superan los máximos permitidos por regulaciones,<br>
                    <strong>Entonces</strong> el sistema muestra alerta sobre violación de límites y requiere autorización especial.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP09</td>
                <td>Gestión de información de la casa de reposo</td>
                <td>Como administrador quiero gestionar la información general de la casa de reposo para mantener datos actualizados sobre la institución.</td>
                <td></td>
            </tr>
            <tr>
                <td>US33</td>
                <td>Gestión de horarios de atención</td>
                <td>Como administrador quiero configurar los horarios de atención y servicios para informar claramente a familias sobre disponibilidad.</td>
                <td>
                    <strong>Escenario 1: Configuración exitosa de horarios</strong><br>
                    <strong>Dado que</strong> un admin configura horarios de atención,<br>
                    <strong>Cuando</strong> establece horarios por servicio, día y disponibilidad,<br>
                    <strong>Entonces</strong> los horarios se actualizan en la plataforma, las familias los ven y se sincronizan con citas.<br><br>
                    <strong>Escenario 2: Cambio de horarios por emergencia</strong><br>
                    <strong>Dado que</strong> un admin modifica horarios por emergencia,<br>
                    <strong>Cuando</strong> debe cambiar horarios por situaciones imprevistas,<br>
                    <strong>Entonces</strong> puede realizar cambios inmediatos con notificación automática a partes afectadas.
                </td>
            </tr>
            <tr>
                <td>US34</td>
                <td>Datos de contacto institucional</td>
                <td>Como administrador quiero gestionar la información de contacto de la casa de reposo para que familias y autoridades tengan acceso a datos actualizados.</td>
                <td>
                    <strong>Escenario 1: Actualización exitosa de información de contacto</strong><br>
                    <strong>Dado que</strong> un admin actualiza datos de contacto institucional,<br>
                    <strong>Cuando</strong> modifica teléfonos, emails o dirección,<br>
                    <strong>Entonces</strong> la información se actualiza en toda la plataforma (landing, apps) y se notifica a familias.<br><br>
                    <strong>Escenario 2: Información de contacto de emergencia</strong><br>
                    <strong>Dado que</strong> hay una situación de emergencia,<br>
                    <strong>Cuando</strong> familias necesitan contactar urgentemente,<br>
                    <strong>Entonces</strong> tienen acceso inmediato a números de emergencia 24/7 y reciben respuesta rápida.
                </td>
            </tr>
            <tr>
                <td>US35</td>
                <td>Información del personal directivo</td>
                <td>Como administrador quiero gestionar la información del personal directivo para transparencia hacia familias y autoridades.</td>
                <td>
                    <strong>Escenario 1: Gestión de información de personal directivo</strong><br>
                    <strong>Dado que</strong> un admin actualiza información de personal directivo,<br>
                    <strong>Cuando</strong> modifica información de directores o coordinadores clave,<br>
                    <strong>Entonces</strong> la info (credenciales, experiencia, rol) se presenta a familias/autoridades y se mantiene verificable.<br><br>
                    <strong>Escenario 2: Acceso a información directiva por autoridades</strong><br>
                    <strong>Dado que</strong> autoridades sanitarias requieren información,<br>
                    <strong>Cuando</strong> necesitan verificar credenciales y responsabilidades del personal clave,<br>
                    <strong>Entonces</strong> pueden acceder a la información completa y actualizada.
                </td>
            </tr>
            <tr>
                <td>US36</td>
                <td>Historia institucional</td>
                <td>Como administrador quiero gestionar la información histórica y reconocimientos de la casa de reposo para generar confianza y credibilidad.</td>
                <td>
                    <strong>Escenario 1: Presentación de historia y reconocimientos institucionales</strong><br>
                    <strong>Dado que</strong> un admin gestiona información histórica,<br>
                    <strong>Cuando</strong> actualiza historia, certificaciones y logros,<br>
                    <strong>Entonces</strong> la información se presenta de manera creíble, incluye certificaciones vigentes y genera confianza.<br><br>
                    <strong>Escenario 2: Verificación de certificaciones por autoridades</strong><br>
                    <strong>Dado que</strong> autoridades verifican certificaciones institucionales,<br>
                    <strong>Cuando</strong> requieren confirmar validez de licencias,<br>
                    <strong>Entonces</strong> pueden acceder a información verificable (N° de registro, fechas) y contactos de entidades.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP10</td>
                <td>Seguridad y privacidad</td>
                <td>Como administrador, quiero garantizar la seguridad y privacidad de los datos personales y médicos para proteger la información sensible de los residentes y familiares, cumpliendo con las normativas correspondientes.</td>
                <td></td>
            </tr>
            <tr>
                <td>US37</td>
                <td>Gestión de usuarios y permisos</td>
                <td>Como administrador quiero saber quién tiene acceso al sistema y qué información puede ver cada usuario para proteger la privacidad de los datos.</td>
                <td>
                    <strong>Escenario 1: Configuración exitosa de permisos de usuario</strong><br>
                    <strong>Dado que</strong> un admin de sistema gestiona accesos,<br>
                    <strong>Cuando</strong> asigna roles y permisos específicos a usuarios (familiares, personal, etc.),<br>
                    <strong>Entonces</strong> cada usuario accede únicamente a la información autorizada para su rol.<br><br>
                    <strong>Escenario 2: Intento de acceso no autorizado</strong><br>
                    <strong>Dado que</strong> un usuario intenta acceder a información,<br>
                    <strong>Cuando</strong> intenta ver datos que no le corresponden según su rol,<br>
                    <strong>Entonces</strong> el sistema bloquea el acceso, registra el intento y notifica al admin.
                </td>
            </tr>
            <tr>
                <td>US38</td>
                <td>Protección de datos mediante cifrado</td>
                <td>Como administrador quiero que toda la información sensible esté cifrada para proteger los datos personales y médicos de accesos no autorizados.</td>
                <td>
                    <strong>Escenario 1: Cifrado exitoso de datos sensibles</strong><br>
                    <strong>Dado que</strong> el sistema almacena información personal y médica,<br>
                    <strong>Cuando</strong> se guardan datos sensibles o se comunican (red),<br>
                    <strong>Entonces</strong> toda la información se cifra automáticamente antes del almacenamiento y durante la transmisión.<br><br>
                    <strong>Escenario 2: Intento de acceso a datos cifrados sin autorización</strong><br>
                    <strong>Dado que</strong> hay un intento de acceso directo a datos cifrados,<br>
                    <strong>Cuando</strong> alguien intenta acceder sin autorización apropiada,<br>
                    <strong>Entonces</strong> los datos permanecen inaccesibles y se activan alertas de seguridad.
                </td>
            </tr>
        </tbody>
                <tr>
                <td>EP11</td>
                <td>Diseño de interfaz</td>
                <td>Como usuario, quiero una interfaz bien diseñada para navegar y usar el sistema sin dificultades.</td>
                <td></td>
            </tr>
            <tr>
                <td>US40</td>
                <td>Menú de navegación consistente</td>
                <td>Como usuario quiero un menú de navegación claro y consistente en todas las páginas para encontrar fácilmente las funciones que necesito.</td>
                <td>
                    <strong>Escenario 1: Navegación consistente en toda la plataforma</strong><br>
                    <strong>Dado que</strong> un usuario se encuentra en cualquier página,<br>
                    <strong>Cuando</strong> utiliza el menú de navegación,<br>
                    <strong>Entonces</strong> encuentra las mismas opciones organizadas idénticamente, adaptadas a la pantalla e indicando la ubicación.<br><br>
                    <strong>Escenario 2: Menú adaptado a permisos de usuario</strong><br>
                    <strong>Dado que</strong> usuarios con diferentes roles acceden al sistema,<br>
                    <strong>Cuando</strong> navegan por la plataforma,<br>
                    <strong>Entonces</strong> ven solo las opciones de menú apropiadas para su rol (las opciones restringidas no aparecen).
                </td>
            </tr>
            <tr>
                <td>US41</td>
                <td>Paleta de colores y tipografía</td>
                <td>Como usuario quiero una interfaz con colores y tipografía consistentes para tener una experiencia visual agradable y fácil de leer.</td>
                <td>
                    <strong>Escenario 1: Aplicación consistente de diseño visual</strong><br>
                    <strong>Dado que</strong> se muestra cualquier página de la plataforma,<br>
                    <strong>Cuando</strong> un usuario navega por diferentes secciones,<br>
                    <strong>Entonces</strong> encuentra colores y tipografía consistentes, legibles y con contraste que cumple estándares de accesibilidad.<br><br>
                    <strong>Escenario 2: Adaptación para usuarios con necesidades especiales</strong><br>
                    <strong>Dado que</strong> usuarios con dificultades visuales acceden,<br>
                    <strong>Cuando</strong> acceden a la plataforma,<br>
                    <strong>Entonces</strong> pueden utilizar funciones de alto contraste o aumento de texto, manteniendo la legibilidad.
                </td>
            </tr>
            <tr>
                <td>US42</td>
                <td>Diseño de formularios usables</td>
                <td>Como usuario quiero formularios claros y fáciles de completar para ingresar información sin confusión ni errores.</td>
                <td>
                    <strong>Escenario 1: Completar formularios de manera eficiente</strong><br>
                    <strong>Dado que</strong> un usuario completa cualquier formulario,<br>
                    <strong>Cuando</strong> ingresa información requerida,<br>
                    <strong>Entonces</strong> los campos están etiquetados, organizados, recibe validación en tiempo real y confirmación al enviar.<br><br>
                    <strong>Escenario 2: Formulario con errores de validación</strong><br>
                    <strong>Dado que</strong> un usuario envía un formulario con información incorrecta,<br>
                    <strong>Cuando</strong> existen errores en los datos ingresados,<br>
                    <strong>Entonces</strong> recibe mensajes de error específicos y mantiene la información correcta ya ingresada.
                </td>
            </tr>
            <tr>
                <td>US43</td>
                <td>Patrones de diseño coherentes</td>
                <td>Como usuario quiero que todas las pantallas sigan patrones de diseño similares para predecir dónde encontrar funciones y cómo interactuar.</td>
                <td>
                    <strong>Escenario 1: Interacción predecible en toda la plataforma</strong><br>
                    <strong>Dado que</strong> un usuario está familiarizado con una sección,<br>
                    <strong>Cuando</strong> navega a nuevas secciones,<br>
                    <strong>Entonces</strong> encuentra patrones de interacción similares (botones, controles) y predecibles.<br><br>
                    <strong>Escenario 2: Nuevos usuarios aprendiendo la interfaz</strong><br>
                    <strong>Dado que</strong> un nuevo usuario accede por primera vez,<br>
                    <strong>Cuando</strong> explora diferentes funcionalidades,<br>
                    <strong>Entonces</strong> puede predecir cómo funcionarán nuevas secciones basándose en la consistencia de la interfaz.
                </td>
            </tr>
            <tr>
                <td>US44</td>
                <td>Manejo de errores comprensible</td>
                <td>Como usuario quiero que los errores se presenten de forma clara y con soluciones sugeridas para resolver problemas sin frustración.</td>
                <td>
                    <strong>Escenario 1: Error del sistema con guía de resolución</strong><br>
                    <strong>Dado que</strong> ocurre un error técnico (sistema o conectividad),<br>
                    <strong>Cuando</strong> el usuario lo experimenta,<br>
                    <strong>Entonces</strong> recibe un mensaje claro explicando qué ocurrió, pasos para resolverlo y contacto alternativo.<br><br>
                    <strong>Escenario 2: Error de usuario con orientación educativa</strong><br>
                    <strong>Dado que</strong> un usuario comete un error (acción incorrecta),<br>
                    <strong>Cuando</strong> realiza una acción no permitida,<br>
                    <strong>Entonces</strong> recibe una explicación clara del porqué y orientación sobre la forma correcta de proceder.
                </td>
            </tr>
            <tr>
                <td>TS01</td>
                <td>Eliminar medicamentos</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Delete para medicamentos para asegurar que el administrador de la casa de reposo pueda remover registros del inventario.</td>
                <td>
                    <strong>Escenario 1: Eliminación exitosa</strong><br>
                    <strong>Dado</strong> un admin autenticado con permisos y un {medicamentoId} existente<br>
                    <strong>Cuando</strong> envía DELETE /medicamentos/{medicamentoId}<br>
                    <strong>Entonces</strong> el servicio responde 204 No Content y el registro queda como eliminado.<br><br>
                    <strong>Escenario 2: Eliminación fallida por inexistencia o falta de permisos</strong><br>
                    <strong>Dado</strong> un usuario sin permisos o un {medicamentoId} inexistente<br>
                    <strong>Cuando</strong> intenta DELETE /medicamentos/{medicamentoId}<br>
                    <strong>Entonces</strong> responde 403 (permisos) o 404 Not Found (no existe) y registra en logs.
                </td>
            </tr>
            <tr>
                <td>TS02</td>
                <td>Agregar medicamentos</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Post medicamentos para permitir que el administrador de la casa de reposo pueda agregar más medicamentos.</td>
                <td>
                    <strong>Escenario 1: Creación exitosa</strong><br>
                    <strong>Dado</strong> un admin autenticado y datos válidos (nombre, lote, fechaVencimiento, cantidad)<br>
                    <strong>Cuando</strong> envía POST /medicamentos<br>
                    <strong>Entonces</strong> responde 201 Created y persiste en base de datos.<br><br>
                    <strong>Escenario 2: Error de validación o duplicado</strong><br>
                    <strong>Dado</strong> un registro con campos faltantes o que coincide con uno existente<br>
                    <strong>Cuando</strong> envía POST /medicamentos<br>
                    <strong>Entonces</strong> responde 400 (validación) o 409 (duplicado) con mensajes detallados.
                </td>
            </tr>
            <tr>
                <td>TS03</td>
                <td>Ver información detallada de los medicamentos</td>
                <td>Como desarrollador backend en NovaPeru Tech quiero crear una función para ver la información a través de una Api.</td>
                <td>
                    <strong>Escenario 1: Consulta exitosa</strong><br>
                    <strong>Dado</strong> un usuario autorizado y un {medicamentoId} válido<br>
                    <strong>Cuando</strong> solicita GET /medicamentos/{medicamentoId}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK con el JSON.<br><br>
                    <strong>Escenario 2: Recurso no encontrado o sin permisos</strong><br>
                    <strong>Dado</strong> un {medicamentoId} inexistente o un usuario sin autorización<br>
                    <strong>Cuando</strong> solicita GET /medicamentos/{medicamentoId}<br>
                    <strong>Entonces</strong> el servicio responde 404 Not Found (si no existe) o 403 (permisos).
                </td>
            </tr>
            <tr>
                <td>TS04</td>
                <td>Actualizar información de medicamentos</td>
                <td>Como desarrollador de backend en NovaPeru Tech quiero crear una función para actualizar la información para asegurar que el administrador de la casa de reposos pueda mantener actualizada la inforción de cada medicamento.</td>
                <td>
                    <strong>Escenario 1: Actualización exitosa con control de concurrencia</strong><br>
                    <strong>Dado</strong> un usuario autorizado, {medicamentoId} existente y datos válidos<br>
                    <strong>Cuando</strong> envía PUT/PATCH /medicamentos/{medicamentoId}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK y aplica los cambios.<br><br>
                    <strong>Escenario 2: Conflicto o validación fallida</strong><br>
                    <strong>Dado</strong> registro de datos inválido<br>
                    <strong>Cuando</strong> intenta PUT/PATCH /medicamentos/{medicamentoId}<br>
                    <strong>Entonces</strong> el servicio responde 400 Bad Request.
                </td>
            </tr>
            <tr>
                <td>TS05</td>
                <td>Agregar pacientes</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para permitir que el administrador registre nuevos residentes con validaciones obligatorias y que se genere un ID único por residente.</td>
                <td>
                    <strong>Escenario 1: Registro exitoso de residente</strong><br>
                    <strong>Dado</strong> un admin autenticado e ingresa datos válidos<br>
                    <strong>Cuando</strong> envía POST /residents<br>
                    <strong>Entonces</strong> responde 201 Created, retorna {residentId} y persiste en BBDD.<br><br>
                    <strong>Escenario 2: Duplicado o campos faltantes</strong><br>
                    <strong>Dado</strong> un DNI ya registrado o campos obligatorios faltantes<br>
                    <strong>Cuando</strong> envía POST /residents<br>
                    <strong>Entonces</strong> responde 400 (faltan datos) o 409 (duplicado) con detalles.
                </td>
            </tr>
            <tr>
                <td>TS06</td>
                <td>Ver información detallada de los pacientes</td>
                <td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que devuelva la información completa del residente para que el personal autorizado pueda consultar fácilmente el expediente.</td>
                <td>
                    <strong>Escenario 1: Consulta autorizada</strong><br>
                    <strong>Dado</strong> personal autorizado y {residentId} válido<br>
                    <strong>Cuando</strong> solicita GET /residents/{residentId}<br>
                    <strong>Entonces</strong> recibe 200 OK con datos (personales, contactos, resumen médico).<br><br>
                    <strong>Escenario 2: Sin permisos o recurso inexistente</strong><br>
                    <strong>Dado</strong> usuario sin permisos o {residentId} no existente<br>
                    <strong>Cuando</strong> solicita GET /residents/{residentId}<br>
                    <strong>Entonces</strong> responde 404 Not Found (no existe) o 403 (permisos).
                </td>
            </tr>
            <tr>
                <td>TS07</td>
                <td>Eliminar paciente</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE que realice una eliminación controlada del residente.</td>
                <td>
                    <strong>Escenario 1: Baja controlada exitosa</strong><br>
                    <strong>Dado</strong> un admin autenticado<br>
                    <strong>Cuando</strong> envía DELETE /residents/{residentId}<br>
                    <strong>Entonces</strong> el sistema marca el residente como 'inactive' y revoca accesos asociados.<br><br>
                    <strong>Escenario 2: Eliminación fallida</strong><br>
                    <strong>Dado</strong> un {residentId} con responsabilidades activas<br>
                    <strong>Cuando</strong> intenta DELETE /residents/{residentId}<br>
                    <strong>Entonces</strong> el servicio responde 409 Conflict con la lista de acciones requeridas.
                </td>
            </tr>
            <tr>
                <td>TS08</td>
                <td>Actualizar información de los pacientes</td>
                <td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar campos del perfil del residente para que las modificaciones queden registradas y sean reversibles si es necesario.</td>
                <td>
                    <strong>Escenario 1: Actualización válida y registrada</strong><br>
                    <strong>Dado</strong> un admin autorizado y datos permitidos<br>
                    <strong>Cuando</strong> envía PATCH /residents/{residentId}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK, aplica cambios y guarda auditoría.<br><br>
                    <strong>Escenario 2: Intento de modificar campos restringidos o datos inválidos</strong><br>
                    <strong>Dado</strong> un registro con campos de solo lectura o formato inválido<br>
                    <strong>Cuando</strong> envía PATCH /residents/{residentId}<br>
                    <strong>Entonces</strong> el servicio responde 400 Bad Request.
                </td>
            </tr>
            <tr>
                <td>TS09</td>
                <td>Agregar información detallada de la casa de reposo</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que un administrador pueda registrar información institucional.</td>
                <td>
                    <strong>Escenario 1: Creación de información institucional exitosa</strong><br>
                    <strong>Dado</strong> un admin autenticado y registro de datos válido<br>
                    <strong>Cuando</strong> envía POST /institution-info<br>
                    <strong>Entonces</strong> el servicio responde 201 Created y los datos quedan disponibles.<br><br>
                    <strong>Escenario 2: Error por falta de permisos o validación</strong><br>
                    <strong>Dado</strong> un usuario no admin o datos obligatorios faltantes<br>
                    <strong>Cuando</strong> envía POST /institution-info<br>
                    <strong>Entonces</strong> responde 403 (permisos) o 400 (validación).
                </td>
            </tr>
            <tr>
                <td>TS10</td>
                <td>Actualizar información de la casa de reposo</td>
                <td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PUT para mantener actualizados los datos institucionales.</td>
                <td>
                    <strong>Escenario 1: Actualización exitosa y auditada</strong><br>
                    <strong>Dado</strong> un admin autenticado y payload válido<br>
                    <strong>Cuando</strong> envía PUT/PATCH /institution-info/{id}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK, actualiza datos y registra auditoría (quién, cuándo).<br><br>
                    <strong>Escenario 2: Conflicto de versión o datos inválidos</strong><br>
                    <strong>Dado</strong> datos inválidos (ej. formato)<br>
                    <strong>Cuando</strong> intenta PUT/PATCH /institution-info/{id}<br>
                    <strong>Entonces</strong> el servicio responde 400 Bad Request.
                </td>
            </tr>
            <tr>
                <td>TS11</td>
                <td>Agregar empleado</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que registre nuevos empleados.</td>
                <td>
                    <strong>Escenario 1: Registro de empleado exitoso</strong><br>
                    <strong>Dado</strong> un admin autenticado y datos válidos<br>
                    <strong>Cuando</strong> envía POST /employees<br>
                    <strong>Entonces</strong> responde 201 Created, retorna {employeeId}, asigna permisos y crea credenciales.<br><br>
                    <strong>Escenario 2: Error por email/ID duplicado o validación</strong><br>
                    <strong>Dado</strong> un email o DNI ya registrado, o campos inválidos<br>
                    <strong>Cuando</strong> envía POST /employees<br>
                    <strong>Entonces</strong> responde 409 (duplicado) o 400 (validación).
                </td>
            </tr>
            <tr>
                <td>TS12</td>
                <td>Eliminar empleado</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE para que el administrador de la casa de reposo revoque persmisos.</td>
                <td>
                    <strong>Escenario 1: Baja controlada exitosa</strong><br>
                    <strong>Dado</strong> un admin autenticado y empleado sin tareas críticas pendientes<br>
                    <strong>Cuando</strong> envía DELETE /employees/{employeeId}<br>
                    <strong>Entonces</strong> el servicio elimina al empleado y registra la acción.<br><br>
                    <strong>Escenario 2: Baja bloqueada por responsabilidades activas o sin permisos</strong><br>
                    <strong>Dado</strong> un empleado con tareas asignadas o un usuario sin permisos<br>
                    <strong>Cuando</strong> intenta DELETE /employees/{employeeId}<br>
                    <strong>Entonces</strong> responde 409 (requiere reasignación) o 403 (permisos).
                </td>
            </tr>
            <tr>
                <td>TS13</td>
                <td>Actualizar información del empleado</td>
                <td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar datos de empleado.</td>
                <td>
                    <strong>Escenario 1: Actualización válida con auditoría</strong><br>
                    <strong>Dado</strong> un admin autenticado y datos válidos<br>
                    <strong>Cuando</strong> envía PATCH /employees/{employeeId}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK y registra el cambio.<br><br>
                    <strong>Escenario 2: Intento de actualizar datos inválidos</strong><br>
                    <strong>Dado</strong> un intento de registrar datos inválidos<br>
                    <strong>Cuando</strong> envía PATCH /employees/{employeeId}<br>
                    <strong>Entonces</strong> el servicio responde 400 Bad Request.
                </td>
            </tr>
            <tr>
                <td>TS14</td>
                <td>Ver información del empleado</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET que muestre el perfil del empleado para que el administrador pueda observar cuantos empleados tiene.</td>
                <td>
                    <strong>Escenario 1: Consulta autorizada del perfil</strong><br>
                    <strong>Dado</strong> un usuario autorizado y un {employeeId} válido<br>
                    <strong>Cuando</strong> solicita GET /employees/{employeeId}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK (datos filtrados según permisos).<br><br>
                    <strong>Escenario 2: empleado no existe</strong><br>
                    <strong>Dado</strong> un {employeeId} inexistente<br>
                    <strong>Cuando</strong> solicita GET /employees/{employeeId}<br>
                    <strong>Entonces</strong> el servicio responde 404 Not Found.
                </td>
            </tr>
            <tr>
                <td>TS15</td>
                <td>Consumir Api de Medicamentos</td>
                <td>Como desarrollador backend en NovaPeru tech quiero consumir la API externa de medicamentos mediante un servicio de integración , para disponer de información confiable y actualizada de medicamentos en el sistema.</td>
                <td>
                    <strong>Escenario 1: Sincronización exitosa y segura</strong><br>
                    <strong>Dado</strong> credenciales válidas y conectividad estable<br>
                    <strong>Cuando</strong> se ejecuta la sincronización (programada o manual)<br>
                    <strong>Entonces</strong> los datos externos se mapean, normalizan y guardan en la BBDD interna.<br><br>
                    <strong>Escenario 2: Fallo externo</strong><br>
                    <strong>Dado</strong> un timeout o respuesta inválida de la API externa<br>
                    <strong>Cuando</strong> intenta sincronizar<br>
                    <strong>Entonces</strong> el servicio registra la incidencia y no sobrescribe los datos locales.
                </td>
            </tr>
            <tr>
                <td>TS16</td>
                <td>Consumir Api de google maps</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de integración con Google Maps que proporcione verificación de direcciones y datos de localización para manejar errores.</td>
                <td>
                    <strong>Escenario 1: Geocoding verificado vía proxy</strong><br>
                    <strong>Dado</strong> una API key protegida en backend y una dirección válida<br>
                    <strong>Cuando</strong> solicita geocoding vía GET /maps/proxy?address=...<br>
                    <strong>Entonces</strong> el proxy devuelve datos normalizados (lat/lng) y la API key no se expone.<br><br>
                    <strong>Escenario 2: Rate limit o error del proveedor</strong><br>
                    <strong>Dado</strong> que Google Maps devuelve 429 (rate limit) o falla<br>
                    <strong>Cuando</strong> realiza la petición al proxy<br>
                    <strong>Entonces</strong> el proxy responde 429/503 (controlado), aplica política de backoff y usa caché.
                </td>
            </tr>
            <tr>
                <td>TS17</td>
                <td>Notificación de visitas</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de notificaciones para enviar recordatorios y alertas de visitas vía email/SMS.</td>
                <td>
                    <strong>Escenario 1: Envío de recordatorio exitoso</strong><br>
                    <strong>Dado</strong> una visita programada y contactos válidos<br>
                    <strong>Cuando</strong> falta el tiempo configurado (ej. 2h) y la cola procesa el job<br>
                    <strong>Entonces</strong> se envía la notificación (email/SMS/push) y el sistema registra el estado 'delivered'.<br><br>
                    <strong>Escenario 2: Fallo en entrega y reintentos</strong><br>
                    <strong>Dado</strong> un fallo de entrega<br>
                    <strong>Cuando</strong> el worker intenta enviar la notificación<br>
                    <strong>Entonces</strong> el sistema aplica los reintentos configurados (y registra 'failed' si se agotan).
                </td>
            </tr>
            <tr>
                <td>TS18</td>
                <td>Buscar y filtrar medicamentos</td>
                <td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET con parámetros de búsqueda facilitar consultas rápidas y generación de reportes.</td>
                <td>
                    <strong>Escenario 1: Búsqueda paginada exitosa</strong><br>
                    <strong>Dado</strong> parámetros de búsqueda válidos (paginación, filtros)<br>
                    <strong>Cuando</strong> solicita GET /medicamentos?{params}<br>
                    <strong>Entonces</strong> el servicio responde 200 OK con la lista paginada.<br><br>
                    <strong>Escenario 2: Parámetros inválidos o sin resultados</strong><br>
                    <strong>Dado</strong> parámetros inválidos o un criterio que no retorna coincidencias<br>
                    <strong>Cuando</strong> solicita GET /medicamentos?{params}<br>
                    <strong>Entonces</strong> responde 400 (inválido) o 200 OK con items: [] (sin resultados).
                </td>
            </tr>
            <tr>
                <td>TS19</td>
                <td>Buscar y filtrar residentes</td>
                <td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET con filtros para que administradores y personal autorizado encuentren residentes fácilmente.</td>
                <td>
                    <strong>Escenario 1: Consulta filtrada y autorizada</strong><br>
                    <strong>Dado</strong> filtros válidos y un usuario autorizado<br>
                    <strong>Cuando</strong> solicita GET /residents?nombre=X&habitacion=Y<br>
                    <strong>Entonces</strong> responde 200 OK con resultados paginados (campos conforme a permisos).<br><br>
                    <strong>Escenario 2: Intento sin permisos o parámetros inválidos</strong><br>
                    <strong>Dado</strong> un usuario sin permiso o parámetros mal formados<br>
                    <strong>Cuando</strong> solicita GET /residents?{params}<br>
                    <strong>Entonces</strong> responde 403 (permisos) o 400 (inválido).
                </td>
            </tr>
            <tr>
                <td>TS20</td>
                <td>Buscar y filtrar empleados</td>
                <td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que permita buscar y filtrar por nombre, rol, turno que se pueda exportar para que vea el reporte de empleados el admnistrador o RRHH.</td>
                <td>
                    <strong>Escenario 1: Búsqueda y exportación permitida</strong><br>
                    <strong>Dado</strong> parámetros válidos y un usuario con permiso de exportación<br>
                    <strong>Cuando</strong> solicita GET /employees?rol=cuidador&export=true<br>
                    <strong>Entonces</strong> responde 200 OK, inicia la exportación (CSV) y devuelve enlace de descarga.<br><br>
                    <strong>Escenario 2: Exportación denegada o sin resultados</strong><br>
                    <strong>Dado</strong> filtros que no arrojan resultados o parámetros inválidos<br>
                    <strong>Cuando</strong> solicita GET /employees?{params}<br>
                    <strong>Entonces</strong> responde 400 (inválido) o 200 OK con lista vacía (sin resultados).
                </td>
            </tr>
        </tbody>
    </table>


## 3.2. Impact Mapping

<img src="../images/Impact map 1.png" alt="Impact map 1" width="auto" height="auto"/>

## 3.3. Product Backlog

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr>
    <td><strong>Orden</strong></td><td><strong>User Story Id</strong></td><td><strong>Título</strong></td><td><strong>Descripción</strong></td><td><strong>Story Points (1/2/3)</strong></td>
  </tr>
  <tr><td>1</td><td>US01</td><td>Menú de navegación</td><td>Como visitante de la landing page, quiero acceder a un menú superior con enlaces a “Log in”, “Sign up”, “Planes” y “Contacto”, para navegar rápidamente a secciones clave.</td><td>1</td></tr>
  <tr><td>2</td><td>US02</td><td>Visualización de Planes</td><td>Como visitante, quiero ver planes con precio, características y duración, para comparar y elegir el que mejor se adapte a mis necesidades.</td><td>2</td></tr>
  <tr><td>3</td><td>US03</td><td>Selección de Plan en Landing Page</td><td>Como visitante, quiero seleccionar un plan y confirmarlo en la misma pantalla, para agilizar y simplificar mi registro.</td><td>3</td></tr>
  <tr><td>4</td><td>US04</td><td>Visualización de creadores</td><td>Como visitante, quiero ver al equipo creador (nombre, foto, rol y descripción), para generar confianza en el servicio.</td><td>2</td></tr>
  <tr><td>5</td><td>US05</td><td>Redes sociales</td><td>Como visitante, quiero acceder a las redes sociales desde el header o footer, para conocer más de la empresa y tener canales adicionales de contacto.</td><td>1</td></tr>
  <tr><td>6</td><td>US06</td><td>Formulario de contacto</td><td>Como visitante, quiero enviar consultas mediante un formulario con validación, para recibir una respuesta personalizada.</td><td>3</td></tr>
  <tr><td>7</td><td>US07</td><td>Cambio de idioma</td><td>Como visitante, quiero cambiar entre español e inglés desde el menú, para entender mejor el contenido.</td><td>3</td></tr>
  <tr><td>8</td><td>US39</td><td>Términos y condiciones</td><td>Como visitante, quiero acceder a los términos y condiciones, para conocer las políticas legales antes de contratar.</td><td>2</td></tr>
  <tr><td>9</td><td>US08</td><td>Historial médico</td><td>Como familiar de un adulto mayor, quiero acceder al historial médico completo, para conocer su evolución y diagnósticos actuales.</td><td>3</td></tr>
  <tr><td>10</td><td>US09</td><td>Agenda de citas médicas</td><td>Como familiar, quiero consultar la agenda de citas médicas, para estar informada y planificar con anticipación.</td><td>3</td></tr>
  <tr><td>11</td><td>US10</td><td>Consulta de información personal</td><td>Como familiar, quiero ver la información personal del residente, para verificar que esté correcta o solicitar cambios.</td><td>3</td></tr>
  <tr><td>12</td><td>US11</td><td>Galería de fotos y actividades</td><td>Como familiar, quiero ver fotos de actividades organizadas por fecha y tipo, para sentirme conectada y verificar su participación social.</td><td>3</td></tr>
  <tr><td>13</td><td>US12</td><td>Registro de residentes</td><td>Como administradora de la casa de reposo, quiero crear perfiles completos de los residentes, para centralizar su información personal y médica.</td><td>3</td></tr>
  <tr><td>14</td><td>US13</td><td>Historial médico institucional</td><td>Como administradora con permisos médicos, quiero gestionar el historial médico de cada residente, para asegurar continuidad de cuidado y cumplir regulaciones.</td><td>3</td></tr>
  <tr><td>15</td><td>US14</td><td>Administración de medicamentos</td><td>Como administradora, quiero controlar la administración de medicamentos, para garantizar cumplimiento de tratamientos y evitar errores.</td><td>3</td></tr>
  <tr><td>16</td><td>US15</td><td>Gestión de visitas familiares</td><td>Como administradora, quiero programar y controlar visitas familiares, para mantener seguridad, orden y horarios establecidos.</td><td>3</td></tr>
  <tr><td>17</td><td>US16</td><td>Recordatorios de citas y consultas</td><td>Como familiar, quiero recibir recordatorios automáticos de citas médicas, para estar preparada y decidir si acompañaré.</td><td>3</td></tr>
  <tr><td>18</td><td>US17</td><td>Notificaciones de cambios en medicación</td><td>Como familiar, quiero ser notificada ante cambios en la medicación, para estar informada del tratamiento.</td><td>3</td></tr>
  <tr><td>19</td><td>US18</td><td>Recordatorios de visitas familiares</td><td>Como familiar, quiero recibir recordatorios de mis visitas programadas, para no olvidar y mantener regularidad en el contacto.</td><td>3</td></tr>
  <tr><td>20</td><td>US19</td><td>Alertas de actualización de datos personales</td><td>Como familiar, quiero recibir notificaciones cuando se actualicen datos personales del residente, para mantenerme informada de cualquier cambio.</td><td>3</td></tr>
  <tr><td>21</td><td>US20</td><td>Preguntas sobre rutina de cuidados</td><td>Como familiar, quiero enviar preguntas a cuidadores sobre la rutina diaria, para resolver dudas puntuales.</td><td>3</td></tr>
  <tr><td>22</td><td>US21</td><td>Peticiones de modificación de cuidados</td><td>Como familiar, quiero solicitar ajustes específicos en el cuidado, para adecuarlo a preferencias o necesidades particulares.</td><td>3</td></tr>
  <tr><td>23</td><td>US22</td><td>Seguimiento del bienestar emocional</td><td>Como familiar, quiero comunicarme sobre el estado emocional y psicológico del residente, para asegurar su bienestar integral.</td><td>3</td></tr>
  <tr><td>24</td><td>US23</td><td>Planificación de eventos familiares</td><td>Como familiar, quiero coordinar eventos o celebraciones dentro de la institución, para organizar ocasiones especiales del residente.</td><td>3</td></tr>
  <tr><td>25</td><td>US24</td><td>Registro de medicamentos en inventario</td><td>Como administradora, quiero registrar medicamentos con datos completos, para mantener un inventario actualizado.</td><td>3</td></tr>
  <tr><td>26</td><td>US25</td><td>Alertas de vencimiento</td><td>Como administradora, quiero recibir alertas sobre medicamentos próximos a vencer, para evitar pérdidas y riesgos de seguridad.</td><td>3</td></tr>
  <tr><td>27</td><td>US26</td><td>Eliminación de medicamentos</td><td>Como administradora, quiero eliminar medicamentos del inventario de forma controlada, para mantener la precisión del stock y cumplir protocolos.</td><td>3</td></tr>
  <tr><td>28</td><td>US27</td><td>Búsqueda y filtrado de inventario</td><td>Como administradora, quiero filtrar y buscar medicamentos por criterios, para encontrar información específica y generar reportes.</td><td>3</td></tr>
  <tr><td>29</td><td>US28</td><td>Información de medicamentos para personal</td><td>Como administradora, quiero brindar información detallada de medicamentos al personal, para asegurar una administración segura y correcta.</td><td>3</td></tr>
  <tr><td>30</td><td>US29</td><td>Gestión de perfiles de empleados</td><td>Como administradora, quiero registrar y mantener perfiles completos del personal, para tener información actualizada y asignar roles.</td><td>3</td></tr>
  <tr><td>31</td><td>US30</td><td>Baja de personal</td><td>Como administradora, quiero dar de baja empleados y revocar accesos, para mantener registros al día y cerrar contratos.</td><td>3</td></tr>
  <tr><td>32</td><td>US31</td><td>Búsqueda y filtrado de empleados</td><td>Como administradora, quiero filtrar y buscar empleados por criterios, para encontrar rápidamente personal específico.</td><td>3</td></tr>
  <tr><td>33</td><td>US32</td><td>Gestión de horas extra</td><td>Como administradora, quiero controlar horas extra trabajadas, para gestionar costos laborales y cumplir regulaciones.</td><td>3</td></tr>
  <tr><td>34</td><td>US33</td><td>Gestión de horarios de atención</td><td>Como administradora, quiero configurar horarios de atención y servicios, para informar disponibilidad y sincronizar citas.</td><td>3</td></tr>
  <tr><td>35</td><td>US34</td><td>Datos de contacto institucional</td><td>Como administradora, quiero actualizar los datos de contacto institucional, para que familias y autoridades accedan a información vigente.</td><td>2</td></tr>
  <tr><td>36</td><td>US35</td><td>Información del personal directivo</td><td>Como administradora, quiero gestionar la información del personal directivo, para dar transparencia a familias y autoridades.</td><td>2</td></tr>
  <tr><td>37</td><td>US36</td><td>Historia institucional</td><td>Como administradora, quiero gestionar historia y reconocimientos de la institución, para generar confianza y credibilidad.</td><td>2</td></tr>
  <tr><td>38</td><td>US37</td><td>Gestión de usuarios y permisos</td><td>Como administradora, quiero configurar roles y permisos de acceso, para proteger la privacidad de los datos.</td><td>3</td></tr>
  <tr><td>39</td><td>US38</td><td>Protección de datos mediante cifrado</td><td>Como administradora, quiero que los datos sensibles estén cifrados en almacenamiento y tránsito, para evitar accesos no autorizados.</td><td>3</td></tr>
  <tr><td>40</td><td>US40</td><td>Menú de navegación consistente</td><td>Como usuaria, quiero un menú claro y consistente en todas las páginas, para encontrar fácilmente las funciones que necesito.</td><td>2</td></tr>
  <tr><td>41</td><td>US41</td><td>Paleta de colores y tipografía</td><td>Como usuaria, quiero colores y tipografía consistentes y accesibles, para una experiencia visual agradable y legible.</td><td>2</td></tr>
  <tr><td>42</td><td>US42</td><td>Diseño de formularios usables</td><td>Como usuaria, quiero formularios claros con validación, para completar información sin confusión ni errores.</td><td>3</td></tr>
  <tr><td>43</td><td>US43</td><td>Patrones de diseño coherentes</td><td>Como usuaria, quiero patrones de diseño similares en todas las pantallas, para predecir dónde encontrar funciones y cómo interactuar.</td><td>2</td></tr>
  <tr><td>44</td><td>US44</td><td>Manejo de errores comprensible</td><td>Como usuaria, quiero mensajes de error claros con pasos de solución, para resolver problemas sin frustración.</td><td>3</td></tr>
  <tr><td>45</td><td>TS01</td><td>Eliminar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Delete para medicamentos para asegurar que el administrador de la casa de reposo pueda remover registros del inventario.</td><td>3</td></tr>
  <tr><td>46</td><td>TS02</td><td>Agregar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Post medicamentos para permitir que el administrador de la casa de reposo pueda agregar más medicamentos.</td><td>3</td></tr>
  <tr><td>47</td><td>TS03</td><td>Ver información detallada de los medicamentos</td><td>Como desarrollador backend en NovaPeru Tech quiero crear una función para ver la información a través de una Api.</td><td>3</td></tr>
  <tr><td>48</td><td>TS04</td><td>Actualizar información de medicamentos</td><td>Como desarrollador de backend en NovaPeru Tech quiero crear una función para actualizar la información para asegurar que el administrador de la casa de reposos pueda mantener actualizada la información de cada medicamento.</td><td>3</td></tr>
  <tr><td>49</td><td>TS05</td><td>Agregar pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para permitir que el administrador registre nuevos residentes con validaciones obligatorias y que se genere un ID único por residente.</td><td>3</td></tr>
  <tr><td>50</td><td>TS06</td><td>Ver información detallada de los pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que devuelva la información completa del residente para que el personal autorizado pueda consultar fácilmente el expediente.</td><td>3</td></tr>
  <tr><td>51</td><td>TS07</td><td>Eliminar paciente</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE que realice una eliminación controlada del residente.</td><td>3</td></tr>
<tr><td>52</td><td>TS08</td><td>Actualizar información de los pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar campos del perfil del residente para que las modificaciones queden registradas y sean reversibles si es necesario.</td><td>3</td></tr>
<tr><td>53</td><td>TS09</td><td>Agregar información detallada de la casa de reposo</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que un administrador pueda registrar información institucional.</td><td>3</td></tr>
<tr><td>54</td><td>TS10</td><td>Actualizar información de la casa de reposo</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PUT para mantener actualizados los datos institucionales.</td><td>3</td></tr>
<tr><td>55</td><td>TS11</td><td>Agregar empleado</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que registre nuevos empleados.</td><td>3</td></tr>
<tr><td>56</td><td>TS12</td><td>Eliminar empleado</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE para que el administrador de la casa de reposo revoque persmisos.</td><td>3</td></tr>
<tr><td>57</td><td>TS13</td><td>Actualizar información del empleado</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar datos de empleado.</td><td>3</td></tr>
<tr><td>58</td><td>TS14</td><td>Ver información del empleado</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET que muestre el perfil del empleado para que el administrador pueda observar cuantos empleados tiene.</td><td>3</td></tr>
<tr><td>59</td><td>TS15</td><td>Consumir Api de Medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero consumir la API externa de medicamentos mediante un servicio de integración , para disponer de información confiable y actualizada de medicamentos en el sistema.</td><td>3</td></tr>
<tr><td>60</td><td>TS16</td><td>Consumir Api de google maps</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de integración con Google Maps que proporcione verificación de direcciones y datos de localización para manejar errores.</td><td>3</td></tr>
<tr><td>61</td><td>TS17</td><td>Notificación de visitas</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de notificaciones para enviar recordatorios y alertas de visitas vía email/SMS.</td><td>3</td></tr>
<tr><td>62</td><td>TS18</td><td>Buscar y filtrar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET con parámetros de búsqueda facilitar consultas rápidas y generación de reportes.</td><td>3</td></tr>
<tr><td>63</td><td>TS19</td><td>Buscar y filtrar residentes</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET con filtros para que administradores y personal autorizado encuentren residentes fácilmente.</td><td>3</td></tr>
<tr><td>64</td><td>TS20</td><td>Buscar y filtrar empleados</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que permita buscar y filtrar por nombre, rol, turno que se pueda exportar para que vea el reporte de empleados el admnistrador o RRHH.</td><td>3</td></tr>
</table>
