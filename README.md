# Portafolio

## Descripción del Proyecto

### Selección de Paleta de Colores

Para el diseño del portafolio, se ha elegido una paleta de colores que se puede consultar en la página de [Color Hunt](https://colorhunt.co/palette/f1e5d1dbb5b5c39898987070). Esta paleta ha sido mencionada en la documentación del proyecto y se utiliza para asegurar una coherencia visual en el diseño.

### Fuente

La fuente utilizada en este proyecto es **Lato**, la cual fue obtenida de [Google Fonts](https://fonts.google.com/specimen/Lato). Lato se eligió por su legibilidad y su estilo moderno, que complementa el diseño del portafolio.

### La Ilustración

La ilustración utilizada en la maqueta fue reemplazada por una de [Undraw](https://undraw.co/), una página recomendada en el documento. La nueva ilustración representa mejor el concepto del proyecto y se alinea más con el mensaje que quiero transmitir.

### Modificar la paleta de colores de bootstrap

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

De esta manera, puedes modificar la paleta de colores de Bootstrap sin necesidad de alterar los archivos originales de la biblioteca

### icons 

Debido  a que los iconos no me cargaron bien en la página, decidí descargarlos en formato svg de la página de [Font Awesome] (https://fontawesome.com/), por lo tanto los iconos se encuentran en la carpeta img.