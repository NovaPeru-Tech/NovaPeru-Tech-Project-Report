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
                    <strong>Escenario 1: Navegación exitosa a través del menú</strong><br>
                    <strong>Dado que</strong> el visitante está en la landing page<br>
                    <strong>Cuando</strong> el menú de navegación está disponible<br>
                    <strong>Entonces</strong> el usuario puede ver los enlaces principales y navegar a las secciones correspondientes.<br><br>
                    <strong>Escenario 2: Menú no disponible</strong><br>
                    <strong>Dado que</strong> el visitante está en la landing page<br>
                    <strong>Cuando</strong> el menú de navegación no se carga correctamente<br>
                    <strong>Entonces</strong> el usuario recibe un mensaje de error y tiene opciones alternativas de navegación.
                </td>
            </tr>
            <tr>
                <td>US02</td>
                <td>Visualización de Planes</td>
                <td>Como visitante de la Landing Page, quiero ver los planes de suscripción junto a su precio y características, para poder elegir el que mejor se adapte a mis necesidades.</td>
                <td>
                    <strong>Escenario 1: Visualización de planes disponibles</strong><br>
                    <strong>Dado que</strong> el visitante navega a la sección de planes<br>
                    <strong>Cuando</strong> los planes están disponibles en el sistema<br>
                    <strong>Entonces</strong> el usuario puede ver la lista de planes con sus precios y características para compararlos.<br><br>
                    <strong>Escenario 2: Planes no disponibles</strong><br>
                    <strong>Dado que</strong> el visitante navega a la sección de planes<br>
                    <strong>Cuando</strong> no hay planes disponibles o ocurre un error de carga<br>
                    <strong>Entonces</strong> el usuario recibe un mensaje informativo sobre la indisponibilidad.
                </td>
            </tr>
            <tr>
                <td>US03</td>
                <td>Selección de Plan en Landing Page</td>
                <td>Como visitante de la landing Page, quiero seleccionar un plan y finalizar la confirmación en la misma pantalla, para agilizar y simplificar el registro.</td>
                <td>
                    <strong>Escenario 1: Selección exitosa de plan</strong><br>
                    <strong>Dado que</strong> el visitante ha seleccionado un plan disponible<br>
                    <strong>Cuando</strong> confirma la selección<br>
                    <strong>Entonces</strong> el sistema muestra el formulario de registro con el plan pre-seleccionado.<br><br>
                    <strong>Escenario 2: Datos de registro incompletos</strong><br>
                    <strong>Dado que</strong> el visitante está completando el formulario de registro<br>
                    <strong>Cuando</strong> faltan datos obligatorios<br>
                    <strong>Entonces</strong> el sistema muestra mensajes de validación específicos para los campos requeridos.
                </td>
            </tr>
            <tr>
                <td>US04</td>
                <td>Visualización de creadores</td>
                <td>Como visitante de la Landing Page, quiero ver a los creadores de la aplicación, para conocer al equipo detrás del producto y generar confianza en el servicio.</td>
                <td>
                    <strong>Escenario 1: Acceso a información del equipo</strong><br>
                    <strong>Dado que</strong> el visitante navega a la sección "Equipo"<br>
                    <strong>Cuando</strong> la información del equipo está disponible<br>
                    <strong>Entonces</strong> el usuario puede ver los detalles de los creadores incluyendo nombres, roles e información de contacto.<br><br>
                    <strong>Escenario 2: Información del equipo no disponible</strong><br>
                    <strong>Dado que</strong> el visitante navega a la sección "Equipo"<br>
                    <strong>Cuando</strong> la información no está disponible<br>
                    <strong>Entonces</strong> el usuario recibe un mensaje informativo sobre la indisponibilidad temporal.
                </td>
            </tr>
            <tr>
                <td>US07</td>
                <td>Cambio de idioma</td>
                <td>Como visitante del Landing Page quiero en el menú un botón para cambiar de idioma entre español e inglés para entender mejor de que trata Veyra.</td>
                <td>
                    <strong>Escenario 1: Cambio exitoso de idioma</strong><br>
                    <strong>Dado que</strong> el visitante selecciona un idioma disponible<br>
                    <strong>Cuando</strong> confirma el cambio de idioma<br>
                    <strong>Entonces</strong> la interfaz se actualiza al idioma seleccionado y mantiene la preferencia.<br><br>
                    <strong>Escenario 2: Idioma no disponible</strong><br>
                    <strong>Dado que</strong> el visitante intenta cambiar a un idioma<br>
                    <strong>Cuando</strong> el idioma seleccionado no está disponible<br>
                    <strong>Entonces</strong> el sistema mantiene el idioma actual y muestra un mensaje informativo.
                </td>
            </tr>
            <tr>
                <td>US39</td>
                <td>Términos y condiciones</td>
                <td>Como visitante de la landing page quiero poder acceder a los términos y condiciones de uso para conocer las políticas legales antes de contratar los servicios.</td>
                <td>
                    <strong>Escenario 1: Acceso a términos y condiciones</strong><br>
                    <strong>Dado que</strong> el visitante solicita ver los términos y condiciones<br>
                    <strong>Cuando</strong> el documento está disponible<br>
                    <strong>Entonces</strong> el usuario puede acceder al documento completo y actualizado.<br><br>
                    <strong>Escenario 2: Términos actualizados requieren aceptación</strong><br>
                    <strong>Dado que</strong> existen términos y condiciones actualizados<br>
                    <strong>Cuando</strong> un usuario existente accede al sistema<br>
                    <strong>Entonces</strong> el sistema requiere la revisión y aceptación de los nuevos términos antes de continuar.
                </td>
            </tr>
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
                    <strong>Escenario 1: Acceso a redes sociales</strong><br>
                    <strong>Dado que</strong> el visitante busca los enlaces de redes sociales<br>
                    <strong>Cuando</strong> los enlaces están disponibles<br>
                    <strong>Entonces</strong> el usuario puede acceder a las páginas oficiales de las redes sociales.<br><br>
                    <strong>Escenario 2: Enlaces no funcionales</strong><br>
                    <strong>Dado que</strong> el visitante intenta acceder a una red social<br>
                    <strong>Cuando</strong> el enlace no está funcionando<br>
                    <strong>Entonces</strong> el usuario recibe un mensaje informativo sobre el problema.
                </td>
            </tr>
            <tr>
                <td>US06</td>
                <td>Formulario de contacto</td>
                <td>Como visitante del landing page quiero completar un formulario de contacto para enviar consultas específicas y recibir una respuesta personalizada de Veyra.</td>
                <td>
                    <strong>Escenario 1: Envío exitoso de consulta</strong><br>
                    <strong>Dado que</strong> el visitante completa el formulario de contacto<br>
                    <strong>Cuando</strong> todos los campos requeridos están completos y válidos<br>
                    <strong>Entonces</strong> la consulta se envía exitosamente y el usuario recibe confirmación.<br><br>
                    <strong>Escenario 2: Datos de contacto inválidos</strong><br>
                    <strong>Dado que</strong> el visitante completa el formulario de contacto<br>
                    <strong>Cuando</strong> existen campos inválidos o incompletos<br>
                    <strong>Entonces</strong> el sistema muestra mensajes de validación específicos para los campos problemáticos.
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
                    <strong>Escenario 1: Acceso al historial médico</strong><br>
                    <strong>Dado que</strong> el familiar está autenticado y tiene permisos<br>
                    <strong>Cuando</strong> solicita ver el historial médico<br>
                    <strong>Entonces</strong> el sistema muestra el historial médico completo organizado cronológicamente.<br><br>
                    <strong>Escenario 2: Sin permisos para acceder al historial</strong><br>
                    <strong>Dado que</strong> el usuario intenta acceder al historial médico<br>
                    <strong>Cuando</strong> no tiene los permisos necesarios<br>
                    <strong>Entonces</strong> el sistema muestra un mensaje de restricción de acceso.
                </td>
            </tr>
            <tr>
                <td>US09</td>
                <td>Agenda de citas Medicas</td>
                <td>Como familiar de un adulto mayor quiero consultar la agenda de citas médicas de mi familiar para estar informado sobre sus próximos tratamientos.</td>
                <td>
                    <strong>Escenario 1: Visualización de citas programadas</strong><br>
                    <strong>Dado que</strong> el familiar está autenticado<br>
                    <strong>Cuando</strong> accede a la agenda de citas<br>
                    <strong>Entonces</strong> el sistema muestra la lista de citas médicas programadas con sus detalles.<br><br>
                    <strong>Escenario 2: No hay citas programadas</strong><br>
                    <strong>Dado que</strong> el familiar consulta la agenda de citas<br>
                    <strong>Cuando</strong> no existen citas programadas<br>
                    <strong>Entonces</strong> el sistema muestra un mensaje informativo sobre la ausencia de citas.
                </td>
            </tr>
            <tr>
                <td>US10</td>
                <td>Consulta de información personal</td>
                <td>Como familiar de un adulto mayor quiero ver la información de mi familiar para estar seguro de que esté correcto o actualizado.</td>
                <td>
                    <strong>Escenario 1: Visualización de información personal</strong><br>
                    <strong>Dado que</strong> el familiar está autenticado<br>
                    <strong>Cuando</strong> accede al perfil de información personal<br>
                    <strong>Entonces</strong> el sistema muestra la información personal actualizada del adulto mayor.<br><br>
                    <strong>Escenario 2: Solicitud de actualización de información</strong><br>
                    <strong>Dado que</strong> el familiar identifica información desactualizada<br>
                    <strong>Cuando</strong> solicita una actualización<br>
                    <strong>Entonces</strong> el sistema registra la solicitud de cambio con la justificación proporcionada.
                </td>
            </tr>
            <tr>
                <td>US11</td>
                <td>Galería de fotos y actividades</td>
                <td>Como familiar de un adulto mayor quiero ver fotos de las actividades diarias de mi familiar para sentirme conectado con su día a día y verificar su participación social.</td>
                <td>
                    <strong>Escenario 1: Acceso a galería de actividades</strong><br>
                    <strong>Dado que</strong> el familiar está autenticado<br>
                    <strong>Cuando</strong> accede a la galería de fotos<br>
                    <strong>Entonces</strong> el sistema muestra las fotos organizadas por fecha y actividad.<br><br>
                    <strong>Escenario 2: Sin actividades recientes</strong><br>
                    <strong>Dado que</strong> el familiar consulta la galería<br>
                    <strong>Cuando</strong> no hay fotos recientes disponibles<br>
                    <strong>Entonces</strong> el sistema muestra un mensaje informativo sobre la frecuencia de actualización.
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
                    <strong>Escenario 1: Creación exitosa de perfil</strong><br>
                    <strong>Dado que</strong> el administrador proporciona información completa del residente<br>
                    <strong>Cuando</strong> envía el formulario de registro<br>
                    <strong>Entonces</strong> el sistema crea el perfil y genera un ID único para el residente.<br><br>
                    <strong>Escenario 2: Datos requeridos faltantes</strong><br>
                    <strong>Dado que</strong> el administrador intenta crear un perfil<br>
                    <strong>Cuando</strong> faltan datos críticos requeridos<br>
                    <strong>Entonces</strong> el sistema muestra mensajes específicos indicando los campos obligatorios.
                </td>
            </tr>
            <tr>
                <td>US13</td>
                <td>Historial médico institucional</td>
                <td>Como administrador quiero gestionar el historial médico completo de cada residente para asegurar continuidad en el cuidado y cumplir con regulaciones sanitarias.</td>
                <td>
                    <strong>Escenario 1: Gestión de historial médico</strong><br>
                    <strong>Dado que</strong> el administrador tiene permisos médicos<br>
                    <strong>Cuando</strong> accede al historial médico de un residente<br>
                    <strong>Entonces</strong> puede ver, agregar y actualizar información médica con registro de fecha y responsable.<br><br>
                    <strong>Escenario 2: Acceso sin permisos médicos</strong><br>
                    <strong>Dado que</strong> un usuario intenta acceder al historial médico<br>
                    <strong>Cuando</strong> no tiene los permisos necesarios<br>
                    <strong>Entonces</strong> el sistema restringe el acceso y muestra un mensaje explicativo.
                </td>
            </tr>
            <tr>
                <td>US14</td>
                <td>Administración de medicamentos</td>
                <td>Como administrador quiero controlar la administración de medicamentos de todos los residentes para garantizar cumplimiento de tratamientos y evitar errores médicos.</td>
                <td>
                    <strong>Escenario 1: Registro de administración de medicamentos</strong><br>
                    <strong>Dado que</strong> el administrador registra la administración de un medicamento<br>
                    <strong>Cuando</strong> el medicamento está disponible en inventario<br>
                    <strong>Entonces</strong> el sistema registra la administración con hora exacta y observaciones.<br><br>
                    <strong>Escenario 2: Medicamento no disponible</strong><br>
                    <strong>Dado que</strong> el administrador intenta registrar una administración<br>
                    <strong>Cuando</strong> el medicamento no está disponible en inventario<br>
                    <strong>Entonces</strong> el sistema muestra una alerta de falta de stock.
                </td>
            </tr>
            <tr>
                <td>US15</td>
                <td>Gestión de visitas familiares</td>
                <td>Como administrador quiero controlar y programar las visitas familiares a los residentes para mantener seguridad, orden y cumplir con los horarios establecidos.</td>
                <td>
                    <strong>Escenario 1: Programación exitosa de visita</strong><br>
                    <strong>Dado que</strong> el administrador programa una nueva visita<br>
                    <strong>Cuando</strong> el horario solicitado está disponible<br>
                    <strong>Entonces</strong> el sistema registra la visita y genera confirmación.<br><br>
                    <strong>Escenario 2: Conflicto de horarios</strong><br>
                    <strong>Dado que</strong> el administrador programa una visita<br>
                    <strong>Cuando</strong> el horario solicitado ya está ocupado<br>
                    <strong>Entonces</strong> el sistema muestra horarios alternativos disponibles.
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
                    <strong>Escenario 1: Envío de recordatorios automáticos</strong><br>
                    <strong>Dado que</strong> existe una cita médica programada<br>
                    <strong>Cuando</strong> se acerca la fecha de la cita<br>
                    <strong>Entonces</strong> el sistema envía recordatorios automáticos a los familiares autorizados.<br><br>
                    <strong>Escenario 2: Falla en envío de recordatorios</strong><br>
                    <strong>Dado que</strong> el sistema intenta enviar recordatorios<br>
                    <strong>Cuando</strong> falla el servicio de notificaciones<br>
                    <strong>Entonces</strong> el sistema registra el error y notifica al administrador.
                </td>
            </tr>
            <tr>
                <td>US17</td>
                <td>Notificaciones de cambios en medicación</td>
                <td>Como familiar quiero ser notificado inmediatamente sobre cualquier cambio en la medicación de mi familiar para estar informado sobre su tratamiento médico.</td>
                <td>
                    <strong>Escenario 1: Notificación de cambio en medicación</strong><br>
                    <strong>Dado que</strong> ocurre un cambio en la medicación del residente<br>
                    <strong>Cuando</strong> el médico actualiza el tratamiento<br>
                    <strong>Entonces</strong> el sistema envía notificación inmediata a familiares autorizados.<br><br>
                    <strong>Escenario 2: Familiar no autorizado</strong><br>
                    <strong>Dado que</strong> ocurre un cambio en la medicación<br>
                    <strong>Cuando</strong> un familiar no está autorizado para recibir esa información<br>
                    <strong>Entonces</strong> el sistema no envía la notificación, respetando las preferencias de privacidad.
                </td>
            </tr>
            <tr>
                <td>US18</td>
                <td>Recordatorios de visitas familiares</td>
                <td>Como familiar quiero recibir recordatorios automáticos sobre mis visitas programadas al adulto mayor para no olvidar las citas y mantener regularidad en el contacto.</td>
                <td>
                    <strong>Escenario 1: Recordatorio de visita programada</strong><br>
                    <strong>Dado que</strong> existe una visita familiar programada<br>
                    <strong>Cuando</strong> se acerca la hora de la visita<br>
                    <strong>Entonces</strong> el sistema envía recordatorio automático al familiar.<br><br>
                    <strong>Escenario 2: Cancelación de visita</strong><br>
                    <strong>Dado que</strong> existe una visita programada<br>
                    <strong>Cuando</strong> ocurre una emergencia que requiere cancelación<br>
                    <strong>Entonces</strong> el sistema envía notificación inmediata de cancelación.
                </td>
            </tr>
            <tr>
                <td>US19</td>
                <td>Alertas de actualización de datos personales</td>
                <td>Como familiar quiero recibir notificaciones automáticas cuando se actualice la información personal o de mi familiar para mantenerme informado de cualquier cambio en su perfil.</td>
                <td>
                    <strong>Escenario 1: Notificación de actualización de datos</strong><br>
                    <strong>Dado que</strong> se actualiza información personal del residente<br>
                    <strong>Cuando</strong> se modifican datos relevantes<br>
                    <strong>Entonces</strong> el sistema envía notificación a familiares autorizados especificando los cambios.<br><br>
                    <strong>Escenario 2: Actualización sin autorización para notificar</strong><br>
                    <strong>Dado que</strong> se actualiza información personal<br>
                    <strong>Cuando</strong> el familiar no tiene autorización para recibir esa información<br>
                    <strong>Entonces</strong> el sistema no envía notificación sobre datos restringidos.
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
                    <strong>Escenario 1: Envío de pregunta sobre cuidados</strong><br>
                    <strong>Dado que</strong> el familiar está autenticado<br>
                    <strong>Cuando</strong> envía una pregunta sobre cuidados<br>
                    <strong>Entonces</strong> la consulta se envía al personal asignado y recibe confirmación.<br><br>
                    <strong>Escenario 2: Canal de comunicación no disponible</strong><br>
                    <strong>Dado que</strong> el familiar intenta enviar una pregunta<br>
                    <strong>Cuando</strong> el sistema de comunicación no está disponible<br>
                    <strong>Entonces</strong> el usuario recibe un mensaje temporal con opciones alternativas.
                </td>
            </tr>
            <tr>
                <td>US21</td>
                <td>Peticiones de modificación de cuidados</td>
                <td>Como familiar quiero solicitar ajustes específicos en el cuidado de mi familiar basados en sus preferencias o necesidades particulares.</td>
                <td>
                    <strong>Escenario 1: Solicitud de modificación de cuidados</strong><br>
                    <strong>Dado que</strong> el familiar tiene permisos para solicitar cambios<br>
                    <strong>Cuando</strong> envía una petición detallada<br>
                    <strong>Entonces</strong> el sistema registra la solicitud con número de seguimiento.<br><br>
                    <strong>Escenario 2: Solicitud que requiere aprobación médica</strong><br>
                    <strong>Dado que</strong> el familiar solicita una modificación<br>
                    <strong>Cuando</strong> la petición involucra aspectos médicos<br>
                    <strong>Entonces</strong> el sistema deriva automáticamente la solicitud al equipo médico.
                </td>
            </tr>
            <tr>
                <td>US22</td>
                <td>Seguimiento del bienestar emocional</td>
                <td>Como familiar quiero comunicarme con el personal sobre el estado emocional y psicológico de mi familiar para asegurar su bienestar integral.</td>
                <td>
                    <strong>Escenario 1: Comunicación sobre estado emocional</strong><br>
                    <strong>Dado que</strong> el familiar está preocupado por el bienestar emocional<br>
                    <strong>Cuando</strong> envía consulta sobre estado anímico<br>
                    <strong>Entonces</strong> el sistema comunica la consulta al área de psicología/trabajo social.<br><br>
                    <strong>Escenario 2: Situación que requiere atención inmediata</strong><br>
                    <strong>Dado que</strong> el familiar reporta cambios emocionales significativos<br>
                    <strong>Cuando</strong> la situación indica posible crisis emocional<br>
                    <strong>Entonces</strong> el sistema escala la situación a atención psicológica prioritaria.
                </td>
            </tr>
            <tr>
                <td>US23</td>
                <td>Planificación de eventos familiares</td>
                <td>Como familiar quiero coordinar con el personal la organización de eventos especiales o celebraciones para mi familiar dentro de las instalaciones.</td>
                <td>
                    <strong>Escenario 1: Coordinación de evento familiar</strong><br>
                    <strong>Dado que</strong> el familiar planifica un evento especial<br>
                    <strong>Cuando</strong> solicita coordinación especificando requerimientos<br>
                    <strong>Entonces</strong> el personal evalúa viabilidad y coordina los recursos necesarios.<br><br>
                    <strong>Escenario 2: Evento no permitido por protocolos</strong><br>
                    <strong>Dado que</strong> el familiar solicita un evento<br>
                    <strong>Cuando</strong> la solicitud no cumple con políticas institucionales<br>
                    <strong>Entonces</strong> el sistema explica las limitaciones y ofrece alternativas.
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
                    <strong>Escenario 1: Registro exitoso de medicamento</strong><br>
                    <strong>Dado que</strong> el administrador registra un nuevo medicamento<br>
                    <strong>Cuando</strong> proporciona todos los datos requeridos<br>
                    <strong>Entonces</strong> el sistema añade el medicamento al inventario y actualiza el stock.<br><br>
                    <strong>Escenario 2: Medicamento duplicado</strong><br>
                    <strong>Dado que</strong> el administrador registra un medicamento<br>
                    <strong>Cuando</strong> intenta ingresar un medicamento con lote duplicado<br>
                    <strong>Entonces</strong> el sistema detecta la duplicación y muestra alerta.
                </td>
            </tr>
            <tr>
                <td>US25</td>
                <td>Alertas de vencimiento</td>
                <td>Como administrador quiero recibir alertas automáticas sobre medicamentos próximos a vencer para evitar pérdidas y riesgos de seguridad.</td>
                <td>
                    <strong>Escenario 1: Alerta por medicamentos próximos a vencer</strong><br>
                    <strong>Dado que</strong> existen medicamentos próximos a vencer<br>
                    <strong>Cuando</strong> faltan 30 días para la fecha de vencimiento<br>
                    <strong>Entonces</strong> el sistema genera alerta automática al administrador.<br><br>
                    <strong>Escenario 2: Medicamentos vencidos en inventario</strong><br>
                    <strong>Dado que</strong> existen medicamentos vencidos<br>
                    <strong>Cuando</strong> el sistema detecta medicamentos vencidos<br>
                    <strong>Entonces</strong> el sistema bloquea automáticamente su uso y genera alerta crítica.
                </td>
            </tr>
            <tr>
                <td>US26</td>
                <td>Eliminación de medicamentos</td>
                <td>Como administrador quiero eliminar medicamentos del inventario de manera controlada para mantener la precisión del stock y cumplir con protocolos de disposición.</td>
                <td>
                    <strong>Escenario 1: Eliminación controlada de medicamento</strong><br>
                    <strong>Dado que</strong> el administrador necesita eliminar un medicamento<br>
                    <strong>Cuando</strong> especifica la razón y justificación<br>
                    <strong>Entonces</strong> el sistema registra la eliminación y actualiza el stock.<br><br>
                    <strong>Escenario 2: Intento de eliminación sin autorización</strong><br>
                    <strong>Dado que</strong> un usuario intenta eliminar un medicamento<br>
                    <strong>Cuando</strong> no posee los permisos necesarios<br>
                    <strong>Entonces</strong> el sistema niega el acceso y registra el intento.
                </td>
            </tr>
            <tr>
                <td>US27</td>
                <td>Búsqueda y filtrado de inventario</td>
                <td>Como administrador quiero filtrar y buscar medicamentos en el inventario para encontrar rápidamente información específica y generar reportes personalizados.</td>
                <td>
                    <strong>Escenario 1: Búsqueda de medicamentos</strong><br>
                    <strong>Dado que</strong> el administrador busca medicamentos<br>
                    <strong>Cuando</strong> utiliza filtros de búsqueda<br>
                    <strong>Entonces</strong> el sistema retorna resultados precisos según los criterios.<br><br>
                    <strong>Escenario 2: Búsqueda sin resultados</strong><br>
                    <strong>Dado que</strong> el administrador busca medicamentos<br>
                    <strong>Cuando</strong> los criterios no coinciden con ningún medicamento<br>
                    <strong>Entonces</strong> el sistema muestra mensaje de "sin resultados".
                </td>
            </tr>
            <tr>
                <td>US28</td>
                <td>Información de medicamentos para personal</td>
                <td>Como administrador quiero proporcionar información detallada sobre medicamentos al personal para asegurar administración segura y correcta.</td>
                <td>
                    <strong>Escenario 1: Acceso a información de medicamentos</strong><br>
                    <strong>Dado que</strong> personal autorizado consulta información<br>
                    <strong>Cuando</strong> accede a detalles de un medicamento<br>
                    <strong>Entonces</strong> el sistema muestra información completa y protocolos de administración.<br><br>
                    <strong>Escenario 2: Medicamento con alertas especiales</strong><br>
                    <strong>Dado que</strong> personal consulta un medicamento<br>
                    <strong>Cuando</strong> el medicamento tiene alertas de seguridad<br>
                    <strong>Entonces</strong> el sistema muestra las alertas prominentemente.
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
                    <strong>Dado que</strong> el administrador registra un nuevo empleado<br>
                    <strong>Cuando</strong> completa la información requerida<br>
                    <strong>Entonces</strong> el sistema crea el perfil y asigna permisos según el rol.<br><br>
                    <strong>Escenario 2: Información incompleta de empleado</strong><br>
                    <strong>Dado que</strong> el administrador registra un empleado<br>
                    <strong>Cuando</strong> faltan datos críticos requeridos<br>
                    <strong>Entonces</strong> el sistema indica qué información falta y no activa permisos.
                </td>
            </tr>
            <tr>
                <td>US30</td>
                <td>Baja de personal</td>
                <td>Como administrador quiero dar de baja empleados del sistema para mantener registros actualizados y gestionar finalizaciones de contratos.</td>
                <td>
                    <strong>Escenario 1: Proceso de baja de empleado</strong><br>
                    <strong>Dado que</strong> el administrador procesa la baja de un empleado<br>
                    <strong>Cuando</strong> especifica fecha de terminación y motivo<br>
                    <strong>Entonces</strong> el sistema desactiva accesos y genera reporte de finalización.<br><br>
                    <strong>Escenario 2: Empleado con responsabilidades activas</strong><br>
                    <strong>Dado que</strong> el administrador intenta dar de baja a un empleado<br>
                    <strong>Cuando</strong> el empleado tiene responsabilidades activas<br>
                    <strong>Entonces</strong> el sistema alerta sobre responsabilidades y requiere reasignación.
                </td>
            </tr>
            <tr>
                <td>US31</td>
                <td>Búsqueda y filtrado de empleados</td>
                <td>Como administrador quiero filtrar y buscar empleados según diferentes criterios para encontrar rápidamente personal específico.</td>
                <td>
                    <strong>Escenario 1: Búsqueda de empleados</strong><br>
                    <strong>Dado que</strong> el administrador busca empleados<br>
                    <strong>Cuando</strong> utiliza filtros de búsqueda<br>
                    <strong>Entonces</strong> el sistema retorna lista precisa de empleados según criterios.<br><br>
                    <strong>Escenario 2: Filtros sin resultados</strong><br>
                    <strong>Dado que</strong> el administrador aplica filtros específicos<br>
                    <strong>Cuando</strong> la combinación no coincide con empleados<br>
                    <strong>Entonces</strong> el sistema muestra mensaje "sin resultados".
                </td>
            </tr>
            <tr>
                <td>US32</td>
                <td>Gestión de horas extra</td>
                <td>Como administrador quiero controlar las horas extra trabajadas por el personal para gestionar costos laborales y cumplir con regulaciones de trabajo.</td>
                <td>
                    <strong>Escenario 1: Registro de horas extra</strong><br>
                    <strong>Dado que</strong> el administrador registra horas extra<br>
                    <strong>Cuando</strong> especifica empleado, fecha, horas y justificación<br>
                    <strong>Entonces</strong> el sistema registra las horas y calcula montos según tarifas.<br><br>
                    <strong>Escenario 2: Horas que exceden límites permitidos</strong><br>
                    <strong>Dado que</strong> el administrador registra horas extra<br>
                    <strong>Cuando</strong> las horas superan los máximos permitidos<br>
                    <strong>Entonces</strong> el sistema muestra alerta y requiere autorización especial.
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
                    <strong>Escenario 1: Configuración de horarios</strong><br>
                    <strong>Dado que</strong> el administrador configura horarios de atención<br>
                    <strong>Cuando</strong> establece horarios por servicio y día<br>
                    <strong>Entonces</strong> el sistema actualiza los horarios en la plataforma.<br><br>
                    <strong>Escenario 2: Cambio de horarios por emergencia</strong><br>
                    <strong>Dado que</strong> el administrador modifica horarios por emergencia<br>
                    <strong>Cuando</strong> debe cambiar horarios por situaciones imprevistas<br>
                    <strong>Entonces</strong> el sistema permite cambios inmediatos con notificación automática.
                </td>
            </tr>
            <tr>
                <td>US34</td>
                <td>Datos de contacto institucional</td>
                <td>Como administrador quiero gestionar la información de contacto de la casa de reposo para que familias y autoridades tengan acceso a datos actualizados.</td>
                <td>
                    <strong>Escenario 1: Actualización de información de contacto</strong><br>
                    <strong>Dado que</strong> el administrador actualiza datos de contacto<br>
                    <strong>Cuando</strong> modifica teléfonos, emails o dirección<br>
                    <strong>Entonces</strong> el sistema actualiza la información en toda la plataforma.<br><br>
                    <strong>Escenario 2: Información de contacto de emergencia</strong><br>
                    <strong>Dado que</strong> existe una situación de emergencia<br>
                    <strong>Cuando</strong> familias necesitan contactar urgentemente<br>
                    <strong>Entonces</strong> tienen acceso inmediato a números de emergencia 24/7.
                </td>
            </tr>
            <tr>
                <td>US35</td>
                <td>Información del personal directivo</td>
                <td>Como administrador quiero gestionar la información del personal directivo para transparencia hacia familias y autoridades.</td>
                <td>
                    <strong>Escenario 1: Gestión de información directiva</strong><br>
                    <strong>Dado que</strong> el administrador actualiza información de personal directivo<br>
                    <strong>Cuando</strong> modifica información de directores o coordinadores<br>
                    <strong>Entonces</strong> el sistema actualiza la información para familias y autoridades.<br><br>
                    <strong>Escenario 2: Acceso a información por autoridades</strong><br>
                    <strong>Dado que</strong> autoridades requieren información directiva<br>
                    <strong>Cuando</strong> necesitan verificar credenciales y responsabilidades<br>
                    <strong>Entonces</strong> pueden acceder a la información completa y actualizada.
                </td>
            </tr>
            <tr>
                <td>US36</td>
                <td>Historia institucional</td>
                <td>Como administrador quiero gestionar la información histórica y reconocimientos de la casa de reposo para generar confianza y credibilidad.</td>
                <td>
                    <strong>Escenario 1: Presentación de historia institucional</strong><br>
                    <strong>Dado que</strong> el administrador gestiona información histórica<br>
                    <strong>Cuando</strong> actualiza historia, certificaciones y logros<br>
                    <strong>Entonces</strong> el sistema presenta la información de manera creíble.<br><br>
                    <strong>Escenario 2: Verificación de certificaciones</strong><br>
                    <strong>Dado que</strong> autoridades verifican certificaciones<br>
                    <strong>Cuando</strong> requieren confirmar validez de licencias<br>
                    <strong>Entonces</strong> pueden acceder a información verificable y contactos de entidades.
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
                    <strong>Escenario 1: Configuración de permisos de usuario</strong><br>
                    <strong>Dado que</strong> el administrador gestiona accesos<br>
                    <strong>Cuando</strong> asigna roles y permisos específicos a usuarios<br>
                    <strong>Entonces</strong> cada usuario accede únicamente a la información autorizada para su rol.<br><br>
                    <strong>Escenario 2: Intento de acceso no autorizado</strong><br>
                    <strong>Dado que</strong> un usuario intenta acceder a información<br>
                    <strong>Cuando</strong> intenta ver datos que no le corresponden según su rol<br>
                    <strong>Entonces</strong> el sistema bloquea el acceso y registra el intento.
                </td>
            </tr>
            <tr>
                <td>US38</td>
                <td>Protección de datos mediante cifrado</td>
                <td>Como administrador quiero que toda la información sensible esté cifrada para proteger los datos personales y médicos de accesos no autorizados.</td>
                <td>
                    <strong>Escenario 1: Cifrado de datos sensibles</strong><br>
                    <strong>Dado que</strong> el sistema almacena información personal y médica<br>
                    <strong>Cuando</strong> se guardan datos sensibles o se comunican<br>
                    <strong>Entonces</strong> toda la información se cifra automáticamente antes del almacenamiento y transmisión.<br><br>
                    <strong>Escenario 2: Intento de acceso a datos cifrados sin autorización</strong><br>
                    <strong>Dado que</strong> hay un intento de acceso directo a datos cifrados<br>
                    <strong>Cuando</strong> alguien intenta acceder sin autorización apropiada<br>
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
                    <strong>Escenario 1: Navegación consistente</strong><br>
                    <strong>Dado que</strong> el usuario se encuentra en cualquier página<br>
                    <strong>Cuando</strong> utiliza el menú de navegación<br>
                    <strong>Entonces</strong> encuentra las mismas opciones organizadas idénticamente.<br><br>
                    <strong>Escenario 2: Menú adaptado a permisos</strong><br>
                    <strong>Dado que</strong> usuarios con diferentes roles acceden al sistema<br>
                    <strong>Cuando</strong> navegan por la plataforma<br>
                    <strong>Entonces</strong> ven solo las opciones de menú apropiadas para su rol.
                </td>
            </tr>
            <tr>
                <td>US41</td>
                <td>Paleta de colores y tipografía</td>
                <td>Como usuario quiero una interfaz con colores y tipografía consistentes para tener una experiencia visual agradable y fácil de leer.</td>
                <td>
                    <strong>Escenario 1: Aplicación consistente de diseño visual</strong><br>
                    <strong>Dado que</strong> se muestra cualquier página de la plataforma<br>
                    <strong>Cuando</strong> el usuario navega por diferentes secciones<br>
                    <strong>Entonces</strong> encuentra colores y tipografía consistentes y legibles.<br><br>
                    <strong>Escenario 2: Adaptación para necesidades especiales</strong><br>
                    <strong>Dado que</strong> usuarios con dificultades visuales acceden<br>
                    <strong>Cuando</strong> acceden a la plataforma<br>
                    <strong>Entonces</strong> pueden utilizar funciones de alto contraste o aumento de texto.
                </td>
            </tr>
            <tr>
                <td>US42</td>
                <td>Diseño de formularios usables</td>
                <td>Como usuario quiero formularios claros y fáciles de completar para ingresar información sin confusión ni errores.</td>
                <td>
                    <strong>Escenario 1: Completar formularios</strong><br>
                    <strong>Dado que</strong> el usuario completa un formulario<br>
                    <strong>Cuando</strong> ingresa información requerida<br>
                    <strong>Entonces</strong> recibe validación en tiempo real y confirmación al enviar.<br><br>
                    <strong>Escenario 2: Formulario con errores de validación</strong><br>
                    <strong>Dado que</strong> el usuario envía un formulario con información incorrecta<br>
                    <strong>Cuando</strong> existen errores en los datos ingresados<br>
                    <strong>Entonces</strong> recibe mensajes de error específicos para cada campo.
                </td>
            </tr>
            <tr>
                <td>US43</td>
                <td>Patrones de diseño coherentes</td>
                <td>Como usuario quiero que todas las pantallas sigan patrones de diseño similares para predecir dónde encontrar funciones y cómo interactuar.</td>
                <td>
                    <strong>Escenario 1: Interacción predecible</strong><br>
                    <strong>Dado que</strong> el usuario está familiarizado con una sección<br>
                    <strong>Cuando</strong> navega a nuevas secciones<br>
                    <strong>Entonces</strong> encuentra patrones de interacción similares y predecibles.<br><br>
                    <strong>Escenario 2: Nuevos usuarios aprendiendo la interfaz</strong><br>
                    <strong>Dado que</strong> un nuevo usuario accede por primera vez<br>
                    <strong>Cuando</strong> explora diferentes funcionalidades<br>
                    <strong>Entonces</strong> puede predecir cómo funcionarán nuevas secciones.
                </td>
            </tr>
            <tr>
                <td>US44</td>
                <td>Manejo de errores comprensible</td>
                <td>Como usuario quiero que los errores se presenten de forma clara y con soluciones sugeridas para resolver problemas sin frustración.</td>
                <td>
                    <strong>Escenario 1: Error del sistema con guía de resolución</strong><br>
                    <strong>Dado que</strong> ocurre un error técnico<br>
                    <strong>Cuando</strong> el usuario lo experimenta<br>
                    <strong>Entonces</strong> recibe un mensaje claro explicando qué ocurrió y pasos para resolverlo.<br><br>
                    <strong>Escenario 2: Error de usuario con orientación</strong><br>
                    <strong>Dado que</strong> el usuario comete un error<br>
                    <strong>Cuando</strong> realiza una acción no permitida<br>
                    <strong>Entonces</strong> recibe una explicación clara y orientación sobre la forma correcta.
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
  <tr><td>45</td><td>TS01</td><td>Eliminar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Delete para medicamentos para asegurar que el administrador de la casa de reposo pueda remover registros del inventario.</td><td>2</td></tr>
  <tr><td>46</td><td>TS02</td><td>Agregar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un EndPoint Post medicamentos para permitir que el administrador de la casa de reposo pueda agregar más medicamentos.</td><td>2</td></tr>
  <tr><td>47</td><td>TS03</td><td>Ver información detallada de los medicamentos</td><td>Como desarrollador backend en NovaPeru Tech quiero crear una función para ver la información a través de una Api.</td><td>1</td></tr>
  <tr><td>48</td><td>TS04</td><td>Actualizar información de medicamentos</td><td>Como desarrollador de backend en NovaPeru Tech quiero crear una función para actualizar la información para asegurar que el administrador de la casa de reposos pueda mantener actualizada la información de cada medicamento.</td><td>2</td></tr>
  <tr><td>49</td><td>TS05</td><td>Agregar pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para permitir que el administrador registre nuevos residentes con validaciones obligatorias y que se genere un ID único por residente.</td><td>2</td></tr>
  <tr><td>50</td><td>TS06</td><td>Ver información detallada de los pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que devuelva la información completa del residente para que el personal autorizado pueda consultar fácilmente el expediente.</td><td>1</td></tr>
  <tr><td>51</td><td>TS07</td><td>Eliminar paciente</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE que realice una eliminación controlada del residente.</td><td>3</td></tr>
<tr><td>52</td><td>TS08</td><td>Actualizar información de los pacientes</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar campos del perfil del residente para que las modificaciones queden registradas y sean reversibles si es necesario.</td><td>2</td></tr>
<tr><td>53</td><td>TS09</td><td>Agregar información detallada de la casa de reposo</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que un administrador pueda registrar información institucional.</td><td>2</td></tr>
<tr><td>54</td><td>TS10</td><td>Actualizar información de la casa de reposo</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PUT para mantener actualizados los datos institucionales.</td><td>2</td></tr>
<tr><td>55</td><td>TS11</td><td>Agregar empleado</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint POST para que registre nuevos empleados.</td><td>2</td></tr>
<tr><td>56</td><td>TS12</td><td>Eliminar empleado</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint DELETE para que el administrador de la casa de reposo revoque persmisos.</td><td>3</td></tr>
<tr><td>57</td><td>TS13</td><td>Actualizar información del empleado</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint PATCH para actualizar datos de empleado.</td><td>2</td></tr>
<tr><td>58</td><td>TS14</td><td>Ver información del empleado</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET que muestre el perfil del empleado para que el administrador pueda observar cuantos empleados tiene.</td><td>1</td></tr>
<tr><td>59</td><td>TS15</td><td>Consumir Api de Medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero consumir la API externa de medicamentos mediante un servicio de integración , para disponer de información confiable y actualizada de medicamentos en el sistema.</td><td>3</td></tr>
<tr><td>60</td><td>TS16</td><td>Consumir Api de google maps</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de integración con Google Maps que proporcione verificación de direcciones y datos de localización para manejar errores.</td><td>3</td></tr>
<tr><td>61</td><td>TS17</td><td>Notificación de visitas</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un servicio de notificaciones para enviar recordatorios y alertas de visitas vía email/SMS.</td><td>3</td></tr>
<tr><td>62</td><td>TS18</td><td>Buscar y filtrar medicamentos</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET con parámetros de búsqueda facilitar consultas rápidas y generación de reportes.</td><td>2</td></tr>
<tr><td>63</td><td>TS19</td><td>Buscar y filtrar residentes</td><td>Como desarrollador backend en NovaPeru tech quiero implementar un endpoint GET con filtros para que administradores y personal autorizado encuentren residentes fácilmente.</td><td>2</td></tr>
<tr><td>64</td><td>TS20</td><td>Buscar y filtrar empleados</td><td>Como desarrollador backend en NovaPeru tech quiero crear un endpoint GET que permita buscar y filtrar por nombre, rol, turno que se pueda exportar para que vea el reporte de empleados el admnistrador o RRHH.</td><td>3</td></tr>
</table>
