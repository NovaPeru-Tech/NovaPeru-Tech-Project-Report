# Capítulo IV: Product Design

## 4.1. Style Guidelines

### 4.1.1. General Style Guidelines

El diseño visual de la plataforma **Veyra** se inclina hacia una estética moderna, limpia y amigable, en línea con nuestro compromiso de ofrecer soluciones de cuidado que transmitan confianza, claridad y facilidad de uso. Nuestro objetivo es crear una experiencia digital que sea tanto eficiente como reconfortante para las familias y las instituciones de cuidado.

En este capítulo, detallaremos cada uno de los elementos visuales y de estilo que guían el desarrollo de la aplicación Veyra, siempre siguiendo los principios de Diseño de Experiencia de Usuario (UX) e Interfaz de Usuario (UI) para garantizar la máxima usabilidad y accesibilidad.

**Branding**

El logo principal de nuestra plataforma es *Veyra*, un nombre que evoca cercanía y visión en el cuidado. Nuestro propósito es ser un puente digital para el cuidado de los adultos mayores, ofreciendo una solución integral para gestores de cuidado y familias. El branding se enfoca en transmitir innovación, soporte y confiabilidad, valores esenciales para quienes confían en nosotros el bienestar de sus seres queridos.
<br>

<p align="center">
  <img src="../images/Veyra-logo.jpeg" alt="Veyra-Logo" width="350px" height="auto"/>
</p>

**Typography**

La tipografía empleada en Veyra será **Rubik**, con sus variantes Regular, Medium, SemiBold y Bold. La elección de Jost se basa en su estética moderna y profesional, que se equilibra con una excelente legibilidad en diversas resoluciones y dispositivos (móviles, tabletas, ordenadores). Además, su disponibilidad a través de Google Fonts asegura una carga eficiente y consistente.

La jerarquía tipográfica se establece de la siguiente manera para garantizar claridad y ritmo visual:

- **Títulos principales (H1/Sección heading):** 4rem (aprox. 64px) en escritorio, 2.8rem (aprox. 45px) en móvil.

- **Subtítulos (H2/Sub-headings):** 2.8rem (aprox. 45px) en escritorio, 2.2rem (aprox. 35px) en móvil.

- **Títulos de componentes (H3/H4):** 2rem (aprox. 32px) a 2.2rem (aprox. 35px).

- **Cuerpo del texto (p):** 1.6rem (aprox. 16px) con un interlineado de 1.6.

- **Botones y etiquetas (span):** 1.4rem (aprox. 14px) a 1.8rem (aprox. 18px).

<p align="center">
  <img src="../images/typografy-Veyra.jpg" alt="Primary Color Palette" width="500px" height="auto"/>
</p>

Esta distribución garantiza un contraste óptimo entre el texto y el fondo, superando un ratio mínimo de 4.5:1 según las WCAG 2.1 AA para una accesibilidad superior.

<br>

**Colors**

Nuestra paleta de colores ha sido cuidadosamente seleccionada para evocar sensaciones de calma, profesionalismo y confianza. Se ha distribuido en tres categorías principales:

**Paleta principal**: Colores que definen la identidad de Veyra y se usan en elementos clave.
* **Primario (Azul Veyra):** var(--primary-color) (referencia principal).
* **Secundario (Azul Profundo):** var(--secondary-color) (para texto principal y elementos interactivos).
* **Terciario (Gris Oscuro):** var(--tertiary-color) (para texto secundario y detalles).
* **Fondo Claro:** var(--bg-light) (fondos de secciones).
* **Fondo Blanco:** var(--white) (fondos de tarjetas y elementos principales).
  
**Paleta de Soporte**: Colores complementarios que añaden profundidad y contraste.
* **Gris Neutro:** Para bordes sutiles, líneas divisorias y fondos de alternancia.

**Colores Funcionales**: Reservados para comunicar estados específicos al usuario.
* **Éxito:** Verde (#4CAF50) para confirmaciones y acciones exitosas.
* **Error:** Rojo (#F44336) para alertas y mensajes de error.
* **Advertencia:** Amarillo (#FFC107) para notificaciones y avisos importantes.


<p align="center">
  <img src="../images/Color Pallete.png" alt="Primary Color Palette" width="800px" height="auto"/>
</p>

Esta combinación cromática refleja los valores de nuestra marca y busca transmitir al público una imagen de profesionalismo, seguridad y calidez en el cuidado de adultos mayores.
<br>

**Spacing**

El espaciado en Veyra sigue un sistema de espaciado modular y consistente para garantizar un ritmo visual armonioso y una jerarquía clara en toda la interfaz. La consistencia en el espaciado ayuda a reducir la carga cognitiva del usuario y mejora la legibilidad.

* **Espaciado Básico:** Usamos un espaciado base de 0.5rem (8px) para elementos pequeños como iconos, botones y texto. Este valor es la unidad mínima y se multiplica para crear espacios más grandes.

* **Margen Interno (Padding) Generoso:** Las secciones principales de la página utilizan un padding vertical de 6rem (96px) para crear pausas visuales claras. Los contenedores de tarjetas o elementos secundarios usan padding más pequeños, como 2.5rem (40px), para agrupar el contenido de forma lógica.

* **Espacio entre Elementos:** El espaciado entre elementos relacionados, como las tarjetas de planes o los miembros del equipo, varía entre 1.5rem (24px) y 3rem (48px). Esto mantiene una densidad de información adecuada sin abrumar visualmente al usuario.

* **Line Height del Texto:** El interlineado del texto (line-height) está configurado en 1.6, lo que facilita la lectura de párrafos largos y evita que las líneas se sientan demasiado juntas.

<br>

**Tono de Comunicación**

La voz y el tono de Veyra están diseñados para ser tan confiables y amigables como nuestra plataforma. Nuestro objetivo es conectar con familias e instituciones de cuidado de manera empática y profesional.

* **Tono: Amigable y empático,** con un toque de profesionalismo. Buscamos proyectar cercanía y comprensión de las necesidades de nuestros usuarios (familias), mientras mantenemos la autoridad y la seriedad que esperan las instituciones de cuidado.

* **Actitud: Confiable y serena.** El 90% de nuestra comunicación es tranquilizadora y segura, mientras que el 10% restante es entusiasta, especialmente en los llamados a la acción (CTAs) para motivar al usuario.

* **Lenguaje: Claro y directo.** Evitamos la jerga técnica innecesaria. Nos enfocamos en los beneficios que Veyra aporta a la vida diaria de las familias y los gestores de cuidado, hablando en términos de paz mental, eficiencia y conexión.

* **Voz: Experta y cálida.** Posicionamos a Veyra como una solución líder en tecnología de cuidado, pero siempre con un enfoque humano y comprensivo.

Este enfoque comunicacional busca generar confianza y lealtad, asegurando a las familias que están tomando la mejor decisión para sus seres queridos, y a las instituciones, que están optimizando sus procesos con una herramienta de vanguardia.


### 4.1.2. Web Style Guidelines

Las directrices de estilo web de Veyra se centran en la simplicidad, la accesibilidad y la modernidad. Nuestro objetivo es crear una experiencia visual que refleje la misión de nuestra plataforma: conectar y simplificar el cuidado de los adultos mayores con un diseño limpio e intuitivo.

**1) Layout**

* **Sistema de Grid:** Utilizamos un diseño de cuadrícula flexible para garantizar que el contenido de Veyra se vea bien en cualquier dispositivo. Este enfoque permite que las tarjetas de servicios y planes se ajusten dinámicamente, manteniendo el orden y la coherencia visual.
* **Headers y Footers:** El encabezado (header) es fijo en la parte superior, proporcionando acceso constante a la navegación principal y los botones de acción (Sign In, Sign Up). El pie de página (footer) es completo y funcional, con enlaces esenciales que complementan la experiencia del usuario.
* **Cards:** Las tarjetas son un componente central en nuestro diseño. Se usan para destacar los servicios, beneficios y testimonios. Tienen bordes redondeados y sombras suaves para darles una apariencia moderna y hacer que el contenido se sienta "elevado" y fácil de leer.

**2) Responsive Design**

* **Desktop:** La navegación principal es visible en la barra superior junto a los botones de inicio de sesión. El contenido se presenta en múltiples columnas para un uso eficiente del espacio de la pantalla.
* **Tablet:** El menú de navegación se oculta en un botón de hamburguesa para maximizar el espacio. Los elementos de la cuadrícula se adaptan a un diseño de dos columnas. Los botones y formularios se expanden para ser fáciles de tocar.
* **Mobile:** La experiencia está optimizada para la visualización en una sola columna. La navegación se realiza a través de un menú desplegable, y todos los elementos interactivos, como botones y campos de entrada, son grandes y claros, ideales para pantallas táctiles.

**3) Interaction Design**

* **Botones:** Nuestros botones son llamativos y fáciles de hacer clic, con efectos visuales sutiles al pasar el cursor para confirmar la interactividad. El botón principal de llamado a la acción (Start now →) destaca claramente del resto.

* **Formularios:** El formulario de contacto en el pie de página es sencillo y directo. Los campos son claros y están bien espaciados para evitar errores del usuario.

**4) Images and Icons**

* **Imágenes:** Se utilizan fotografías de alta calidad que evocan calidez, conexión y cuidado. Las imágenes de personas mayores y familias interactuando refuerzan el mensaje de Veyra. Las imágenes están optimizadas para una carga rápida.

* **Íconos:** Empleamos un conjunto de íconos de estilo lineal y minimalista. Estos iconos se utilizan para representar servicios y características, ofreciendo una guía visual rápida y coherente en toda la página.

**5) Repositorio Central**

* **Organización:** El proyecto sigue una estructura de archivos lógica. Los estilos están en la carpeta assets/style.css, y los archivos JavaScript en assets/scripts. Todos los activos visuales (imágenes, logos) se encuentran centralizados en assets/images y assets/logos, respectivamente.

* **Versionado:** Usamos un sistema de control de versiones como Git para gestionar los cambios en los archivos de estilo y contenido. Esto asegura que todos los colaboradores trabajen en la versión más reciente del proyecto.

## 4.2. Information Architecture

La arquitectura de la información de la página de inicio de Veyra está diseñada para una navegación intuitiva, permitiendo que los usuarios encuentren rápidamente la información que necesitan y comprendan el valor de nuestra plataforma.

### 4.2.1. Organization Systems

* **Jerarquía de Contenidos:** La información está estructurada de lo general a lo específico. Comenzamos con un mensaje de impacto en la sección Hero, seguido de un resumen de nuestros servicios, y luego profundizamos en las características y beneficios en las secciones subsiguientes.
  
* **Secciones Principales:** La página de inicio está organizada en secciones clave:
    * **Hero:** La promesa de Veyra.

    * **What We Offer:** Una visión general de los servicios.

    * **Features:** Los beneficios clave del producto.

    * **Benefits:** Cómo Veyra ayuda a los usuarios.

    * **About Us:** Quiénes somos.

    * **Our Team:** Las personas detrás del proyecto.

    * **Plans:** Opciones de precios.

    * **Testimonials & CTA:** Reseñas y llamado a la acción final.

* **Agrupación de Contenidos:** El contenido se agrupa lógicamente para facilitar la comprensión. Por ejemplo, los beneficios se agrupan en tarjetas con títulos claros y párrafos descriptivos, mientras que los testimonios se presentan en un formato de cuadrícula fácil de escanear.

### 4.2.2. Labeling Systems

* **Nomenclatura:** Se utiliza un lenguaje claro y directo en los títulos de las secciones (What we offer, Features, Plans). Los botones tienen etiquetas descriptivas como Start now →, Sign In y Sign Up para que el usuario sepa exactamente qué esperar.

* **Consistencia:** Mantenemos una nomenclatura uniforme. Por ejemplo, la sección de precios se llama Plans en la barra de navegación y en el título de la sección, evitando confusiones.

* **Lenguaje Adaptativo:** El contenido está diseñado para ser fácil de entender para todos, utilizando un lenguaje que resuena con familias y cuidadores de personas mayores, sin jerga técnica.

### 4.2.3. SEO Tags and Meta Tags

* **Title Tags:**
  
    * **Landing Page:** "Veyra - The Best Care is Always Connected"

* **Meta Description:**
  
    * **Landing Page:** "Veyra es una plataforma digital que conecta a familias y cuidadores, ofreciendo una gestión transparente y segura del cuidado de adultos mayores."

* **Keywords:**
  
    * **Landing Page:** "cuidado de adultos mayores, gestión de cuidado, plataforma para cuidadores, salud familiar, bienestar senior, Veyra"

* **Meta Author:**
  
    * **Landing Page:** "NovaPeru Tech"
 
* **Meta Charset:**
  
    * "UTF-8"
 
* **Meta Viewport:**
  
    * "width=device-width, initial-scale=1.0"
 
### 4.2.4. Searching Systems

* **Barra de Búsqueda:** Aunque la página de inicio no requiere una barra de búsqueda, una vez que el usuario inicia sesión en la aplicación principal, esta funcionalidad será clave. Estará ubicada en un lugar prominente y permitirá buscar rápidamente información de residentes, historial médico y otros datos relevantes.

* **Filtros y Facetas:** Dentro de la aplicación, los usuarios podrán filtrar la información por residente, tipo de medicamento, fecha, etc., para encontrar lo que necesitan de manera eficiente.

* **Historial de Búsqueda:** Se implementará un historial para que el personal de enfermería y los administradores puedan acceder rápidamente a las búsquedas frecuentes.

* **Resultados Relevantes:** Los resultados de búsqueda se priorizarán según la relevancia para la cuenta y las funciones del usuario.


### 4.2.5. Navigation Systems

* **Navegación Global:** La barra de navegación en el encabezado proporciona acceso principal a las secciones de la página de inicio. El menú de hamburguesa en dispositivos móviles asegura que esta navegación sea siempre accesible.

* **Navegación Contextual:** Enlaces internos, como los botones en la sección What We Offer y los botones de llamado a la acción, guían al usuario de manera contextual a la siguiente etapa de su recorrido.

* **Navegación Secundaria:** Enlaces internos, como los botones en la sección What We Offer y los botones de llamado a la acción, guían al usuario de manera contextual a la siguiente etapa de su recorrido.

## 4.3. Landing Page UI Design

El diseño de la interfaz de usuario (UI) de la página de inicio de Veyra es fundamental para captar la atención de los visitantes y guiarlos hacia una acción clara: conectar con el cuidado de sus seres queridos. Nos hemos centrado en la creación de una experiencia intuitiva y fluida, garantizando que cada elemento de la página sea interactivo y fácil de usar, reflejando el compromiso de Veyra con la simplicidad y la transparencia.

### 4.3.1. Landing Page Wireframe

El wireframe de nuestra página de inicio sirve como un mapa visual que define la estructura y el flujo de la información. Este esquema asegura una disposición lógica de los componentes, facilitando la navegación y destacando la propuesta de valor de Veyra. Las secciones del wireframe están diseñadas para contar una historia completa y persuasiva:

**Nav y Hero:**

Esta sección de entrada incluye el logotipo de Veyra, acompañado de un eslogan que resume nuestra promesa: "The Best Care is Always Connected" (El Mejor Cuidado Siempre Está Conectado). La barra de navegación permite un acceso rápido a secciones clave como Features, Benefits, y About Us, mientras que el área principal ofrece una visión concisa del producto, acompañada de un claro llamado a la acción: "Start now →" (Empieza ahora →). Un visual atractivo refuerza el mensaje de calidez y conexión familiar.

<img src="../images/hero-section-landing-wireframe.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">


**Services (What We Offer):**

Aquí se detallan los servicios principales de Veyra: Home Health Care, Pediatric Care, Companion Care y Conditions Treated. Cada servicio se presenta con un ícono representativo y una breve descripción, haciendo que nuestra oferta sea fácil de entender y visualmente accesible.

<img src="../images/whatweoffer-section-landing-wireframe.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">


**Acerca de la aplicación (About the Platform):**

Esta sección presenta lo que hace única a Veyra: una plataforma diseñada para centros de cuidado de adultos mayores que optimiza la gestión clínica y la comunicación. Explicamos cómo Veyra centraliza la información para mejorar la eficiencia, reducir errores y, lo más importante, dar tranquilidad a las familias. Enfatizamos nuestros valores de transparencia, seguridad y conexión, mostrando una lista de beneficios clave como la comunicación fluida, el acceso a información en tiempo real y la seguridad de los datos.

<img src="../images/benefits-section-landing-wireframe.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

**Sobre el Equipo (Our Team):**

En esta sección, se humaniza la marca al presentar al equipo detrás de Veyra. Con fotos y descripciones de los miembros, mostramos a las personas dedicadas a este proyecto, construyendo confianza y una conexión personal con los visitantes.

<img src="../images/ourteam-section-landing-wireframe.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

**Precios (Plans):**

La sección de Precios ofrece una visión clara de los planes disponibles. Presentamos el Family Plan y el Nursing Home Plan, con un comparativo de características para ayudar a los usuarios a elegir la opción que mejor se adapte a sus necesidades, ya sea para el cuidado en casa o para una institución. Un conmutador entre tarifas mensuales y anuales, junto con la indicación de un ahorro, hace la elección más informada.

<img src="../images/plans-section-landing-wireframe.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

**Footer:**
El pie de página es un elemento crucial para la usabilidad. Contiene enlaces a información vital como "Terms of Service" y "Privacy Policy", además de detalles de contacto (correo electrónico, teléfono y ubicación). Esto proporciona un acceso rápido a la información sin saturar la interfaz, ofreciendo un cierre limpio y funcional a la página.

<img src="../images/footer-section-landing-wireframe.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

Este wireframe sienta las bases para un diseño visual que no solo se ve bien, sino que también guía al usuario de manera intuitiva a través de nuestra propuesta de valor, reforzando la confianza y la conexión que Veyra promete.

### 4.3.2. Landing Page Mock-up

**Hero de la aplicación** 

El hero de nuestra plataforma Veyra presenta una imagen principal que evoca cuidado y conexión, con un título claro: "The Best Care is Always Connected". Una breve descripción capta nuestra esencia, y un botón de llamado a la acción "Start for free →" invita a los usuarios a dar el primer paso. Una barra de navegación en la parte superior permite acceder de forma fluida a todas las secciones de la página, proporcionando una experiencia de usuario intuitiva.

<img src="../images/hero-section-landing.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

**What We Offer** 

En la sección "What We Offer", presentamos nuestras principales áreas de servicio a través de tarjetas con iconos representativos. Cada tarjeta tiene un título y una breve descripción, como "Home Health Care" o "Pediatric Care", lo que permite a los usuarios entender rápidamente el alcance de nuestra plataforma y los tipos de cuidado que apoyamos.

<img src="../images/features-section-landing.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

**Features** 

La sección de "Features" muestra las funcionalidades clave de Veyra. El diseño tipo acordeón permite a los usuarios expandir cada característica para leer su descripción completa, mientras que un video de demostración de YouTube al lado les ofrece una vista visual de la plataforma en acción. Esto combina información detallada con un formato interactivo y dinámico.

<img src="../images/whatweoffer-section-landing.png" alt="Landing Page Mockup" style="max-width: 100%; height: auto; border: 2px solid #00bfff;">

**Benefits** 

En "Benefits", destacamos las ventajas de utilizar Veyra. A través de un diseño de tarjetas con imágenes, títulos y descripciones, comunicamos cómo nuestra plataforma mejora la comunicación, agiliza la gestión clínica y aumenta la tranquilidad tanto para las familias como para las instituciones de cuidado.

<img src="../images/benefits-section-landing.png" alt="Landing Page Mockup" style="width: auto; height: auto; border: 2px solid #00bfff;">

**About Us** 

La sección "About Us" presenta a NovaPeru Tech, la empresa detrás de Veyra. Aquí, compartimos nuestra misión y los valores de innovación y confianza que nos impulsan. Un video o imagen animada acompaña el texto, reforzando nuestro mensaje de una manera visualmente atractiva y moderna.

<img src="../images/aboutus-section-landing.png" alt="Landing Page Mockup" style="width: auto; height: auto; border: 2px solid #00bfff;">

**Our Team** 

La sección "Our Team" presenta a los ingenieros de software detrás de Veyra. Las tarjetas de perfil muestran una foto, el nombre, el cargo y una breve biografía de cada miembro. El diseño de 3 tarjetas arriba y 2 abajo, centradas, brinda un aspecto organizado y profesional, permitiendo a los usuarios conocer al equipo de desarrollo.

<img src="../images/ourteam-section-landing.png" alt="Landing Page Mockup" style="width: auto; height: auto; border: 2px solid #00bfff;">

**Plans** 

En la sección de "Plans", ofrecemos los detalles de nuestros planes de precios. Las tarjetas de "Family Plan" y "Nursing Home Plan" incluyen descripciones, precios con opciones mensuales y anuales, y listas de características. El diseño permite un fácil cambio entre planes mensuales y anuales, facilitando la elección del plan adecuado.

<img src="../images/plans-section-landing.png" alt="Landing Page Mockup" style="width: auto; height: auto; border: 2px solid #00bfff;">

**Footer** 

El "Footer" de nuestra landing page contiene enlaces útiles y recursos adicionales. Un formulario de suscripción invita a los usuarios a unirse a nuestra comunidad. El logo de Veyra, enlaces de contacto, información legal y de derechos de autor se encuentran aquí, asegurando que toda la información relevante esté fácilmente accesible para los usuarios.

<img src="../images/footer-section-landing.png" alt="Landing Page Mockup" style="width: auto; height: auto; border: 2px solid #00bfff;">

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes
<p>
En esta sección se presentan los <strong>wireframes diseñados para la aplicación web de NovaPeru Tech (Veyra)</strong>. 
Cada pantalla responde a las funcionalidades principales del sistema y a los distintos roles de usuario 
(Administrador, Familiar, Personal de cuidado).
</p>

<h5>Login – NovaPeru Tech</h5>
<p>Pantalla de inicio donde los usuarios acceden a la aplicación según su rol 
(Administrador, Familiar, Personal de cuidado). Incluye campos de correo y contraseña, además de validaciones de acceso.</p>

<img src="../images/Login-NovaPeru-Tech.jpg" alt="Login" style="width: auto; height: auto; border: 2px solid #00bfff;">

<h5>Inicio de Sesión – NovaPeru Tech</h5>
<p>Formulario de acceso con credenciales de usuario. Presenta opciones de recuperación de contraseña y mantiene consistencia visual con la identidad de NovaPeru Tech.</p>

<img src="../images/IniciodeSesión-NovaPeru-Tech.jpg" alt="Inicio de Sesión" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Registrar Familiar – NovaPeru Tech</h5>
<p>Formulario para que los familiares creen una cuenta, ingresando datos personales básicos, correo electrónico y contraseña. Incluye validaciones de formato y confirmación de correo.</p>

<img src="../images/RegistrarFamiliar-NovaPeru-Tech.jpg" alt="Registrar Familiar" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Registrar Administrador – NovaPeru Tech</h5>
<p>Pantalla destinada a registrar un nuevo administrador en la plataforma. Permite ingresar información personal, datos de contacto y credenciales de acceso.</p>

<img src="../images/RegistrarAdministrador-NovaPeru-Tech.jpg" alt="Registrar Administrador" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Inventario – NovaPeru Tech</h5>
<p>Módulo donde el administrador puede visualizar el inventario de medicamentos y recursos clínicos. Permite filtrar, ordenar y consultar detalles de cada ítem.</p>

<img src="../images/Inventario-NovaPeru-Tech.jpg" alt="Inventario" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Inventario – Modificar – NovaPeru Tech</h5>
<p>Sección para editar la información de medicamentos en el inventario: nombre, cantidad, fecha de vencimiento, laboratorio y observaciones.</p>

<img src="../images/Inventario-Modificar-NovaPeru-Tech.jpg" alt="Inventario Modificar" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Paciente – NovaPeru Tech</h5>
<p>Pantalla que muestra la información general de un residente (datos personales, estado clínico, actividades recientes).</p>

<img src="../images/Paciente-NovaPeru-Tech.jpg" alt="Paciente" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Paciente – Agregar – NovaPeru Tech</h5>
<p>Formulario para registrar un nuevo residente en la institución. Incluye datos personales, médicos, contactos de emergencia y observaciones.</p>

<img src="../images/Paciente-Agregar-NovaPeru-Tech.jpg" alt="Paciente Agregar" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Paciente – Eliminar – NovaPeru Tech</h5>
<p>Módulo que permite al administrador eliminar registros de pacientes, con mensaje de confirmación para evitar acciones accidentales.</p>

<img src="../images/Paciente-Eliminar-NovaPeru-Tech.jpg" alt="Paciente Eliminar" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Empleado – NovaPeru Tech</h5>
<p>Pantalla donde se listan los empleados de la institución, mostrando nombre, rol, contacto y estado laboral.</p>

<img src="../images/Empleado-NovaPeru-Tech.jpg" alt="Empleado" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Empleado – Card Detalles – NovaPeru Tech</h5>
<p>Vista detallada de un empleado en formato de card, mostrando información personal, turno asignado, horas extra y contacto de emergencia.</p>

<img src="../images/Empleado-Card-Detalles-NovaPeru-Tech.jpg" alt="Empleado Card Detalles" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Actividad – Familiar – NovaPeru Tech</h5>
<p>Pantalla que muestra las actividades recientes del residente (ejercicios, visitas, terapias). 
El familiar puede visualizar fotos, descripciones y fechas.</p>

<img src="../images/Actividad-Familiar-NovaPeru-Tech.jpg" alt="Actividad Familiar" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Historial de Pedido – NovaPeru Tech</h5>
<p>Pantalla que permite consultar pedidos realizados, con detalles de estado, fecha y productos solicitados.</p>

<img src="../images/Historial-de-Pedido-NovaPeru-Tech.jpg" alt="Historial de Pedido" style="width:auto; height:auto; border:2px solid #00bfff;">

### 4.4.2. Web Applications Wireflow Diagrams
<p>Los Wireflows se emplean principalmente en el diseño de la experiencia de usuario (UX) y son especialmente útiles para aplicaciones que incluyen flujos de trabajo e interacciones complejas.</p>

<img src="../images/Web-Applications-Wireflow-Diagrams.jpg" alt="Web-Applications-Wireflow-Diagrams" style="width:auto; height:auto; border:2px solid #00bfff;">

### 4.4.3. Web Applications Mock-ups
<p>
En esta sección se presentan los <strong>mock-ups diseñados para la aplicación web de NovaPeru Tech (Veyra)</strong>. 
Cada pantalla responde a las funcionalidades principales del sistema y a los distintos roles de usuario 
(Administrador, Familiar, Personal de cuidado).
</p>

<h5>Login – NovaPeru Tech</h5>
<p>Pantalla de inicio donde los usuarios acceden a la aplicación según su rol 
(Administrador, Familiar, Personal de cuidado). Incluye campos de correo y contraseña, además de validaciones de acceso.</p>

<img src="../images/Login-NovaPeru-Tech.jpg" alt="Login Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Inicio de Sesión – NovaPeru Tech</h5>
<p>Formulario de acceso con credenciales de usuario. Presenta opciones de recuperación de contraseña y mantiene consistencia visual con la identidad de NovaPeru Tech.</p>

<img src="../images/Inicio-de-sesión-NovaPeru-Tech.jpg" alt="Inicio de Sesión Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Registrar Familiar – NovaPeru Tech</h5>
<p>Formulario para que los familiares creen una cuenta, ingresando datos personales básicos, correo electrónico y contraseña. Incluye validaciones de formato y confirmación de correo.</p>

<img src="../images/Registrar-Familiar-NovaPeru-Tech.jpg" alt="Registrar Familiar Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Registrar Administrador – NovaPeru Tech</h5>
<p>Pantalla destinada a registrar un nuevo administrador en la plataforma. Permite ingresar información personal, datos de contacto y credenciales de acceso.</p>

<img src="../images/Registrar-Administrador-NovaPeru-Tech.jpg" alt="Registrar Administrador Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Inventario – NovaPeru Tech</h5>
<p>Módulo donde el administrador puede visualizar el inventario de medicamentos y recursos clínicos. Permite filtrar, ordenar y consultar detalles de cada ítem.</p>

<img src="../images/Inventario-NovaPeru-Tech.jpg" alt="Inventario Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Inventario – Modificar – NovaPeru Tech</h5>
<p>Sección para editar la información de medicamentos en el inventario: nombre, cantidad, fecha de vencimiento, laboratorio y observaciones.</p>

<img src="../images/Inventario-Modificar-NovaPeru-Tech.jpg" alt="Inventario Modificar Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Paciente – NovaPeru Tech</h5>
<p>Pantalla que muestra la información general de un residente (datos personales, estado clínico, actividades recientes).</p>

<img src="../images/Paciente-NovaPeru-Tech.jpg" alt="Paciente Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Paciente – Agregar – NovaPeru Tech</h5>
<p>Formulario para registrar un nuevo residente en la institución. Incluye datos personales, médicos, contactos de emergencia y observaciones.</p>

<img src="../images/Paciente-Agregar-NovaPeru-Tech.jpg" alt="Paciente Agregar Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Paciente – Eliminar – NovaPeru Tech</h5>
<p>Módulo que permite al administrador eliminar registros de pacientes, con mensaje de confirmación para evitar acciones accidentales.</p>

<img src="../images/Paciente-Eliminar-NovaPeru-Tech.jpg" alt="Paciente Eliminar Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Empleado – NovaPeru Tech</h5>
<p>Pantalla donde se listan los empleados de la institución, mostrando nombre, rol, contacto y estado laboral.</p>

<img src="../images/Empleado-Card-Detalles-NovaPeru-Tech.jpg" alt="Empleado Card Detalles Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Empleado – Card Detalles – NovaPeru Tech</h5>
<p>Vista detallada de un empleado en formato de card, mostrando información personal, turno asignado, horas extra y contacto de emergencia.</p>

<img src="../images/Empleado-Card-Detalles-NovaPeru-Tech.jpg" alt="Empleado Card Detalles" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Actividad – Familiar – NovaPeru Tech</h5>
<p>Pantalla que muestra las actividades recientes del residente (ejercicios, visitas, terapias). 
El familiar puede visualizar fotos, descripciones y fechas.</p>

<img src="../images/Actividad-Familiar-NovaPeru-Tech.jpg" alt="Actividad Familiar Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

<h5>Historial de Pedido – NovaPeru Tech</h5>
<p>Pantalla que permite consultar pedidos realizados, con detalles de estado, fecha y productos solicitados.</p>

<img src="../images/Historial-de-Pedido-NovaPeru-Tech.jpg" alt="Historial de Pedido Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">

### Mock-ups Version Mobile
<p>En esta sección se muestran los mock-ups realizados para nuestro Web Application version Mobile.</p>

<img src="../images/Mobil1.png" alt="Login Mockup" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil2.png" alt="Inicio de Sesion" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil3.png" alt="Registrar Familiar" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil4.png" alt="Registrar Administrador" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil5.png" alt="Inicio" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil6-corregido.png" alt="Historial Actividades" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil7.png" alt="Historial Actividades 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil8.png" alt="Datos del Negocio" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil9.png" alt="Datos del Negocio 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil10.png" alt="Inventario" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil11.png" alt="Inventario 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil12.png" alt="Inventario 3" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil13.png" alt="Inventario 4" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil14-corregido.png" alt="Información inventario" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil15.png" alt="Actividades" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil16.png" alt="Actividades 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil17.png" alt="Actividdes 3" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil18.png" alt="Agregar Actividad" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil19-corregido.png" alt="Agregar Actividad 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil20.png" alt="Editar Actividad" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil21.png" alt="Editar Actividad 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil22.png" alt="Editar Actividad 3" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil23.png" alt="Residentes" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil24-corregido.png" alt="Residentes 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil25.png" alt="Agregar Datos del residente" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil26-corregido.png" alt="Agregar Datos del residente 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil27.png" alt="Modificar Datos del residente" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil28-corregido.png" alt="Modificar Datos del residente 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil29.png" alt="Agregar Historia " style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil30.png" alt="Empleados" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil31-corregido.png" alt="Empleados 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil32.png" alt="Modificar Datos del empleado" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil33-corregido.png" alt="Modificar Datos del empleado 2" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil34.png" alt="Agregar Datos del empleado" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil35-corregido.png" alt="Agregar Datos del empleado" style="width:auto; height:auto; border:2px solid #00bfff;">
<img src="../images/Mobil36.png" alt="Detalles del empleado" style="width:auto; height:auto; border:2px solid #00bfff;">

### 4.4.4. Web Applications User Flow Diagrams

## 4.5. Web Applications Prototyping


![ContextDiagram Diagram](../images/prototypy.png)
https://upcedupe-my.sharepoint.com/:v:/g/personal/u202312932_upc_edu_pe/ERvba6f0TWdDhgiVHVZ6HJwBgC_FOF0gNDEdsy9t47rPAA?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=Pc0kHx

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Design-Level Event Storming

Para identificar los eventos de dominio, es recomendable realizar una sesión de Event Storming. Esta técnica permite visualizar y comprender el flujo de eventos dentro del dominio, facilitando la identificación de los Bounded Context.

El desarrollo del proceso del Domain-Driven Design se realizó en la aplicación Miro: https://miro.com/app/board/uXjVJBlKaKg=/?share_link_id=383869260607


1. Bounded Context **IAM**
   
   <img src="../assets/img/chapter-V/iam-eventstorming.png" alt="Bounded Context IAM" style="width:auto; height:auto; border:2px solid #00bfff;">

   
2. Bounded Context **Inventories**
   
   <img src="../assets/img/chapter-V/inventory-eventstorming.png" alt="Bounded Context Inventories" style="width:auto; height:auto; border:2px solid #00bfff;">


3. Bounded Context **Employees**
   
   <img src="../assets/img/chapter-V/enployees-eventstorming.png" alt="Bounded Context Employees" style="width:auto; height:auto; border:2px solid #00bfff;">


4. Bounded Context **Nursing Home**
   
   <img src="../assets/img/chapter-V/nursinghome-eventstorming.png" alt="Bounded Context Nursing Home" style="width:auto; height:auto; border:2px solid #00bfff;">


5. Bounded Context **Residents**
   
   <img src="../assets/img/chapter-V/residents-eventstorming.png" alt="Bounded Context Residents" style="width:auto; height:auto; border:2px solid #00bfff;">


6. Bounded Context **Familiar**
   
   <img src="../assets/img/chapter-V/familiar-eventstorming.png" alt="Bounded Context Familiar" style="width:auto; height:auto; border:2px solid #00bfff;">


### 4.6.2. Software Architecture Context Diagram

El esquema de contexto ofrece una perspectiva general de las interacciones entre el sistema de software Veyra, los usuarios y sistemas externos.

![ContextDiagram Diagram](../images/contextDiagram.png)

### 4.6.3. Software Architecture Container Diagrams

El diagrama de contenedores ofrece una visión general de las conexiones entre aplicaciones y fuentes de datos en el sistema de Veyra. Muestra cómo interactúan y dependen entre sí para su funcionamiento.

![ContainerDiagram Diagram](../images/containerDiagram.png)

### 4.6.4. Software Architecture Components Diagrams

El diagrama de componentes proporciona una vista más detallada de la arquitectura del sistema Veyra. 
Este nivel de diseño se centra en los módulos internos de cada contenedor definido en el diagrama de contenedores, 
mostrando cómo se organizan, qué responsabilidades cumplen y cómo se comunican entre sí.

![ContainerDiagram Diagram](../images/Software-Architecture-Components-Diagrams.jpg)

## 4.7. Software Object-Oriented Design

### 4.7.1. Class Diagrams
<p>Employees diagram</p>

![Employees Diagram](../images/Employee.svg)


<p>Medications diagram </p>

![IAM Diagram](../images/platform-Medications.svg)

<p>IAM diagram</p>

![IAM Diagram](../images/platform-IAM.svg)

<p>Profiles diagram</p>

![profile Diagram](../images/platform-profiles.svg)

<p>Nursing home</p>

![profile Diagram](../images/NursingHome.svg)

## 4.8. Database Design

### 4.8.1. Database Diagrams

![Database](../images/VeyraDatabase.svg)


