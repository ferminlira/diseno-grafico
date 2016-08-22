# Frameworks

# Bootstrap
Bootstrap, es un framework originalmente creado por Twitter, que permite crear interfaces web con CSS y JavaScript, cuya particularidad es la de adaptar la interfaz del sitio web al tamaño del dispositivo en que se visualice. Es decir, el sitio web se adapta automáticamente al tamaño de una PC, una Tablet u otro dispositivo. Esta técnica de diseño y desarrollo se conoce como “responsive design” o diseño adaptativo.

El beneficio de usar responsive design en un sitio web, es principalmente que el sitio web se adapta automáticamente al dispositivo desde donde se acceda. Lo que se usa con más frecuencia, y que a mi opinión personal me gusta más, es el uso de media queries, que es un módulo de CSS3 que permite la representación de contenido para adaptarse a condiciones como la resolución de la pantalla y si trabajás las dimensiones de tu contenido en porcentajes, puedes tener una web muy fluida capaz de adaptarse a casi cualquier tamaño de forma automática.

Bootstrap tiene un soporte relativamente incompleto para HTML5 y CSS 3, pero es compatible con la mayoría de los navegadores web. La información básica de compatibilidad de sitios web o aplicaciones esta disponible para todos los dispositivos y navegadores. Existe un concepto de compatibilidad parcial que hace disponible la información básica de un sitio web para todos los dispositivos y navegadores. Por ejemplo, las propiedades introducidas en CSS3 para las esquinas redondeadas, gradientes y sombras son usadas por Bootstrap a pesar de la falta de soporte de navegadores antiguos. Esto extiende la funcionalidad de la herramienta, pero no es requerida para su uso.

Desde la versión 2.0 también soporta diseños sensibles. Esto significa que el diseño gráfico de la página se ajusta dinámicamente, tomando en cuenta las características del dispositivo usado (Computadoras, tabletas, teléfonos móviles).



-----
### Características

Desde la aparición de Bootstrap 3 el framework se ha vuelto bastante más compatible con desarrollo web responsive, entre otras características se han reforzado las siguientes:

* Soporte bastante bueno (casi completo) con HTML5 y CSS3, permitiendo ser usado de forma muy flexible para desarrollo web con unos excelentes resultados.
* Se ha añadido un sistema GRID que permite diseñar usando un GRID de 12 columnas donde se debe plasmar el contenido, con esto podemos desarrollar responsive de forma mucho más fácil e intuitiva.
* Boostrap 3 establece Media Queries para 4 tamaños de dispositivos diferentes variando dependiendo del tamaño de su pantalla, estas Media Queries permiten desarrollar para dispositivos móviles y tablets de forma mucho más fácil.
* Boostrap 3 también permite insertar imágenes responsive, es decir, con solo insertar la imagen con la clase “img-responsive” las imágenes se adaptaran al tamaño.

Todas estas características hacen que Boostrap sea una excelente opción para desarrollar webs y aplicaciones web totalmente adaptables a cualquier tipo de dispositivo.



-----


### Compatibilidad con navegadores

Boostrap es compatible con la mayoría de navegadores web del mercado, y más desde la versión 3, actualmente es totalmente compatible con los siguientes navegadores:

* Google Chrome (en todas las plataformas).
* Safari (tanto en iOS como en Mac).
* Mozilla Firefox (en Mac y en Windows).
* Internet Explorer (en Windows y Windows Phone).
* Opera (en Windows y Mac).

Actualmente existen muchísimos themes para WordPress que tienen una base Bootstrap o están desarrollados con Bootstrap, es más, podemos decir que actualmente el 80% de los themes para WordPress que son responsive están desarrollados con una base Bootstrap.



-----

### Bootstrap-Primeros pasos

####Descargando Bootstrap

Existen varias formas diferentes de empezar con Bootstrap, cada una orientada a un tipo de público en función de su nivel técnico. 

* **Descargar el código CSS y JavaScript compilado**, que es la forma más sencilla de empezar a utilizar Bootstrap. La desventaja es que esta versión no incluye ni los archivos originales ni la documentación. Para descargar esta versión, accede a getbootstrap.com y pulsa el botón Download Bootstrap.
* **Descargar el código fuente, contiene todos los archivos Less, y JavaScript originales de Bootstrap.** La desventaja es que requiere un compilador de archivos Less y cierto trabajo de configuración. Descarga la versión más reciente en el sitio github.com/twbs/bootstrap/releases.
* **Descargar el código fuente en formato Sass**, se trata de una variante de la versión anterior y que se ha creado para facilitar la integración de Bootstrap en las aplicaciones Ruby On Rails, Compass o cualquier otro proyecto basado en Sass. Descarga la versión más reciente en el sitio github.com/twbs/bootstrap-sass/releases.

#### Utiliza la CDN de Bootstrap

La empresa NetDNA aloja de forma gratuita en su CDN una copia de los archivos CSS y JavaScript de Bootstrap. Para utilizar estos archivos, modifica los siguientes dos enlaces en tus páginas (cambia el valor 3.0.0 por la versión específica de Bootstrap que quieras):

```
<!-- Versión compilada y comprimida del CSS de Bootstrap -->
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.0/css/bootstrap.min.css">
 
<!-- Tema opcional -->
<link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.1.0/css/bootstrap-theme.min.css">
 
<!-- Versión compilada y comprimida del JavaScript de Bootstrap -->
<script src="//netdna.bootstrapcdn.com/bootstrap/3.1.0/js/bootstrap.min.js"></script>
```

#### Instala Bootstrap con Bower

Utiliza este gestor de dependencias para gestionar los archivos CSS y JavaScript originales de Bootstrap y mantener una copia local de su documentación. Para ello, ejecuta el siguiente comando:

```
$ bower install bootstrap

```

#### La primera plantilla Bootstrap

Si eres nuevo en Bootstrap, puedes empezar con la plantilla HTML básica que se muestra a continuación:

El siguiente código HTML muestra una plantilla muy sencilla creada con Bootstrap:

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Plantilla básica de Bootstrap</title>
 
    <!-- CSS de Bootstrap -->
    <link href="css/bootstrap.min.css" rel="stylesheet" media="screen">
 
    <!-- librerías opcionales que activan el soporte de HTML5 para IE8 -->
    <!--[if lt IE 9]>
      <script src="https://oss.maxcdn.com/libs/html5shiv/3.7.0/html5shiv.js"></script>
      <script src="https://oss.maxcdn.com/libs/respond.js/1.4.2/respond.min.js"></script>
    <![endif]-->
  </head>
  <body>
    <h1>¡Hola mundo!</h1>
 
    <!-- Librería jQuery requerida por los plugins de JavaScript -->
    <script src="http://code.jquery.com/jquery.js"></script>
 
    <!-- Todos los plugins JavaScript de Bootstrap (también puedes
         incluir archivos JavaScript individuales de los únicos
         plugins que utilices) -->
    <script src="js/bootstrap.min.js"></script>
  </body>
</html>
```


-----


### Ejemplos de sitios web que utilizan Bootstrap

Twitter, es el ejemplo más conocido que usa este framework, sin embargo aquí te mostramos otros ejemplos que también lo usan.

#### Getflywheel.com

<div align="center">
![](http://i.imgur.com/Q9Di4Mf.jpg)
</div>
<br>


#### Atmail.com

<div align="center">
![](http://i.imgur.com/KvAe0vr.jpg)
</div>
<br>
# Material Design

Material design es un lenguaje de diseño en el que predominan animaciones, transiciones y los efectos de profundidad como la iluminación y las sombras.

Material Design quiere servirse de un diseño común para un amplio rango de dispositivos, haciendo que la experiencia de usuario sea mucho mejor. Desde nuestro smartphone, pasando por la Web, y por supuesto con las tablets, que también podrán usar este lenguaje de diseño. Aunque está diseñado especialmente para dispositivos táctiles no deja de lado la inclusión de teclado, ratón o entrada por voz.

Material Design recibe su nombre por estar basado en objetos materiales. Piezas colocadas en un espacio (lugar) y con un tiempo (movimiento) determinado.

Es un diseño donde la profundidad, las superficies, los bordes, las sombras y los colores juegan un papel principal.

Precisamente este diseño basado en objetos es una manera de intentar aproximarse a la realidad, algo que en un mundo donde todo es táctil y virtual es difícil. Material Design quiere guiarse por las leyes de la física, donde las animaciones sean lógicas, los objetos se superpongan pero no puedan atravesarse el uno al otro y demás.




-----

### Material Design para Bootstrap

Si utilizas el Bootstrap como tu framework de front-end preferido  y además te gustaría integrar el framework de diseño visual de Google no te faltan soluciones en la web.

Bootstrap de Twitter es el framework de HTML, CSS y JavaScript más popular del mercado para desarrollar de forma rapida y fácil proyectos responsive y mobile first en la web.

Material Design es un lenguaje de diseño desarrollado por Google con el objetivo de hacer una web más bonita y amigable.

“Material Design for Bootstrap“, o MDB es un framework con las mejores características de ambos mundos y puede ser lo que estabas buscando.



-----

### Características principales de MDB


* Más de 300 elementos de UI “material”
* Más de 1000 iconos material
* Fácil de instalar
* Responsive. Funciona en tablets, teléfonos y ordenadores de escritorio
* Compatible entre navegadores. Funciona en todos los navegadores modernos
* Gratuito para uso personal y profesional


-----

### ¿Cómo funciona?

MDB es un kit muy potente para Material Design que podrás usar para empezar tus nuevos proyectos o implementar en alguno ya existente.

Tendrás que registrarte y puedes optar entre la versión gratuita, que te da acceso al framework, diferentes componentes y plantillas, o la versión Pro (entre 29 y 199 dólares), que además de todo lo anterior tendrás acceso a más 100 componentes premium, soporte premium y actualizaciones ilimitadas.

**Después de bajarte el kit, ¡ya lo puedes utlizar y empezar a crear!**

Si no sabes como, el equipo de mdbostratap.com te ofrece algunas plantillas ‘starter‘ con las que puedes empezar.

**Entre los componentes de MDB más populares y que pueden dar a tu sitio web el toque profesional que necesita, puedes encontrar:**

* Plantillas (gratuito)
* Animaciones (gratuito). 74 animaciones de CSS que podrás aplicar a cada elemento de tu proyecto.
* Formularios (gratuito). Ya sabes lo difícil que es maquetar formularios. Con MDB lo tendrás mucho más fácil.  !Echa un vistazo al “Date picker” o el “Time picker”!
* Conjunto E-commerce (pro). Con carrito de compras o catalogos.
* Conjunto Magazine (pro). Maquetar tu blog dejará de ser tan complicado.
* SideNav (pro)
* Logo generator
* Parallax

MDB es un framework muy completo con lo que puedes obtener un resultado muy profesional en poco tiempo. Lo podrás utilizar para tu sitio web personal, tienda online o blog.

En el sitio web oficial, además de las plantillas gratis, también podrás encontrar tutoriales y videos para aprender.
