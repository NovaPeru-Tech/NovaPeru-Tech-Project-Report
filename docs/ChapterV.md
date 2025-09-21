# Capítulo V: Product Implementation, Validation & Deployment

### 5.1. Software Configuration Management.

En este punto del informe se describe las decisiones y los principios que ayudarán al
equipo a garantizar la coherencia durante el desarrollo de la solución.

### 5.1.1. Software Development Environment Configuration.

En este apartado se proporcionan los enlaces a las aplicaciones y productos de
software creados durante el ciclo del proyecto utilizando los programas correspondientes.

Con ese fin, se organizará en las siguientes secciones:
1. [ ] Project Management
2. [ ] Requirements Management
3. [ ] Product UX/UI Design
4. [ ] Software Development
5. [ ] Software Testing
6. [ ] Software Documentation

Asimismo, se clasificarán los elementos de estas secciones como rutas de referencia
(para software basado en modelos Saas) o rutas de descarga (para productos que se
ejecuten en las computadoras de los miembros del equipo) para cada uno de los productos
de software.

**Project Management**

Esta disciplina se fundamenta en la administración de proyectos y busca principalmente la
mejora de procesos y su entorno con el propósito de lograr los resultados esperados.

* Durante el ciclo digital del proyecto, se llevará a cabo la implementación de un producto
  de software basado en el modelo SaaS, el cual funcionará a través de un navegador web; no
  obstante, no se desarrollará una versión de la aplicación móvil correspondiente.

**Requirements Management:**

Este proceso se enfoca en asegurar que una organización documente, verifique y satisfaga las
necesidades y expectativas de sus clientes, así como las de las partes interesadas internas
o externas.


* **Trello:** Trello es una plataforma digital de gestión de proyectos basada en tableros,
* listas y tarjetas, que permite organizar tareas, colaborar en equipo y supervisar el progreso
* de manera visual y eficiente.

**Product UX/UI Design**

Esta herramienta facilita la creación digital de modelos que se integran en la vida del consumidor.
En este caso, estamos desarrollando un modelo de sitio web compatible tanto con computadoras como
con dispositivos móviles.

Para lograrlo, utilizamos varias herramientas de diseño y colaboración, que incluyen:

1. **Uxpressia:** Uxpressia es una plataforma en línea especializada en el mapeo de la trayectoria del
   cliente. Nos ayuda a crear mapas de impacto y perfiles de usuario, como User Personas, Empathy Maps
   y Journey Maps. Puedes encontrar más información sobre Uxpressia en este [enlace](https://uxpressia.com/).

2. **MIRO:** MIRO es una pizarra digital colaborativa en línea que se adapta a diversas actividades
   colaborativas, como investigación, ideación, creación de lluvias de ideas y mapas mentales. Es una
   herramienta versátil que facilita el trabajo en equipo. Descubre más sobre MIRO en su
   [sitio web](https://miro.com/es/).

3. **Figma:** Figma es una herramienta de prototipado web y un editor de gráficos vectoriales. A
   diferencia de otras herramientas, Figma se ejecuta en línea, lo que permite crear modelos que
   funcionan tanto en navegadores web como en navegadores móviles. Puedes explorar
   Figma en [este enlace](https://www.figma.com/es-es/).

4. **Lucid Chart:** Esta es una aplicación de diagramación en línea que permite a los usuarios colaborar y
   trabajar juntos en tiempo real para crear una variedad de diseños, incluidos diagramas UML, mapas
   mentales, prototipos de software y otros tipos de diagramas. Puedes conocer más acerca de Lucid Chart
   en [este enlace](https://www.lucidchart.com/pages/es).

5. **Overflow:** Overflow es una herramienta de diagramación que ofrece la posibilidad de colaborar en
   tiempo real. Utilizamos esta herramienta para crear diagramas de Userflows. Si deseas obtener más
   información sobre Overflow, visita su [sitio web](https://overflow.io/).

Estas herramientas nos ayudan a dar vida a nuestros diseños digitales y a garantizar que nuestros
productos sean accesibles y atractivos en diferentes plataformas.


**Software Development:**

El desarrollo de software es una metodología aplicada en la creación de productos de software. Esta
metodología se utiliza para establecer un proceso que guía el desarrollo del software, y cada uno de
sus pasos describe un enfoque específico para las distintas actividades que ocurren durante el proceso.

Aquí te presentamos algunas herramientas y tecnologías clave que utilizaremos en el proyecto:

1. **GitHub:** GitHub es una plataforma de repositorio comunitario que se utiliza para almacenar y
   gestionar los avances de proyectos realizados por grupos de personas. Puedes acceder al repositorio
   del proyecto en este [enlace](https://github.com/SV51-MetaSoft-App-Web).

2. **Webstorm:** Webstorm es un entorno de desarrollo de JetBrains, una empresa especializada en software,
   orientado al desarrollo web en JavaScript. Esta herramienta proporciona facilidades para probar
   sitios web en navegadores como Google Chrome. En nuestro proyecto, utilizaremos webstorm para
   trabajar con lenguajes como HTML, CSS y JavaScript. Obtén más información sobre WebStorm [aquí](https://www.jetbrains.com/webstorm/).

3. **HTML:** HTML es un lenguaje de marcado que se utiliza en el desarrollo de sitios web para crear
   hipertextos y enlazar a otros documentos. Este lenguaje proporciona herramientas para diseñar
   sitios web y se puede combinar eficazmente con CSS y JavaScript. En nuestro proyecto, utilizaremos
   HTML para implementar la documentación de la página web. Obtén más información sobre la edición de
   archivos HTML en WebStorm [aquí](https://www.jetbrains.com/help/idea/editing-html-files.html).

4. **CSS:** CSS es un lenguaje de diseño destinado al entorno web, que posibilita la mejora de la interfaz
   de usuario previamente diseñada al añadir elementos como colores y tamaños, entre otros. Además,
   es posible crear un estilo en CSS y compartirlo en el sitio web creado en HTML. Este lenguaje será
   empleado en la implementación del diseño de nuestra plataforma web. Puedes obtener más información
   sobre CSS en [enlace](https://www.jetbrains.com/help/idea/style-sheets.html).

5. **JavaScript:** Es un lenguaje de programación que es interpretado por otros programas. Funciona bajo
   el paradigma de programación orientada a objetos (POO), utilizando prototipos en lugar de clases
   para la implementación. Este lenguaje permite crear dinámicas para los usuarios a través de la
   lógica de programación y será utilizado en la creación de las interacciones dinámicas en la plataforma
   web. Puedes encontrar más detalles sobre JavaScript en [enlace](https://www.jetbrains.com/help/idea/style-sheets.html).

Estas herramientas y tecnologías desempeñarán un papel fundamental en la creación exitosa de nuestro
producto de software.

**Software Testing:**

Se trata de la acción de evaluar los elementos y el funcionamiento del software sometido a prueba
mediante procesos de validación y verificación.

**Lenguaje Gherkin:** Este lenguaje, conocido como DSL (Lenguaje Específico de Dominio), está diseñado
específicamente para abordar problemas particulares. Además de poder ser interpretado en código,
permite agregar historias de usuario del programa junto con sus componentes correspondientes, como
Característica, Escenario, Ejemplo, Esquema de Escenario, Dado, Cuando, Entonces y Y.

**Software Documentation**

Se refiere a textos escritos o ilustraciones que acompañan al software de computadora o están
integrados en su código fuente. Esta documentación tiene como objetivo explicar cómo funciona el
software o cómo utilizarlo.

### 5.1.2. Source Code Management.


### 5.1.3. Source Code Style Guide & Conventions.


### 5.1.4. Software Deployment Configuration.


## 5.2. Landing Page, Services & Applications Implementation.


### 5.2.1. Sprint n


#### 5.2.1.1. Sprint Planning n.


##### 5.2.1.2. Sprint Backlog n.


##### 5.2.1.3. Development Evidence for Sprint Review.


##### 5.2.1.4. Testing Suite Evidence for Sprint Review.


##### 5.2.1.5. Execution Evidence for Sprint Review.


##### 5.2.1.6. Services Documentation Evidence for Sprint Review.


##### 5.2.1.7. Software Deployment Evidence for Sprint Review.


##### 5.2.1.8. Team Collaboration Insights during Sprint.


### Conclusiones
Veyra representa una solución integral para la gestión eficiente del cuidado de pacientes, centralizando funcionalidades clave como el registro de datos de salud, la comunicación entre la familia y los cuidadores, y la administración de planes de cuidado personalizados.

La implementación de tecnologías modernas permite que el sistema sea escalable, modular y adaptable a las necesidades de diversas situaciones de cuidado, garantizando su efectividad para diferentes tipos de pacientes y organizaciones.

El sistema Veyra reduce la carga operativa manual y mejora la toma de decisiones al automatizar procesos clave como el envío de notificaciones de medicamentos y la visualización de métricas de salud en tiempo real.

La cobertura de pruebas (unitarias e integradas) podría ampliarse, sobre todo en módulos críticos como la activación de alertas de emergencia y la sincronización de datos de dispositivos de salud, para garantizar una mayor confiabilidad del sistema ante cambios.

---

### Bibliografía
- Refactoring.Guru. (s.f.). *Design patterns*. [https://refactoring.guru/es/design-patterns](https://refactoring.guru/es/design-patterns)
- Gothelf, J., & Seiden, J. (2021). *Lean UX: Designing great products with agile teams* (3rd ed.). O’Reilly Media.
- Evans, E. (2004). *Domain-driven design: Tackling complexity in the heart of software*. Addison-Wesley.
- Vernon, V. (s.f.). *Domain-driven design reference: Definitions and pattern summaries*. [https://domainlanguage.com/ddd/reference/](https://domainlanguage.com/ddd/reference/)
- Martin, R. C. (2017). *Clean architecture: A craftsman's guide to software structure and design*. Prentice Hall.

---

### Anexos
- **Deploy Landing Page:** [Ver Landing Page](....)
- **Entrevistas:** [Ver Entrevistas]()
- **Diagrama C4:** [Ver Diagrama C4]()
- **Diagrama de clases del frontend:** [Ver Diagrama del Frontend]()
- **Diagrama de clases del bounded context IAM:** [Ver Diagrama del IAM]()
- **Diagrama de clases del bounded context Personnel:** [Ver Diagrama del Personnel](...)
- **Diagrama de clases del bounded context FleetManagment:** [Ver Diagrama del FleetManagment](...)
- **Diagrama de clases de la base de datos:** [Ver Diagrama de la base de datos]()  
