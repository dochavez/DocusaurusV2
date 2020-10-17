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

![estructura de proyecto](https://github.com/dochavez/DocusaurusV2/blob/main/estructura%20del%20proyecto.jpg)


*  ## Desplegando la Aplicación. 📦

5.	Para ejecutar Docusaurus utilizamos el siguiente comando desde la terminal: **npm start** y nuestro proyecto se desplegará en nuestro navegador web con la dirección **http://localhost:3000** 

![pagina principal](https://github.com/dochavez/DocusaurusV2/blob/main/Docusaurus%20pagina%20principal.jpg)

*  ## Analizando la estructura del proyecto instalado de Docusaurus versión 2.📜

•	La carpeta **/blog/**: contiene los archivos de Markdown del blog, los cuales se usan para desplegar diferentes tipos de contenidos presentados por diferentes usuarios. <br>
•	La carpeta **/docs/**: contiene los archivos de Markdown para la sección de los documentos.<br>
•	La carpeta **/src/**: contiene archivos fuentes con extension **.js** y hojas de estilos (CSS). Es importante mencionar que cualquier archivo que este dentro de la ruta **/src/pages** será convertido dentro de la página web. <br>
•	La carpeta **/static/**: no es más que un Directorio estático. Cualquier contenido dentro de aquí se copiará en la raíz del directorio de compilación final. La cual se utilizará para desplegar nuestro sitio web en internet. <br>
•	El archivo **/docusaurus.config.js**:  es un archivo de configuración que contiene la configuración completa del sitio. <br> 
•	El archivo **/package.json**: Es una aplicación de React. Puede instalar y usar cualquier paquete npm que desee en ellos. <br>
•	El archivo **/sidebar.js**: utilizado por la documentación para especificar el orden de los documentos en la barra lateral.<br>

*  ## Personaliza tu Sitio.🛠️

Docusaurus nos permite una gran flexibilidad y adaptación a nuestras necesidades. Es por eso que en el archivo denominado docusaurus.config.js modificaremos las directivas **title** y **tagline** 




