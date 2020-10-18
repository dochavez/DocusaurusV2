# Docusaurus Versión 2
## Instalación y Configuración para **Principiantes** 🚀 <br>
Elaborado por: **Danny Chávez** <br>


Documentar es una forma de dejar en evidencia lo que se hace para que otras personas puedan aprender, modificar, crear, diseñar y compartir. Aunque es importante mencionar que documentar puede ser una tarea complicada. Lo cual puede desencadenar que un proyecto alcance su máximo potencial. Pero gracias a Docusaurus nuestra tarea puede verse muy simplificada.
Con Docusaurus nos ayuda a crear y mantener sitios web donde podemos mostrar nuestra documentación. Gracias a la implementación de React.js, podemos contar con soporte para blogs, paginas con diseños personalizados con estilos muy elegantes y dinámicos. 


*  ## Verificación para preparar el entorno. 📋

•	Verifica que tienes instalado en tu computadora <a href="https://nodejs.org/es/" target="_blank">**Node.js**</a>, <a href="https://classic.yarnpkg.com/en/docs/install/#windows-stable" target="_blank"> **Yarn**</a>, <a href="https://www.npmjs.com/get-npm" target="_blank">**Node Package Manager (NPM)**</a>, <a href="https://git-scm.com/downloads" target="_blank">**Gitbash**</a> (opcional dependiendo del sistema operativo que uses) y un **editor** de código fuente (para nuestro caso utilizaremos <a href="https://code.visualstudio.com/" target="_blank">**Visual Studio Code**</a>) 

*  ## Instalación de Docusaurus versión 2. 🔧

1.	Crea un directorio para descargar Docusaurus.
2.	Ingresa a la carpeta creada desde la terminal de preferencia (Gitbash, cmd, etc.)
3.	Ejecuta la instrucción **npx @docusaurus/init@next init [name] "[template]"**, donde [name] deberá de ser reemplazado por cualquier nombre que queramos y [template] por classic para usar la pagina por default que se cargará en el sitio web. Docusaurus tiene la disponibilidad de usar varias plantillas.

![instalacion](https://github.com/dochavez/DocusaurusV2/blob/main/instalacion.jpg)
###### Figura 1. Ejecución de comando.

![instalacion1](https://github.com/dochavez/DocusaurusV2/blob/main/instalacion1.jpg)
###### Figura 2. Confirmación de la instalación de forma exitosa

4.	Asumiendo que los pasos anteriores fueron ejecutados correctamente, deberas de ver una estructura siguiente:

![estructura de proyecto](https://github.com/dochavez/DocusaurusV2/blob/main/estructura%20del%20proyecto.jpg)
###### Figura 3. Estructura del proyecto de Docusaurus.


*  ## Desplegando la Aplicación. 📦

5.	Para ejecutar Docusaurus utilizamos el siguiente comando desde la terminal: **npm start** y nuestro proyecto se desplegará en nuestro navegador web con la dirección **http://localhost:3000** 

![pagina principal](https://github.com/dochavez/DocusaurusV2/blob/main/Docusaurus%20pagina%20principal.jpg)
###### Figura 4. Página principal.

*  ## Analizando la estructura del proyecto instalado.📜

•	La carpeta **/blog/**: contiene los archivos de Markdown del blog, los cuales se usan para desplegar diferentes tipos de contenidos presentados por diferentes usuarios. <br>
•	La carpeta **/docs/**: contiene los archivos de Markdown para la sección de los documentos.<br>
•	La carpeta **/src/**: contiene archivos fuentes con extension **.js** y hojas de estilos (CSS). Es importante mencionar que cualquier archivo que este dentro de la ruta **/src/pages** será convertido dentro de la página web. <br>
•	La carpeta **/static/**: no es más que un Directorio estático. Cualquier contenido dentro de aquí se copiará en la raíz del directorio de compilación final. La cual se utilizará para desplegar nuestro sitio web en internet. <br>
•	El archivo **/docusaurus.config.js**:  es un archivo de configuración que contiene la configuración completa del sitio. <br> 
•	El archivo **/package.json**: Es una aplicación de React. Puede instalar y usar cualquier paquete npm que desee en ellos. <br>
•	El archivo **/sidebar.js**: utilizado por la documentación para especificar el orden de los documentos en la barra lateral.<br>

*  ## Personaliza tu Sitio.🛠️

Docusaurus nos permite una gran flexibilidad y adaptación a nuestras necesidades. Es por eso que en el archivo denominado **docusaurus.config.js** puedes modificar las directivas **title** y **tagline** poniendo cualquier nombre que quieras. Para el caso del**favicon** debes de agregar una imagen con extensión **.ico**. Un buen recursos que puedes usar para crear este tipo de archivos es accediendo al sitio web <a href="https://favicon.io/favicon-converter/" target="_blank"> favicon.io </a>. Una vez que tengas el nuevo archivo, deberas de copiarlo y reemplazarlo adentro de la carpeta **static\img**. Ahora puede probar los cambios iniciando el proyecto con el comando **npm run start** o puedes utilizar **yarn run start** desde la terminal. Recuerda estar adentro de la carpeta del directorio que creastes en el paso **numero 1** de este tutorial. Dirigite a **http://localhost:3000** para ver los cambios efectuados.


![website](https://github.com/dochavez/DocusaurusV2/blob/main/website.jpg)
###### Figura 5. Agregando Título, Sutitulos e ícono.


![Resultado](https://github.com/dochavez/DocusaurusV2/blob/main/Resultado.jpg)
###### Figura 6. Muestra de cambios efectuados.

*  ## Describiendo más elementos de nuestra pagina principal.🏠

El archivo **index.js** es la página de inicio de nuestro sitio web. En ella, se exportan los componentes de React que son presentados entre la barra de navegación y el pie de la página. Puedes crear tus propios componentes dentro del archivo **index.js**. Ya que la plantilla incluye Hojas de Estilos (CSS) creadas por el equipo de Docusaurus bajo una estructura que lleva por nombre <a href="https://facebookincubator.github.io/infima/" target="_blank">Infima</a>.

*  ## Variedad de Colores.🌈

Tal como mencionamos anteriormente, **Infima** soporta las Hojas de Estilos (conocidas como CSS) para hacer algun cambio de colores a nuestro sitio web. Esta acción la podemos aplicar dentro de la ruta **src/css/custom.css**

![Colores css](https://github.com/dochavez/DocusaurusV2/blob/main/colores%20css.jpg)
###### Figura 7. Control de Colores de nuestra página principal.

Es importante destacar que los valores de los colores se deben de agregar en formato hexadecimal. Si quieres conocer todas las posibles combinaciones de colores que puedes aplicar, puedes visitar el siguiente sitio web <a href="https://htmlcolorcodes.com/es/" target="_blank"> www.htmlcolorcodes.com/es/</a>.

*  ## Barra de Navegación. 🗄️

La barra de navegación conocida como **navbar** permite agregar enlaces a otras páginas dentro del mismo sitio. Para esto, debemos proporcionar una ruta, aunque tambien puede ser una URL que nos lleve a un enlace externo. Para modificar la barra de navegacion, debemos de ubicarnos dentro del archivo denominado **docusaurus.config.js**

![Barra de Navegacion](https://github.com/dochavez/DocusaurusV2/blob/main/barra%20de%20navegacion.jpg)
###### Figura 8. Identificación de la Barra de Navegación.

![navbar](https://github.com/dochavez/DocusaurusV2/blob/main/navbar.jpg)
###### Figura 9. Despliegue de la Barra de Navegación.

*  ## Pie de Página. 📃

Al igual que la barra de navegación, el componente de pie de página puede ser modificado. El cual se encuentra dentro del archivo **docusaurus.config.js**. Se pueden agregar enlaces que nos lleven a otra información de interes dentro del sitio o bien pueden ser enlaces externos.

![Pie de Pagina](https://github.com/dochavez/DocusaurusV2/blob/main/pie%20de%20pagina.jpg)
###### Figura 10. Identificación del Pie de Página

![Footer](https://github.com/dochavez/DocusaurusV2/blob/main/footer.jpg)
###### Figura 11. Despliegue del Pie de Página

Finalmente, podemos decir que también podemos agregar texto relacionado a los derechos de autor al pie de la página. Esto lo podemos encontrar en la sección 
```
copyright: `Copyright © ${new Date().getFullYear()} My Project, Inc. Built with Docusaurus.`, 
```
dentro del archivo **docusaurus.config.js**.

*  ## Sección de Documentos. 📖

Una de las geniales caracteristicas que proporciona Docusaurus es que podemos proporcionar una gran variedad de documentos que contienen diferentes tópicos de información. Estos documentos se almacenan dentro de la carpeta denominada **docs**. Para crear documentos debemos de crear archivos que contengan la extensión **.md**. Una vez que creemos nuestro documento, Docusaurus los mostrara de manera instantanea. La estructura que debemos de seguir para crear un documento es
```
---
id: AGREGA_UN_NOMBRE
title: AGREGA_UN TITULO
---
# AGREGAR LA INFORMACION DESPUES DE ESTA LINEA
```
Donde **id** es el nombre del documento que vamos a crear, **title** es el titulo que aparecerá en nuestra sección de documentos de nuestro sitio web. 

*  ## Organizando nuestros Documentos. 📚

Si queremos agregar una sección para que nuestros documentos aparezcan organizados por categorias, debemos de agregar una sección especial para ellos. Por lo tanto, todos ellos se presentaran como una estructura organizada, permitiendo una fácil navegación entre ellos. Si queremos agregar nuevas secciones debemos de ubicarnos dentro del archivo **sidebar.js**

![sidebar](https://github.com/dochavez/DocusaurusV2/blob/main/sidebar.jpg)
###### Figura 12. Identificación de la estructura de nuestros documentos.

![sidebar1](https://github.com/dochavez/DocusaurusV2/blob/main/sidebar1.jpg)
###### Figura 13. Despliegue de la organización de nuestros documentos.

*  ## Controlando las versiones de nuestro proyecto. 🧬

El control de versiones es importante para mantener al día nuestro trabajo. Eso significa que muchos cambios o actualizaciones pueden ocurrir todos los dias. Por lo tanto es importante llevar un buen control de las versiones que se nos presentan. Es importante mantener presente que las actualizaciones en cuanto al control de versiones deben de estar en correspondencia con las necesidades de nuestros documentos. En otras palabras, solo si es necesario hacer un cambio. Para efectuar un control de versiones debemos de ubicarnos dentro del archivo **package.json** y agregar por ejemplo el siguiente script:
```"version": "docusaurus doc:version"```, después podemos ejecutar el siguiente comando ```npm run version <version>``` donde "<version>" es el nuevo número de versión que será agregado tanto para el control de nuestros documentos como la estructura de los mismos. Es decir, nuestro **sidebar**

```
# Estructura del Directorio aplicando control de versiones. Referencia: https://v2.docusaurus.io/docs/versioning

website
├── sidebars.json        
├── docs                 
│   ├── foo
│   │   └── bar.md       
│   └── hello.md         
├── versions.json        
├── versioned_docs
│   ├── version-1.1.0
│   │   ├── foo
│   │   │   └── bar.md   
│   │   └── hello.md
│   └── version-1.0.0
│       ├── foo
│       │   └── bar.md   
│       └── hello.md
├── versioned_sidebars
│   ├── version-1.1.0-sidebars.json
│   └── version-1.0.0-sidebars.json
├── docusaurus.config.js
└── package.json

```









