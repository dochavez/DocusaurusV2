# Docusaurus Versión 2
## Instalación y Configuracion para **Principiantes** paso a paso 🚀 <br>
Elaborado por: **Danny Chávez** <br>
DEVELOPER CIRCLE COMMUNITY CHALLENGE 2020

Documentar es una forma de dejar en evidencia lo que se hace para que otras personas puedan aprender, modificar, crear, diseñar y compartir. Aunque es importante mencionar que documentar puede ser una tarea complicada. Lo cual puede desencadenar que un proyecto alcance su máximo potencial. Pero gracias a Docusaurus nuestra tarea puede verse muy simplificada.
Con Docusaurus nos ayuda a crear y mantener sitios web donde podemos mostrar nuestra documentación. Gracias a la implementación de React.js, podemos contar con soporte para blogs, paginas con diseños personalizados con estilos muy elegantes y dinámicos. 


*  ## Verificación para preparar el entorno. 📋

•	Verifica que tienes instalado en tu computadora <a href="https://nodejs.org/es/" target="_blank">**Node.js**</a>, <a href="https://classic.yarnpkg.com/en/docs/install/#windows-stable" target="_blank"> **Yarn**</a>, <a href="https://www.npmjs.com/get-npm" target="_blank">**Node Package Manager (NPM)**</a>, <a href="https://git-scm.com/downloads" target="_blank">**Gitbash**</a> (opcional dependiendo del sistema operativo que uses) y un **editor** de código fuente (para nuestro caso utilizaremos <a href="https://code.visualstudio.com/" target="_blank">**Visual Studio Code**</a>) 

*  ## Instalación de Docusaurus versión 2. 🔧

1.	Crea un directorio para descargar Docusaurus.
2.	Ingresa a la carpeta creada desde la terminal de preferencia (Gitbash, cmd, etc.)
3.	Ejecuta la instrucción **npx @docusaurus/init@next init [name] "[template]"**, donde [name] deberá de ser reemplazado por cualquier nombre que queramos y [template] por classic para usar la pagina por default que se cargará en el sitio web. Docusaurus tiene la disponibilidad de usar varias plantillas.

![instalacion](https://github.com/dochavez/DocusaurusV2/blob/main/instalacion.jpg)

![instalacion1](https://github.com/dochavez/DocusaurusV2/blob/main/instalacion1.jpg)

4.	Asumiendo que los pasos anteriores fueron ejecutados correctamente, deberas de ver una estructura siguiente:

my-website
├── blog
│   ├── 2019-05-28-hola.md
│   ├── 2019-05-29-hello-world.md
│   └── 2020-05-30-welcome.md
├── docs
│   ├── doc1.md
│   ├── doc2.md
│   ├── doc3.md
│   └── mdx.md
├── src
│   ├── css
│   │   └── custom.css
│   └── pages
│       ├── styles.module.css
│       └── index.js
├── static
│   └── img
├── docusaurus.config.js
├── package.json
├── README.md
├── sidebars.js
└── yarn.lock

*  ## Desplegando la Aplicación. 📦

5.	Para ejecutar Docusaurus utilizamos el siguiente comando desde la terminal: **npm start** y nuestro proyecto se desplegará en nuestro navegador web con la dirección **http://localhost:3000** 

![pagina principal](https://github.com/dochavez/DocusaurusV2/blob/main/Docusaurus%20pagina%20principal.jpg)





