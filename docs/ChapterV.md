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


A continuación, se describe la gestión del código fuente, también conocida por las siglas SCM (Source Code Management). Su función principal es rastrear los cambios que realizará el equipo durante el desarrollo de su proyecto en el repositorio de código fuente. Se utilizará como un sistema de control de versiones que lepermitirá realizar un seguimiento de los cambios realizados por miembros o desarrolladores individuales del proyecto. Además, es importante tener en cuenta que usaremos GitHub como nuestro sistema de control de versiones.

1. [ ] URL de la organización: NovaPeru Tech - https://github.com/NovaPeru-Tech

2. [ ] URL del repositorio de la Landing Page: NovaPeru-Tech-LandingPage - https://github.com/NovaPeru-Tech/NovaPeru-Tech-LandingPage

**GitFlow**

GitFlow es un modelo alternativo para la creación de ramas en Git que se ha convertido en una herramienta esencial para muchos desarrolladores en los últimos años. Este flujo de trabajo de control de versiones, desarrollado y popularizado por Vicent Driessen, desempeña un papel crucial en la gestión de las versiones de un código, facilitando la creación ordenada de nuevas características (Features) y correcciones de problemas urgentes (Hotfixes).

![GitFlow.png](/assets/img/chapter-V/GitFlow.png)

Como se mencionó previamente, GitFlow opera con ramas o "branches". A continuación, se detallan las ramas que se utilizarán en el flujo de trabajo de nuestro proyecto.

* **Main Branches:**
    * **Main:** Esta es la rama principal desde la cual se ramifican todas las demás. Contendrá la versión más reciente junto con las versiones anteriores creadas por los desarrolladores. Aquí se mantendrá el historial oficial de las versiones publicadas.
    * **Develop:** Esta rama puede ser creada a partir de la rama principal (Main) y contendrá todas las características (Features) estables. A través de esta rama, el equipo podrá integrar las funcionalidades de manera efectiva.

* **Support Branches**
  A diferencia de las ramas principales, estas ramas secundarias tienen una vida útil limitada, ya que se eliminan al fusionarse con sus ramas primarias.
    * **Feature:**
        * Se ramifica de: develop
        * Debe fusionarse de nuevo en: develop
        * Se utilizan para desarrollar las nuevas funciones que se integrarán en la próxima versión. Es importante destacar que esta rama existe únicamente mientras está en proceso de desarrollo. Sin embargo, una vez que el desarrollador haya completado esa función, se fusionará nuevamente con la rama "develop".

* **Convenciones para nombrar los Features:**
    * **Feture Branch:** feature/name
      **Example:**
        1. feature/welcome
        2. feature/about
        3. feture/myfeture
    * **Conventional Commits**
      El commit debe seguir la siguiente estructura:
      **\<type> [optional scope]: \<description>**
      **[optional body]**
      **[optional footer(s)]**
        * **Type:**
          **1\. feat:** Cuando se agrega un nuevo feature.
          **2\. fix:** cuando corriges un error.
          **3\. build:** cuando afectan los componentes de compilación como la herramienta de compilación, las dependencias o la version del proyecto.
          **4\. chore:** modificaciones privadas del código.
          **5\. docs:** commits que afectan solo a la documentación.
          **6\. refractor:** commits que reescriben o reestructura el código, pero no cambia el comportamiento.
          **7\. perf:** commits especiales que mejoran el rendimiento.
          **8\. style:** commits que no afectan el programa. (espacios en blanco, formato, puntos o comas faltantes).
          **9\. test:** commits que agregan pruebas.
        * **Scope**
          Ofrece información contextual adicional. Aunque es opcional, es beneficioso incluirlo para proporcionar a los desarrolladores una descripción más detallada del commit.
          **\<description>**
          Es una parte obligatoria del formato de los commits. Siempre debemos usar lenguaje en modo imperativo y evitar escribir en mayúsculas
          **[optional body]**
          El cuerpo es opcional y, cuando se utiliza, debe explicar la motivación detrás del cambio y contrastarlo con el comportamiento anterior. Es ideal para mencionar identificadores de problemas y sus relaciones.
          **[optional footer(s)]**
          Esta sección es opcional y puede incluir información sobre cambios significativos. Puede hacer referencia al problema por su identificación y, en esta sección, se incluyen los cambios importantes precedidos por "BREAKING CHANGES:" seguido de uno o dos saltos de línea.
          **Ejemplos:**
            1. feat(welcome): add welcome section
            2. build(release): bump version to 1.0.0
            3. style: remove empty line
            4. feat(sign up): add the button to sign up
            5. feat!: email the costumer when product is shipped
            6. feat: remove ticket list endpoint
               refers to JIRA-1337
               BREAKING CHANGES: ticket enpoints no longer supports list all entites.

Como se mencionó previamente, la gestión de nuestro código fuente se llevará a cabo mediante
GitHub. El IDE utilizado en este caso, WebStorm, debe estar vinculado directamente al
repositorio creado por nuestra empresa MetaSoft. De esta manera, cada commit realizado por
un miembro del equipo se subirá automáticamente y se cargará en el GitHub de la organización. Las instrucciones para completar con éxito este proceso de emparejamiento se detallan a continuación:

* **Activar el controlador de versiones del IDE**
  Dado que utilizaremos GitHub para gestionar nuestro código, la opción que debe estar
  habilitada o seleccionada es aquella que indique que el sistema de control se realizará
  mediante Git. Para hacer esto, siga los siguientes pasos:

    1. Diríjase a la pestaña "VCS" en WebStorm.
    2. Luego, seleccione la opción "Enable Version Control Integration".


![activar-el-controlador-de-versiones-1.png](/assets/img/chapter-V/activar-el-controlador-de-versiones-1.png)

Ahora se debe seleccionar el sistema de control a través de Git y, por último aceptar los cambios.

![activar-el-controlador-de-versiones-2.png](/assets/img/chapter-V/activar-el-controlador-de-versiones-2.png)

* **Aregar una cuenta de GitHub, siga estos pasos:**
    1. Diríjase a la sección de configuración en su aplicación.
    2. Dentro de la pestaña 'File', busque y seleccione la opción 'Settings'.
    3. En la configuración, busque la sección de version control.
    4. Agregue su cuenta de GitHub para obtener acceso a los repositorios.

![aregar-una-cuenta-de-GitHub-2.png](/assets/img/chapter-V/aregar-una-cuenta-de-GitHub-2.png)

* **Configurar el nombre de usuario de Git:** Una vez que hayas establecido el sistema de control de versiones que se vinculará con tu IDE, deberás ingresar la cuenta que utilizarás. Para hacerlo, sigue estos pasos:
    1. Realiza un commit en tu proyecto. Durante este proceso, se te solicitará que ingreses tu nombre de usuario de Git.
    2. Después de haberlo añadido, todos los cambios se guardarán en el repositorio especificado en esa plataforma, siempre y cuando des la orden correspondiente.
    3. Para configurar tu nombre de usuario de Git, primero selecciona la opción 'commit' que se encuentra dentro de la pestaña 'Git'.


* **Guardar el progreso en GitHub:** Con todo configurado en WebStorm, ahora puedes subir tu código a GitHub sin problemas. Simplemente dirígete a la opción 'GitHub' que se encuentra en la pestaña 'Git' y comparte el proyecto.


* **Configurar la propiedad del repositorio en GitHub:** Ahora, solo necesitas configurar la ubicación del repositorio. El código ya debería estar guardado en GitHub, pero solo estará presente en tu propia cuenta. Para cambiar la propiedad y transferirla a la organización deseada, sigue estos pasos:
    1. Ingresa al repositorio creado en GitHub.
    2. Selecciona la pestaña 'settings'
    3. Dirigite al apartado de 'DangerZone'
    4. Luego da click en 'transfer'
    5. Finalmente elegimos el nuevo lugar para guardar el repositorio.


* **Configurar control remoto en Git:** Por último, dado que el repositorio ahora está bajo la propiedad de la empresa y depende de ella, es necesario acceder al control remoto del código. Para hacerlo, simplemente ingresa al repositorio creado y copia la URL del repositorio.

Ahora, en el IDE, dirígete a la pestaña 'Git' y elige la opción 'Manage Remotes'.

Finalmente, como último paso, debes pegar el enlace copiado en el campo de dirección que solicita el IDE para el control remoto en Git.

Si has seguido correctamente todos los pasos y directrices mencionados, entonces has completado la configuración con éxito. Ahora, solo necesitas realizar un commit y los cambios que hayas efectuado se guardarán en el repositorio de GitHub, ya sea que hayas realizado modificaciones en el código, creado nuevas ramas u otras acciones.

### 5.1.3. Source Code Style Guide & Conventions.

En esta sección, se presentarán las pautas, convenciones, estilos y principios que se aplicarán a cada uno de los lenguajes utilizados en la creación de nuestra aplicación. La observancia de este conjunto de directrices reviste una importancia fundamental, ya que tiene el propósito de mantener la calidad estructural del software, mejorar la legibilidad del código fuente y simplificar el mantenimiento del mismo.

Dado que en este proyecto se emplearán varios lenguajes, como HTML, CSS, JavaScript, C# y TypeScript para el desarrollo de la plataforma web, así como Gherkin para el proceso de pruebas del programa, a continuación, se detallarán y describirán las reglas y recomendaciones generales que se tendrán en cuenta al utilizarlos.


**Nomenclatura General**

Para los nombres de variables, objetos, elementos y funciones que se utilicen en el proyecto, se emplearán términos en inglés que estén relacionados con lo que representan. No se utilizarán mayúsculas en estos nombres, ya que, de acuerdo con W3Schools (sin fecha), la combinación de mayúsculas y minúsculas puede dificultar la legibilidad del código. En su lugar, se optará por utilizar exclusivamente letras minúsculas, lo que contribuirá a una mayor claridad en el código.

Ejemplos de nomenclatura estándar, siguiendo las recomendaciones de Google (s.f.):

```
.gallery {}
.video {}
.login {}
```

Estas pautas de nomenclatura ayudarán a mantener una coherencia en el código y facilitarán su comprensión.

**Sangría**

Cuando se trabaje con HTML, CSS y/o JavaScript, se aplicará un espaciado de dos espacios antes de cada línea que se encuentre dentro de un bloque. Según W3Schools (sin fecha), no se recomienda el uso de la tecla "Tabulación". A continuación, se muestra un ejemplo de la sangría estándar en HTML siguiendo las directrices de W3Schools (s.f.):

``` html
<!DOCTYPE html>
<html>
  <head>
    <title>Título del Documento</title>
  </head>
  <body>
    <h1>Encabezado Principal</h1>
    <p>Este es un párrafo dentro del cuerpo del documento.</p>
  </body>
</html>
```

Este estilo de sangría proporciona una estructura clara y organizada al código, lo que facilita su lectura y mantenimiento.

Ejemplo de formato estándar de sangría en CSS, conforme a las recomendaciones de W3Schools (s.f):

``` CSS
html {
  background: #fff; /* Fondo blanco */
  color: #404;     /* Color de texto gris */
}
```

Ejemplo de nomenclatura estándar de la sangría en JavaScript según W3School (s.f.):

``` JavaScript
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```

**Especificaciones generales**

A continuación, detallaremos las reglas específicas necesarias para comprender el código de nuestra aplicación en cada lenguaje.

**HTML:**

HTML, acrónimo de HyperText Markup Language en inglés, es un lenguaje de marcado que se utiliza para definir la estructura de una página web. También incluye funcionalidades que permiten controlar el comportamiento de diferentes elementos del contenido de la página, como cambiar el tamaño del texto o aplicar formato cursiva, entre otros. En nuestro proyecto, emplearemos HTML5, y a continuación, se presentan las características y directrices que debemos seguir para utilizar este lenguaje de la siguiente manera:

* **Declare Document Type**
  La declaración del tipo de documento debe realizarse en la primera línea del código. Según las recomendaciones de Google (s.f.), se prefiere la sintaxis de HTML5 para todos los documentos HTML. Para declararla, simplemente copia lo siguiente:

``` html
<!DOCTYPE html>
```

* **Blank Lines**
  Cada vez que comiences un nuevo bloque, lista o tabla de gran longitud, es recomendable dejar una línea en blanco después del elemento anterior para mejorar la legibilidad y la presentación del código, de acuerdo con las pautas de W3Schools (s.f.):

``` html
<!DOCTYPE html>
<html>
<head>
<title>Animales Exóticos</title>
</head>
<body>
<h1>Lemur de Madagascar</h1>
<p>El lémur de Madagascar es un primate endémico de la isla de Madagascar en el Océano Índico.</p>

<h1>Pangolín</h1>
<p>El pangolín es un mamífero cubierto de escamas que se encuentra en regiones de África y Asia.</p>

<h1>Ocelote</h1>
<p>El ocelote es un felino salvaje que habita en América del Sur y Central, conocido por su pelaje moteado.</p>
</body>
</html>
```

Esta práctica de dejar una línea en blanco mejora la estructura y legibilidad del código HTML.

* **Quote attribute Values**
  Para los valores de los atributos, es común utilizar comillas dobles alrededor de ellos, aunque esta característica no sea obligatoria. Según W3Schools (sin fecha), esto mejora la legibilidad del código y es una práctica común entre los desarrolladores. Aquí tienes un ejemplo:

``` html
<table class="striped">
```

Este enfoque de usar comillas dobles alrededor de los valores de los atributos es ampliamente aceptado y recomendado en la comunidad de desarrollo web.

* **Never Skip the \<title> Element**
  El elemento `<title>` permite que las páginas aparezcan en la lista de resultados al realizar búsquedas en un navegador web. Además, este elemento es responsable de proporcionar el nombre de la página cuando se agrega a marcadores o favoritos. A continuación, se muestra un ejemplo de su uso:

``` html
<title>Guía de Estilo HTML y Convenciones de Codificación</title>
```

Este elemento es esencial para mejorar la identificación y accesibilidad de una página web.

* **HTML Line-Wrapping**
  A pesar de que en un documento HTML no exista un límite estricto en la cantidad de palabras por línea, no se recomienda generar líneas de código excesivamente largas. De hecho, hacerlo dificulta la legibilidad del código. Para continuar en la siguiente línea, se deben utilizar al menos cuatro espacios para distinguir elementos secundarios. Aquí tienes un ejemplo basado en las recomendaciones de Google (sin fecha):

``` html
<button mat-icon-button color='primary' class="menu-button"
(click)="openMenu()">
<mat-icon>menu</mat-icon>
</button>
```

Este estilo de formateo ayuda a mantener un código más legible y facilita la identificación de los elementos y su jerarquía en la estructura del documento HTML.

**CSS:**

CSS, conocido por sus siglas en inglés, Cascading Style Sheets (Hojas de Estilo en Cascada), es un lenguaje que se enfoca en definir y mejorar la presentación de un documento basado en HTML. A continuación, se presentan las directrices que debemos seguir al utilizar CSS:

* **Shorthand Properties**
  Se recomienda utilizar abreviaturas de propiedades y declarar los campos de los elementos en la menor cantidad de líneas posible, según las pautas de Google (sin fecha). Esto aumenta la eficiencia del código y lo hace más legible. Además, se debe evitar agregar unidades después del valor cero. Aquí tienes un ejemplo:

``` css
border-top: 0;
font: 100%/1.6 palatino, georgia, serif;
padding: 0 1em 0;
```

Siguiendo estas recomendaciones, se puede lograr un código CSS más conciso y fácil de entender.

* **Declaration Stops**
  Es importante incluir un punto y coma al final de cada declaración en CSS, al igual que en la mayoría de los lenguajes de programación. Siguiendo las pautas de Google (sin fecha), esta práctica contribuye a mantener la coherencia en el código. A continuación, se muestra un ejemplo:

``` css
html {
  background: #fff;
  color: #404;
}
```

El uso consistente de puntos y comas al final de las declaraciones CSS ayuda a prevenir errores y mejora la claridad del código.

* **Property Name Stops**
  Es necesario incluir un espacio entre los dos puntos que siguen al nombre de una propiedad y el valor correspondiente. Siempre se debe colocar un solo espacio después de los dos puntos, pero no antes. A continuación, se muestra un ejemplo siguiendo esta convención estándar de Google (s.f):

``` css
html {
  background: #fff;
  color: #404;
}
```

Mantener esta consistencia en la colocación de espacios ayuda a que el código CSS sea más legible y fácil de entender.

* **Declaration Block Separation**
  Es esencial utilizar un espacio separador después del nombre de un selector de elemento y antes de la llave que inicia un bloque de declaración CSS. Además, la llave de apertura del bloque debe estar en la misma línea que el selector. Aquí tienes un ejemplo siguiendo esta convención estándar de Google (sin fecha):

``` css
html {
  background: #fff;
  color: #404;
}
```

El cumplimiento de estas directrices ayuda a mantener la consistencia y la legibilidad en el código CSS.

* **CSS quotation Marks**
  No se deben utilizar comillas dobles (`"`) en el código CSS; en su lugar, se permiten y deben emplearse comillas simples (`'`) únicamente para selectores de atributos y valores de propiedades.
  Ejemplo conforme a las pautas estándar de Google (sin fecha):

``` css
html {
  font-family: 'open sans', arial, sans-serif;
}
```

Este ejemplo demuestra el uso de comillas simples para encerrar el valor del atributo `font-family` en CSS, lo cual es una práctica común y aceptada.

**JavaScript**

JavaScript es un lenguaje de programación que permite especificar de manera precisa las acciones que debe realizar el navegador web, incluyendo el orden de ejecución de tareas y la frecuencia con la que se deben llevar a cabo. A continuación, se presentan las pautas para el uso de JavaScript en nuestro proyecto:

* **Spaces around operators**
  Es importante añadir espacios alrededor de cada operador matemático y comas que se utilicen en el código JavaScript. A continuación, se muestra un ejemplo siguiendo la convención estándar de W3Schools (sin fecha):

``` javascript
let x = y + z;
const myArray = ['Volvo', 'Saab', 'Fiat'];
```

El uso consistente de espacios alrededor de operadores y comas mejora la legibilidad del código JavaScript.

* **Simple Statement's End**
  Es fundamental que una instrucción simple finalice con un punto y coma, tal como es el caso en muchos otros lenguajes de programación. A continuación, se muestra un ejemplo que cumple con la convención estándar de W3Schools (sin fecha):

``` javascript
let x = v + 7;
const myArray = ['Volvo', 'Saab', 'Fiat'];
```

El uso de punto y coma al final de cada instrucción ayuda a garantizar la estructura correcta del código JavaScript y a evitar posibles errores.

* **Beginning and End of Function**
  Un bloque de función debe incluir una llave al final de la primera línea, de modo que el cierre de la función esté en la última línea, sin necesidad de un punto y coma. Este mismo principio se aplica a las estructuras condicionales y los bucles. A continuación, se muestra un ejemplo que cumple con la convención estándar de W3Schools (sin fecha):

``` javascript
function toCelsius(fahrenheit) {
  return (5 / 9) * (fahrenheit - 32);
}
```

En este ejemplo, la función `toCelsius` está formateada de acuerdo con estas pautas, con la llave de apertura en la misma línea que la declaración de la función y la llave de cierre en la última línea. Esto ayuda a mantener la estructura y la legibilidad del código JavaScript.

* **Object Rules**
  Para la creación de un objeto, al igual que en una función, se comienza con una llave al final de la primera línea. Sin embargo, en este caso, la llave de cierre debe ir seguida de un punto y coma. Para definir las propiedades del objeto, se utilizan dos puntos y un espacio para separar el nombre de la propiedad de su valor. Si el valor es un string, se debe encerrar entre comillas dobles. A continuación, se muestra un ejemplo siguiendo la convención estándar de W3Schools (sin fecha):

``` javascript
const person = {
  firstName: "John",
  lastName: "Doe",
  age: 50,
  eyeColor: "blue"
};
```

En este ejemplo, el objeto `person` está formateado de acuerdo con estas pautas, lo que mejora la legibilidad y la estructura del código JavaScript.

**Gherking:**

Gherkin es un Lenguaje Específico de Dominio (DSL por sus siglas en inglés) que se utiliza para resolver problemas específicos mediante la generación de casos de prueba que validan una característica en diversos escenarios. Gherkin incluye varios elementos, entre los cuales los más conocidos y utilizados son Feature, Scenario, Example, Given, When y Then. A continuación, se presentan las pautas que debemos seguir al utilizar Gherkin en nuestro código:

* **Discernible Given-When-Then Blocks**
  Es importante aplicar sangría a los elementos que representan los pasos a seguir en un escenario. En el caso de "And", se debe aplicar una sangría adicional. Siguiendo la recomendación de Keiblinger (2021), este enfoque ayuda a identificar rápidamente las partes que componen un escenario. A continuación, se muestra un ejemplo:

``` gherkin
Scenario: Ingreso de requisitos con claridad
  Given que en el formulario de ingreso de oferta laboral
  When escribo claramente los requisitos
  Then se mostrará el mensaje
  And mi oferta solo aparecerá a quienes cumplan con estos
  And se habilita la opción
```

En este ejemplo, se ha aplicado la sangría de manera adecuada para resaltar los pasos del escenario, y se ha utilizado una sangría adicional para los pasos que comienzan con "And". Esto mejora la legibilidad y la comprensión de los escenarios escritos en Gherkin.

* **Step with Tables**
  Conforme a la recomendación de Keiblinger (2021), cuando sea necesario introducir valores en partes del escenario, se debe emplear una tabla o crear un formulario que refleje esa parte del escenario. Antes de esta representación, se deben colocar dos puntos. Aquí tienes un ejemplo:

``` gherkin
Then se mostrará el mensaje:
  | Mensaje |
  | Se completaron los requisitos adecuadamente |
```

Este enfoque permite una representación clara y estructurada de los valores relacionados con una parte específica del escenario.

* **Reducing Noise**
  Para evitar la acumulación de demasiadas líneas de código en un escenario, es recomendable incluir valores por defecto dentro de los pasos para campos que no sean muy relevantes para ese escenario en particular. Los valores "estándar" que se coloquen deben estar entre comillas simples. Siguiendo el consejo de Keiblinger (2021), esta práctica contribuye significativamente a la reducción del tamaño del código. A continuación, se muestra un ejemplo:

``` gherkin
When escribo claramente los requisitos 'dominio en C'
```

En este ejemplo, se ha incluido un valor por defecto ('dominio en C') entre comillas simples dentro del paso para representar un campo que no es esencial en ese escenario. Esto ayuda a mantener el escenario más conciso y legible.

* **Scenarios Separator**
  Para separar dos escenarios, se debe insertar un salto de línea y, según la sugerencia de Keiblinger (2021), si es posible, agregar una línea de comentario para facilitar la visualización de estos. De esta manera, se identifica rápidamente el inicio y el fin de un escenario. A continuación, se presenta un ejemplo:

``` gherkin
Scenario: Ingreso de requisitos con claridad
Given que en el formulario de ingreso de oferta laboral
When escribo claramente los requisitos
Then se mostrará el mensaje
And mi oferta solo aparecerá a quienes cumplan con estos
And se habilita la opción

# --------------------------

Scenario: Otro escenario
Given que en otro contexto
When ocurre algo diferente
Then se muestra otro resultado
```

En este ejemplo, se ha agregado un salto de línea entre los dos escenarios y se ha incluido una línea de comentario como separador para mejorar la visualización y la identificación de cada escenario.

**C#:**

C# es un lenguaje de programación desarrollado por Microsoft en el año 2000 como parte de su plataforma .NET. Desde su creación, C# ha evolucionado significativamente, convirtiéndose en una herramienta esencial para el desarrollo de una amplia gama de aplicaciones, desde software de escritorio hasta aplicaciones web y móviles, así como servicios en la nube. Su diseño moderno y su integración con el ecosistema de .NET lo han consolidado como una opción preferida para muchos desarrolladores a nivel global.

A continuación, se presentan las pautas para utilizar C# en nuestro proyecto:

* **Datos de cadena**


Use **interpolación de cadenas** para concatenar cadenas cortas, como se muestra en el código siguiente.

```C#  
  string displayName = $"{nameList[n].LastName}, {nameList[n].FirstName}";
```

Para anexar cadenas en bucles, especialmente cuando se trabaja con grandes cantidades de texto, utilice un objeto System.Text.StringBuilder.
En este ejemplo, se han seguido las pautas para nombrar clases e interfaces de manera clara y legible.


```C#  
  var phrase = "lalalalalalalalalalalalalalalalalalalalalalalalalalalalalala";
  var manyPhrases = new StringBuilder();
  for (var i = 0; i < 10000; i++)
  {
      manyPhrases.Append(phrase);
  }
  //Console.WriteLine("tra" + manyPhrases);
```

* **Delegados**

Use **Func<> y Action<>** en lugar de definir tipos de delegado. En una clase, defina el método delegado.

```C#  
  Action<string> actionExample1 = x => Console.WriteLine($"x is: {x}");
  
  Action<string, string> actionExample2 = (x, y) => Console.WriteLine($"x is: {x}, y is {y}");
  
  Func<string, int> funcExample1 = x => Convert.ToInt32(x);
  
  Func<int, int, int> funcExample2 = (x, y) => x + y;
```

Llame al método con la signatura definida por el delegado Func<> o Action<>.

```C#  
  actionExample1("string for x");
  actionExample2("string for x", "string for y");
  Console.WriteLine($"The value is {funcExample1("1")}");
  Console.WriteLine($"The sum is {funcExample2(1, 2)}");
```

* **try-catch y using en el control de excepciones**

Use **try-catch** para controlar las excepciones. Use **using** para liberar recursos no administrados.

``` C#  
  try
  {
      // Code that may throw an exception
  }
  catch (Exception ex)
  {
      // Code to handle the exception
  }
  
  using (var resource = new Resource())
  {
      // Code that uses the resource
  }
```

* **Operadores && y ||**

Use **&&** y **||** en lugar de **&** y **|** para operaciones lógicas. Los operadores **&&** y **||** realizan una evaluación de cortocircuito, lo que significa que si la primera parte de la expresión es suficiente para determinar el resultado, la segunda parte no se evalúa.

```C#  
  if (a == 10 && b == 20)
  {
      // Code to execute if both conditions are true
  }
  
  if (a == 10 || b == 20)
  {
      // Code to execute if either condition is true
  }
```

* **Comentarios**

Use comentarios para explicar el código y proporcionar información adicional. Los comentarios deben ser claros y concisos.

```C#  
  // This is a single-line comment
  
  /*
  This is a multi-line comment
  that spans multiple lines
  */
```
* **Operador new**

Use **new** para crear instancias de clases y estructuras.

```C#  
  var person = new Person();
  var point = new Point(10, 20);
```

* **Control de eventos**

Use **eventos** para notificar a los suscriptores cuando ocurre un evento.

```C#  
  public class Button
  {
      public event EventHandler Click;
  
      protected virtual void OnClick(EventArgs e)
      {
          Click?.Invoke(this, e);
      }
  }
```

* **Consultas LINQ**

Use consultas LINQ para realizar operaciones de consulta en colecciones de datos.

```C#  
  var query = from c in customers
              where c.City == "London"
              select c;
```

* **Variables locales con asignación implícita de tipos**

Use la asignación implícita de tipos para las variables locales cuando el tipo se puede inferir fácilmente.

```C#  
  var name = "John";
  var age = 30;
```

**Typescript**

JavaScript es uno de los lenguajes más populares y ha experimentado un rápido avance y mejora en los últimos años. A continuación, se presentan las pautas para utilizar JavaScript en nuestro proyecto:

En TypeScript, se recomienda que las variables se declaren en minúsculas y se especifique el tipo de dato utilizando dos puntos después del nombre de la variable. Aquí tienes ejemplos de cómo declarar y asignar valores a variables en TypeScript:

``` typescript
// Definición e inicialización separadas
let edad: number;
edad = 20;

// Definición e inicialización en la misma línea.
let edadAitor: number = 18;
```

Además, en TypeScript, se siguen las mismas convenciones que se utilizan en JavaScript.

### 5.1.4. Software Deployment Configuration.


Para desplegar la Landing Page desde GitHubPages hay que seguir los siguientes pasos:

**1. Ubicar el repositorio que tiene guardado el codigo fuente y dirigirse al apartado de configuración (settings):**

![repo-landing-page.png](/assets/img/chapter-V/repo-landing-page.png)


**1. Seleccionar la sección pages:**


![pages-landing-page.png](/assets/img/chapter-V/pages-landing-page.png)


**1. Configurar la rama que será usada para hacer deploy:**

![rama-landing-page.png](/assets/img/chapter-V/rama-landing-page.png)


## 5.2. Landing Page, Services & Applications Implementation.


### 5.2.1. Sprint 1

En la fase inicial de nuestro proyecto, nos propusimos llevar a cabo la implementación del diseño de nuestra Landing Page utilizando WebStorm como entorno de desarrollo. Esto implica que al concluir el Sprint, todas las secciones, ya sea Home, Services, Pricing, Testimonials o About Us, deben estar completadas. A continuación, adjuntamos imágenes que ilustran cómo gestionamos las tareas en Jira Software.

Repositorio: [https://github.com/NovaPeru-Tech/NovaPeru-Tech-LandingPage](https://github.com/NovaPeru-Tech/NovaPeru-Tech-LandingPage)

Landing Page Deployed: https://novaperu-tech.github.io/NovaPeru-Tech-NovaPeru-Tech-LandingPage/

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
