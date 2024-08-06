# Portafolio

## Descripción del Proyecto

Este desafío consiste en un portafolio personal que muestra las habilidades adquiridas durante el curso, así como algunos de los proyectos realizados. El portafolio ha sido desarrollado utilizando Bootstrap y Sass, con solo algunas modificaciones menores en CSS. 

#### instalacion de Bootstrap

Para instalar Bootstrap, sigue estos pasos utilizando la línea de comandos **Cmd**:

Paso 1: Crea la carpeta del proyecto con el siguiente comando:

**mkdir Portafolio-karen-godoy**

Luego, entra en la carpeta recién creada con:

**cd Portafolio-karen-godoy**

Paso 2: Inicializa un nuevo proyecto, para ello ulizamos el comando que se muestra a continuación, el cual es el proceso para crear un archivo package.json en el directorio del proyecto. Este archivo contiene información sobre el proyecto y sus dependencias:

**npm init -y**

Paso 3: Instala Bootstrap en la carpeta del proyecto con el siguiente comando:

npm install bootstrap

Este comando descargará Bootstrap y sus dependencias en la carpeta node_modules, que es necesaria para el correcto funcionamiento del proyecto. 

Esta es la forma que a mi me funciono instalar de forma correcta bootstrap.

### Selección de Paleta de Colores

Para el diseño del portafolio, se ha elegido una paleta de colores que se puede consultar en la página de [Color Hunt](https://colorhunt.co/palette/f1e5d1dbb5b5c39898987070). Esta paleta ha sido mencionada en la documentación del proyecto y se utiliza para asegurar una coherencia visual en el diseño.

### Fuente

La fuente utilizada en este proyecto es **Lato**, la cual fue obtenida de [Google Fonts](https://fonts.google.com/specimen/Lato). Lato se eligió por su legibilidad y su estilo moderno, que complementa el diseño del portafolio.

### La Ilustración

La ilustración utilizada en la maqueta fue reemplazada por una de [Undraw](https://undraw.co/), una página recomendada en el documento. La nueva ilustración representa mejor el concepto del proyecto y se alinea más con el mensaje que quiero transmitir.

### Iconos

Debido a que los iconos de la section `skills` no se cargaban correctamente en la página, decidí descargarlos en formato SVG desde [Font Awesome](https://fontawesome.com/). Por lo tanto, los iconos se encuentran en la carpeta `img`. Por el contrario los iconos de la section `contact` si estan cargados como iconos de `Font Awesome`.

# Modificar la Paleta de Colores de Bootstrap

Para personalizar la paleta de colores de Bootstrap en tu proyecto, sigue estos pasos:

1.**Crea un Archivo de Variables Personalizadas**

Primero, crea una carpeta para tus archivos de variables (por ejemplo, `variables/`) y dentro de esta carpeta, crea un archivo SCSS para definir tus colores personalizados. 

   En el archivo `_variables.scss`, define tus variables de colores de la siguiente manera:
   $primary: #987070;  // Color primario
   $secondary: #C39898; // Color secundario
   $success: #DBB5B5;  // Color de éxito
   $danger: #F1E5D1;   // Color de peligro

2. **Importa Tus Variables en el Archivo Principal SCSS**

   A continuación, importa el archivo con tus variables personalizadas en el archivo SCSS principal (`main.scss`). hay que asegurarse que la importación de las variables esté ubicada **antes de la importación de Bootstrap**. Esto garantiza que las variables sobrescriban las variables predeterminadas de Bootstrap.

   La estructura de tu archivo `main.scss` debería verse así:

   // Importar primero las variables personalizadas
   @import 'variables/variables';

   // Importar Bootstrap
   @import '~bootstrap/scss/bootstrap';

De esta manera, se puede modificar la paleta de colores de Bootstrap sin necesidad de alterar los archivos originales de la biblioteca.