# Imágenes

# Gráficos de mapas de bits

Algunos conceptos pueden conocerse con distintos nombres, especialmente si se aceptan las denominaciones de otras lenguas. Eso es lo que sucede con la noción de mapa de bits, que también aparece mencionada como bitmap, pixmap, imagen matricial o imagen rasterizada. 

Se trata de aquellas imágenes que se forman a partir de puntos, llamados píxeles dispuestos en un rectángulo o tabla, que se denominada raster. Cada píxel contiene la información del color, la cual puede o no contener transparencia, y ésta se consigue combinando el rojo, el verde y el azul. Nótese la diferencia con la pintura, donde los colores primarios contienen el amarillo en lugar del verde.
 
Las imágenes de mapa de bits (bitmaps o imágenes raster) están formadas por una rejilla de celdas, a cada una de las cuales, denominada píxel (Picture Element, Elemento de Imagen), se le asigna un valor de color y luminancia propios, de tal forma que su agrupación crea la ilusión de una imagen de tono continuo.

<div align="center">
![](http://i.imgur.com/xFwRCYx.jpg)
</div>
<br>

Una imagen de mapa de bits es creada mediante una rejilla de píxeles única. Cuando se modifica su tamaño, se modifican grupos de píxeles, no los objetos o figuras que contiene, por lo que estos suelen deformarse o perder alguno de los píxeles que los definen. Por lo tanto, una imagen de mapa de bits está diseñada para un tamaño determinado, perdiendo calidad si se modifican sus dimensiones, dependiendo esta pérdida de la resolución a la que se ha definido la imagen.

Los gráficos de mapa de bits se obtienen normalmente a partir de capturas de originales en papel utilizando escáneres, mediante cámaras digitales o directamente en programas gráficos. También existen multitud de sitios en Internet que ofrecen imágenes de este tipo de forma gratuita o por una cantidad variable de dinero.


-----


## Resolución de una imagen de mapa de bits
<br>

La resolución de una imagen es el un concepto que suele confundir bastante, principalmente porque no es un concepto único, sino que depende del medio en el que la imagen vaya a ser visualizada o tratada. Así, podemos hablar de resolución de un archivo digital, resolución de impresión, resolución de semitono, resolución de escaneado, etc.

Tal vez el concepto más ligado a la propia naturaleza de la imagen digital sea el de resolución del archivo digital, definida como el número de píxeles distintos que tiene una imagen por unidad de longitud, es decir, la densidad de éstos en la imagen. Sus unidades de medida son los píxeles por pulgada (ppp o ppi, pixels per inch, en inglés) o los píxeles por centímetro (más raramente). Cuanto mayor sea esta resolución, más contenedores de información (píxeles) tiene el fichero digital, más calidad tendrá la imagen y más peso en Kb tendrá el fichero.

<div align="center">
![](http://i.imgur.com/i5ATW1Z.jpg)
</div>
<br>

Esta resolución está muy ligada al concepto de resolución de pantalla en un monitor, referida al número de píxeles por pulgada existentes en la pantalla del monitor en el que se visualiza la imagen. Una configuración del monitor en alta resolución exhibirá más píxeles por pulgada, por lo que éstos serán más pequeños, permitiendo una mejor visualización de la imagen en pantalla. En ningún caso podremos visualizar una imagen a mayor resolución que la de pantalla, que suele ser de 72 ppp en un sistema Mac y de 96 ppp en un PC.

<div align="center">
![](http://i.imgur.com/zQovJMm.gif)
</div>
<br>

Una vez definida la resolución de pantalla, el tamaño de los píxeles dependerá del tamaño físico de la pantalla, medido en pulgadas. Las resoluciones de pantalla más comunes en la actualidad son 800x600 y 1024x768 píxeles, oscilando los tamaños de pantalla entre 15 y 21 pulgadas.



-----

## Dimensiones de una imagen mapa de bits
<br>

Puesto que la resolución de una imagen se mide en pulgadas o centímetros, parecería lógico pensar que estas mismas unidades se utilizaran para definir las dimensiones de una imagen.

El principal inconveniente de obrar así es que estas unidades expresan valores de medida absolutos, mientras que los dispositivos de salida suelen trabajar en dimensiones relativas (píxeles o puntos de impresión). Por ejemplo, los monitores trabajan en píxeles, adaptando las dimensiones de los objetos que presenta a la resolución de pantalla usada, por lo que una imagen se visualizará más pequeña cuanto mayor sea la resolución.

<div align="center">
![](http://i.imgur.com/ujLjovf.gif)
</div>
<br>

Además, si se utilizan centímetros o pulgadas será necesario también conocer también la resolución de la imagen, medida en píxeles por unidad de longitud, para saber la información gráfica que contiene.

Es conveniente entonces utilizar como unidades de medida de las dimensiones de una imagen bien los píxeles de pantalla, si está destinada a mostrarse en un monitor, bien los puntos de impresión, si está destinada a la imprenta o impresora.

El espacio relativo de pantalla ocupado por una imagen de dimensiones 150x100 píxeles será el mismo sea cual sea la resolución, con la única diferencia de que cuanto menor sea ésta, más grande será su tamaño absoluto en pulgadas o centímetros, al ser de mayor tamaño los píxeles.

No olvidemos que la resolución útil de una imagen nunca es mayor que la del medio en el que se visualiza. Una imagen escaneada a 200 ppp se visualizará en un monitor de PC con la configuración por defecto a 96 ppp, desperdiciándose el resto de información sobre los valores de los píxeles de la imagen, mientras que una imagen escaneada a 50 ppp se visualizará igualmente a 96 ppp en la pantalla del monitor, aunque en este caso su calidad será escasa, al no contener los píxeles suficiente información gráfica.

Resumiendo, sea cual sea el tamaño de los píxeles o puntos de una imagen, una vez presentados en un medio dado su tamaño se adaptará al de los píxeles éste, por lo que esta unidad de medida resulta la más conveniente en todos los casos.

Una consideración importante: las dimensiones de una imagen en pantalla no suelen coincidir con las dimensiones de la imagen impresa, ya que, mientras en la resolución de pantalla permanece constante, la resolución propia de la imagen varía al cambiar el tamaño de ésta, y viceversa, según las siguientes reglas:

* Si disminuimos la resolución de la imagen, la anchura y la altura aumentarán.
* Si aumentamos la resolución, la anchura y la altura disminuirán.
* Si aumentamos la anchura o la altura, la resolución disminuirá.
* Si disminuimos la anchura o la altura, la resolución aumentará.

Por lo tanto, si queremos aumentar las dimensiones de una imagen en un programa como Photoshop sin perder calidad, lo mejor es trabajar con la imagen en una alta resolución (sobre dos veces la resolución final deseada). Entonces, disminuiremos la resolución o aumentaremos la anchura y la altura (ambas acciones producirán resultados similares). Una vez que las dimensiones de la imagen sean las deseadas podremos disminuir la resolución al valor deseado.

Por otra parte, el tamaño de visualización de una imagen en pantalla es a menudo diferente de su tamaño impreso. Los píxeles de la imagen se traducen directamente a píxeles del monitor, por lo que cuando la resolución de la imagen es más alta que la resolución del monitor aparece la imagen en pantalla más grande que sus dimensiones especificadas para la impresión.

Por ejemplo, una imagen de 1 x 1 pulgadas a una resolución de 144 ppp ocupará en una pantalla de resolución 72 ppp un área de 2 x 2 pulgadas, ya que como el monitor puede exhibir solamente 72 píxeles por pulgada, necesita 2 pulgadas para mostrar los 144 píxeles de la imagen.

# Gestión del color en mapas de bits

Las posibles configuraciones de color que podemos tener en una imagen de tipo mapa de bits son muchas, en ellas, podemos ver  el modo de color, la profundidad, etc, lo que será abordado a continuación.


-----
## Modo de color

El modo de color expresa la cantidad máxima de datos de color que se pueden almacenar en un determinado formato de archivo gráfico.

Podemos considerar el modo de color como el contenedor en que colocamos la información sobre cada píxel de una imagen. Así, podemos guardar una cantidad pequeña de datos de color en un contenedor muy grande, pero no podremos almacenar una gran cantidad de datos de color en un contenedor muy pequeño.

Los principales modos de color utilizados en aplicaciones gráficas son:

#### Modo Bit Map o monocromático

Correspondiente a una profundidad de color de 1 bit, ofrece una imagen monocromática formada exclusivamente por los colores blanco y negro puros, sin tonos intermedios entre ellos.

<div align="center">
![](http://i.imgur.com/15e2EwO.gif)
</div>
<br>

Para convertir una imagen a modo monocromático hay que pasarla antes a modo escala de grises.En este modo no es posible trabajar con capas ni filtros.

#### Modo Escala de Grises

Este modo maneja un solo canal (el negro) para trabajar con imágenes monocromáticas de 256 tonos de gris, entre el blanco y el negro.

<div align="center">
![](http://i.imgur.com/YOAC0B9.jpg)
</div>
<br>

El tono de gris de cada píxel se puede obtener bien asignándole un valor de brillo que va de 0 (negro) a 255 (blanco), bien como porcentajes de tinta negra (0% es igual a blanco y 100% es igual a negro). Las imágenes producidas con escáneres en blanco y negro o en escala de grises se visualizan normalmente en el modo escala de grises.

El modo Escala de Grises admite cualquier formato de grabación, y salvo las funciones de aplicación de color, todas las herramientas de los programas gráficos funcionan de la misma manera a como lo hacen con otras imágenes de color.

Si se convierte una imagen modo de color a un modo Escala de Grises y después se guarda y se cierra, sus valores de luminosidad permanecerán intactos, pero la información de color no podrá recuperarse.

#### Modo Color Indexado

Denominado así porque tiene un solo canal de color (indexado) de 8 bits, por lo que sólo se puede obtener con él un máximo de 256 colores.

<div align="center">
![](http://i.imgur.com/3RJFWQP.jpg)
</div>
<br>

En este modo, la gama de colores de la imagen se adecua a una paleta con un número restringido de ellos, por lo que puede resultar útil para trabajar con algunos formatos que sólo admiten la paleta de colores del sistema.

También resulta útil reducir una imágenes a color 8 bits para su utilización en aplicaciones multimedia, ya que con ello se consiguen ficheros de menos peso.

Su principal inconveniente es que la mayoría de las imágenes del mundo real se componen de más de 256 colores. Además, aunque admite efectos artísticos de color, muchas de las herramientas de los principales programas gráficos no están operativas con una paleta de colores tan limitada.

#### Modo Color RGB

Trabaja con tres canales, ofreciendo una imagen tricromática compuesta por los colores primarios de la luz, Rojo(R), Verde(G) y Azul(B), construida con 8 bits/pixel por canal (24 bits en total). Con ello se consiguen imágenes a todo color, con 16,7 millones de colores distintos disponibles, más de los que el ojo humano es capaz de diferenciar.

<div align="center">
![](http://i.imgur.com/uWZA1Uo.jpg)
</div>
<br>

Es un modelo de color aditivo (la suma de todos los colores primarios produce el blanco), siendo el estándar de imagen de todo color que se utilice con monitores de video y pantallas de ordenador.

Las imágenes de color RGB se obtienen asignando un valor de intensidad a cada píxel, desde 0 (negro puro) a 255 (blanco puro) para cada uno de los componentes RGB.

Es el modo más versátil, porque es el único que admite todas las opciones y los filtros que proporcionan las aplicaciones gráficas. Además, admite cualquier formato de grabación y canales alfa.

#### Modo Color CMYK

Trabaja con cuatro canales de 8 bits (32 bits de profundidad de color), ofreciendo una imagen cuatricromática compuesta de los 4 colores primarios para impresión: Cyan (C), Magenta (M), Amarillo(Y) y Negro (K).

<div align="center">
![](http://i.imgur.com/ZbwoqVM.jpg)
</div>
<br>

Es un modelo de color sustractivo, en el que la suma de todos los colores primarios produce teóricamente  el negro, que proporciona imágenes a todo color y admite cualquier formato de grabación, siendo el más conveniente cuando se envía la imagen a una impresora de color especial o cuando se desea separar los colores para la filmación o imprenta (fotolitos).

Su principal inconveniente es que sólo es operativo en sistemas de impresión industrial y en las publicaciones de alta calidad, ya que, exceptuando los escáneres de tambor que se emplean en fotomecánica, el resto de los digitalizadores comerciales trabajan en modo RGB.

El proceso de convertir una imagen RGB al formato CMYK crea un separación de color. En general, es mejor convertir una imagen al modo CMYK después de haberla modificado. Modificar imágenes en modo RGB es más eficiente porque los archivos CMYK son un tercio más grandes que los archivos RGB.

#### Modo Color Lab

Consiste en tres canales, cada uno de los cuales contiene hasta 256 tonalidades diferentes: un canal L de Luminosidad y dos canales cromáticos, A (que oscila entre verde y rojo) y B (que oscila entre azul y amarillo). El componente de luminosidad L va de 0 (negro) a 100 (blanco). Los componentes A (eje rojo-verde) y B (eje azul-amarillo) van de +120 a -120.


<div align="center">
![](http://i.imgur.com/7J8atDx.gif)
</div>
<br>

El modelo de color Lab se basa en el modelo propuesto en 1931 por la CIE (Commission Internationale d'Eclairage) como estándar internacional para medir el color. En 1976, este modelo se perfeccionó y se denominó CIE Lab.

<div align="center">
![](http://i.imgur.com/iFsqF1p.jpg)
</div>
<br>

El color Lab es independiente del dispositivo, creando colores coherentes con independencia de los dispositivos concretos para crear o reproducir la imagen (monitores, impresoras, etc.).

Este modo permite cambiar la luminosidad de una imagen sin alterar los valores de tono y saturación del color, siendo adecuado para transferir imágenes de unos sistemas a otros, pues los valores cromáticos se mantienen independientes del dispositivo de salida de la imagen.

<div align="center">
![](http://i.imgur.com/TsOueNW.jpg)
</div>
<br>


Se usa sobre todo para trabajar en imágenes Photo CD o para modificar la luminancia y los valores del color de una imagen independientemente. También se puede usar el modo Lab para conservar la fidelidad del color al trasladar archivos entre sistemas y para imprimir en impresoras de PostScript de Nivel 2.

Sólo las impresoras PostScript de nivel 2 puede reproducir esta imágenes. Para impresiones normales, se recomienda pasar las imágenes a RGB o a CMYK.

#### Modo Duotono

Modo de color que trabaja con imágenes en escala de grises, a las que se le pueden añadir tintas planas (3 para cada imagen, más el negro), con el fin de colorear distintas gamas de grises.


<div align="center">
![](http://i.imgur.com/zPlab4i.jpg)
</div>
<br>

Sólo posee un canal de color (Duotono, Tritono o Cuatritono, dependiendo del número de tintas).

Con este método podemos obtener fotos en blanco y negro viradas al color que queramos. Suele ser empleado en impresión, donde se usan dos o más planchas para añadir riqueza y profundidad tonal a una imagen de escala de grises.

El problema que presenta este modo es que en los duotonos, tritonos y cuadritonos sólo hay un canal, por lo que no es posible tratar cada tinta de forma distinta según las zonas de la imagen. Es decir, no podemos hacer una zona en la que solo haya, por ejemplo, un parche cuadrado de tinta roja, mientras que en el resto sólo hay una imagen de semitono en blanco y negro.

#### Modo Multicanal

Posee múltiples canales de 256 niveles de grises, descomponiendo la imagen en tantos canales alfa como canales de color tuviera el original (una imagen RGB quedará descompuesta en 3 canales y una CMYK en 4 canales).

En este modo, cada tinta es un canal que a la hora de imprimir se superpondrá en el orden que determinemos sobre los otros. Por ello, es posible tratar cada zona de forma particularizada.

<div align="center">
![](http://i.imgur.com/jhpZIcD.jpg)
</div>
<br>

Se utiliza en determinadas situaciones de impresión en escala de grises. También, para ensamblar canales individuales de diversas imágenes antes de convertir la nueva imagen a un modo de color, pues los canales de color de tinta plana se conservan si se convierte una imagen a modo multicanal.

Al convertir una imagen en color a multicanal, la nueva información de escala de grises se basa en los valores de color de los píxeles de cada canal. Si la imagen estaba en modo CMYK, el modo multicanal crea canales de tinta plana cian, magenta, amarilla y negra. Si estaba en modo RGB, se crean canales de tinta plana cian, magenta y amarilla.



-----

## Gestión del color en mapas de bits

Los gráficos de mapa de bits almacenan una completa información sobre el color de cada uno de sus píxeles constituyentes. Cuantos más colores pueda tener la imagen, más calidad final tendrá y más información será necesario almacenar.

Relacionados con el número de colores posibles, sus características y su almacenamiento encontramos los siguientes conceptos:

#### Profundidad de color

La profundidad de color de una imagen se refiere al número de colores diferentes que puede contener cada uno de los puntos o píxeles que la forman, y depende de la cantidad de información (número de bits) que puede almacenar un píxel.

<div align="center">
![](http://i.imgur.com/LbFwuJc.jpg)
</div>
<br>

Cuanto mayor sea la profundidad de bit en una imagen, mayor será la cantidad de tonos (escala de grises o color) que puedan ser representados, más colores habrá disponibles y más exacta será la representación del color en la imagen digital. Las imágenes digitales se pueden producir en blanco y negro, a escala de grises o a color.

Una imagen en blanco y negro (bitonal) está representada por píxeles que constan de 1 bit de información cada uno, por lo que pueden representar dos tonos (típicamente negro y blanco), utilizando los valores 0 para el negro y 1 para el blanco o viceversa.

Una imagen a escala de grises está compuesta por píxeles representados por múltiples bits de información, que típicamente varían entre 2 bits (4 tonos) a 8 bits (256 tonos) o más.

Una imagen a color está típicamente representada por una profundidad de bits entre 8 y 32 bits. En una imagen de 24 bits, los bits por lo general están divididos en tres grupos (8 para el rojo, 8 para el verde y 8 para el azul). Para representar otros colores se utilizan combinaciones de esos bits, consiguiéndose en total 16,7 millones de valores de color.

Con 32 bits por píxel también se siguen utilizando 24 bits para la representación del color. Los 8 bits restantes se utilizan para el denominado canal alfa, valor independiente del color que se asigna a cada píxel de la imagen, utilizado para definir el grado de transparencia de cada punto de la imagen. Un valor 0 indica que el punto es totalmente transparente, mientras que un valor 255 indica que será totalmente visible (opaco).

La cantidad de colores utilizados en la imagen influye mucho en el tamaño del archivo que la contiene. cuantos más colores se utilicen, más grande será el tamaño del fichero gráfico necesario.

#### Rango dinámico

Es el rango de diferencia tonal entre la parte más clara y la más oscura de una imagen.

Cuanto más alto sea el rango dinámico, más matices se podrán representar, a pesar de que el rango dinámico no se correlaciona en forma automática con la cantidad de tonos reproducidos.

<div align="center">
![](http://i.imgur.com/9krsD1E.jpg)
</div>
<br>

En este ejemplo, la imagen de la derecha posee un rango dinámico más amplio, pero una cantidad limitada de tonos representados (observa la falta de detalle en las sombras). La imagen izquierda, por el contrario, posee un rango dinámico más estrecho, pero una mayor cantidad de tonos representados.

El rango dinámico también describe la capacidad de un sistema digital de reproducir información tonal. Esta capacidad es más importante en los documentos de tono continuo, como las fotografías, donde puede ser el aspecto más importante de la calidad de imagen.

#### Paletas de color

A la hora de trabajar con imágenes en formato digital se debe tener en cuenta la configuración de los sistemas utilizados para visualizarlas, ya que esto condicionará el proceso de edición de las mismas.

La mayoría de los ordenadores personales limitan el número de colores que se pueden mostrar simultáneamente a 256. Los colores disponibles, en lugar de ser un conjunto fijo, pueden ser seleccionados de una paleta de 16 millones de colores (el modelo RGB). Es decir, la gama total de colores cubre todas esas combinaciones, pero en cada momento sólo es posible mostrar 256 diferentes.

Para solucionar esta deficiencia, manteniendo un número máximo de 256 colores (8 bits por canal), se introdujeron las paletas de color, en las que se utilizan los colores que sean más apropiados para la imagen (desde 4 a 256). La paleta puede ser exacta (escoge los mismos colores que aparecen en la imagen), adaptable (escoge los colores que encuentra), web (escoge los colores más próximos dentro de la paleta WebSafe), etc.

<div align="center">
![](http://i.imgur.com/WaRem6t.jpg)
</div>
<br>

Las imágenes que utilizan una paleta de colores propia requieren un espacio adicional en el archivo para guardar esta información. La información de cada uno de los colores utilizados en la paleta ocupará 24 bits (8 bits par cada color básico), por lo que para almacenar una paleta de 256 colores se requerirán 6.144 bits (256 valores x 24 bits = 6.144 bits).

Una vez definida la paleta, la información relativa a cada uno de los puntos que forman la imagen no contendrá el valor absoluto del color de ese punto, sino que hará referencia a uno de los colores de la paleta. Será la tarjeta gráfica del ordenador la que utilizará la información de la paleta de color para saber en qué proporciones se debe mezclar los tres colores básicos que permiten cada uno de los colores.

El resultado es una gama de colores casi real con un número de colores pequeño, con lo que el fichero gráfico resultante ocupará menos espacio. Por este motivo, y por la existencia de formatos gráficos que sólo permiten trabajar con 256 colores, las paletas de color se mantienen vigentes, a pesar de la mejora de prestaciones de las tarjetas de vídeo, capaces de trabajar en la actualidad con millones de colores sin pérdida de rendimiento del sistema.

# Peso y optimización de ficheros gráficos

Cuando trabajamos con archivos gráficos en general y con mapas de bits en particular debemos tener en cuenta ciertaos aspectos fundamentales ya que lo que se busca es tener controlado el peso de los archivos, de modo que puedan ocupar menos espacio y por tanto ser transferidos con mayor rapidez.


-----

### Peso de los archivos gráficos

Los mapas de bits pueden estar definidos en un número variable de colores. Como regla general, cuantos más colores tenga la imagen, mayor calidad tendrá, aunque esta regla depende mucho de la imagen en sí.

Por ejemplo, una letra negra sobre fondo blanco (1 bit de profundidad de color), formada por líneas rectas horizontales y verticales, sólo necesitará estos dos colores para visualizarse de forma correcta, aunque aumentemos su tamaño (resolución).


<div align="center">
![](http://i.imgur.com/zFCOqBe.gif)
</div>
<br>

Si trabajamos con una profundidad de color de 8 bits tendremos 256 colores posibles para cada píxel (caso de iconos o ilustraciones en formato GIF, por ejemplo) y si aumentamos la profundidad a 24 bits tendremos millones de colores para cada píxel de la imagen (caso de fotografías en formato JPG o PNG, por ejemplo).

También podemos definir diferentes resoluciones para una imagen. Cuanto mayor sea la resolución, más píxeles formarán la imagen, más datos de información necesitará y, por lo tanto, mayor será el tamaño del fichero resultante.

Por lo tanto, cuantos más colores tenga una imagen y cuanto mayor sea su resolución, mayor peso tendrá el fichero necesario para almacenarla.

<div align="center">
![](http://i.imgur.com/dOV6yWC.gif)
</div>
<br>

En la fórmula anterior, ancho y alto están dados en pulgadas, resolución en píxeles por pulgada y profundidad del color en bites.

Para una imagen de 3 x 2 pulgadas a una resolución de 72 ppp y con una profundidad de color de 8 bits, por ejemplo, tendremos:

**Peso fichero = [[(3 x 72) x (2 x 72)] x 8] / 8 = 31104 bytes = 31 Kb**

Si las dimensiones de la imagen está en centímetros, basta dividir estos por 2,54. Así, una imagen de 1 x 1 pulgadas a una resolución de 300 ppp y con una profundidad de color de 24 bits (color real) tendrá un peso de: contiene un total de 90.000 píxeles.

**Peso fichero = [[(1 x 300) / 2,54 x (1 x 300) / 2,54] x 24] / 8 = 41850 bytes = 419 Kb**

Si trabajamos directamente con píxeles (captura con cámara digital, por ejemplo), bastará multiplicar las dimensiones de la imagen entre sí y por la profundidad de color en bits para determinar la cantidad de bits presentes en un archivo de imagen., y dividiendo el resultado entre 8, tendremos el peso del fichero en bytes.

<div align="center">
![](http://i.imgur.com/1P9UHiz.gif)
</div>
<br>

Como vemos, los pesos obtenidos son muy altos, sobre todo en el caso de imágenes destinadas a Internet, donde el ancho de banda es un recurso limitado.



-----

### Optimización de ficheros gráficos

Generalmente, los ficheros de imágenes de mapa de bits necesitan almacenar mucha información gráfica, lo que hace que su peso final en bytes sea excesivo, tanto para su impresión (si la imagen es muy grande puede durar mucho el proceso de impresión) como para su transferencia por Internet, medio en el que el ancho de banda está muy limitado.

Con objeto de minimizar el peso de los ficheros gráficos se han desarrollado diferentes técnicas de optimización basadas en dos principios diferentes:

* Reducir el número de colores utilizados en la imagen.
* Comprimir los datos de la imagen para que ocupen menos espacio.
* Reducción de colores (dithering)

El principio del dithering se basa en la reducción del número de colores usado en una imagen, al considerar que en la mayoría de los casos se utiliza demasiada información gráfica en un fichero, información que se puede eliminar sin pérdidas notables en la calidad final de la imagen.


<div align="center">
![](http://i.imgur.com/ZFP1Y7f.jpg)
</div>
<br>

Si una determinada imagen utiliza sólo 40 colores, para reducir el tamaño de su archivo bastaría con definir los 40 colores utilizando una paleta de color, guardando luego los puntos de la imagen con una profundidad de 8 bits.

Por otra parte, una imagen que utilice 256 colores puede tener una calidad aceptable en relación a la misma imagen con 16,8 millones de colores, siendo, su tamaño tres veces más pequeño. Para obtener un color no presente en la paleta de 256 colores de la imagen siempre es posible mezclar los que sí están, consiguiendo en la mayoría de los casos una buena aproximación al necesitado.

<div align="center">
![](http://i.imgur.com/0n33NnE.jpg)
</div>
<br>

La técnica del dithering va a ser la encargada de calcular la proporción con que se deben mezclar los colores de la paleta para obtener otros.

Para obtener una determinada tonalidad de color se utilizan varios puntos que tienen un color muy próximo al que se desea conseguir. Cuando se observar la imagen desde una cierta distancia, el color de los puntos adyacentes se mezcla, dando lugar a la ilusión de nuevas tonalidades de color.

Este sistema de optimización por reducción de colores es utilizado por ejemplo en el formato GIF.

#### Reducción de datos (compresión)

La compresión es una técnica que permite reducir el tamaño de un fichero mediante procesos matemáticos, facilitando así la transferencia de los mismos por red o su almacenamiento en cualquier otro soporte.

Todas las técnicas de compresión reducen la cadena de código binario de una imagen sin comprimir a una forma abreviada matemática basada en complejos algoritmos, apoyándose en la teoría de que en una imagen existe información repetida que en realidad sólo se debe guardar una vez.

<div align="center">
![](http://i.imgur.com/Ueeisyj.jpg)
</div>
<br>

Los algoritmos matemáticos que el ordenador emplea para generar la compresión son muy variados y los hay realmente complejos. Algunos valen para todo tipo de imágenes y otros son eficaces solamente con un tipo de ellas.

Existen dos tipos básicos de algoritmos de compresión, los que actúan sin pérdidas y los que comprimen con pérdidas.

Los **sistemas sin pérdida** abrevian el código binario sin desechar información, por lo que los datos de salida de la decodificación son idénticos bit a bit a los de la fuente original. Los factores de compresión conseguidos son pequeños, menores de 10:1 en el mejor de los casos, no pudiéndose garantizar un factor de compresión determinado, ya que depende de la cantidad de redundancia de la información original . Estos sistemas se suelen usar en el escaneado bitonal de material de texto.

Los **sistemas con pérdida** utilizan diferentes formas de compensar o desechar la información menos importante de una imagen basándose en la percepción visual humana, consiguiendo a veces resultados casi idénticos al original con un peso mucho menor. La calidad de la imagen no sólo depende del factor de compresión, sino también del algoritmo empleado. Los factores de compresión son altos, de 40:1 a 100:1

Se suelen utilizar con imágenes tonales, particularmente con imágenes de tono continuo, en las que la simple abreviatura de información que proporcionan los sistemas sin pérdida no tienen como resultado un ahorro de archivo apreciable.

Existe una variación de los sistemas de compresión, los sistemas emergentes, que ofrecen la capacidad de proporcionar imágenes de resolución múltiple desde un solo archivo, con la consiguiente flexibilidad en la entrega y presentación de las imágenes a los usuarios finales.

**Los principales algoritmos de compresión usados en ficheros gráficos son:**

#### RLE (Run Length Encoded)

Es tal vez el esquema de compresión sin pérdidas más sencillo, y también uno de los más ineficaces. Está basado en sustituir la información gráfica de píxeles que se repiten por el valor del color de uno de ellos y la posición de cada uno de los puntos que lo utilizan.

Esta técnica es eficiente cuando dentro del fichero gráfico que se va a comprimir se repite un byte sucesivamente un número grande de veces. En estos casos, todos los bytes iguales se sustituyen por dos, el primero de los cuales indica el numero de veces que se repite el segundo.

<div align="center">
![](http://i.imgur.com/6YImSkv.gif)
</div>
<br>

Existen diferentes formas de implementar RLE, todas ellas patentadas. Una de ellas, la más ineficiente, es utilizar un carácter, llamado comúnmente DLE, que sirva para indicar que se ha producido una repetición de un carácter. Otra es utilizando un carácter "centinela", con un bit que indica si la siguiente información es acerca de una repetición o son datos sin repetición.

Este método permite obtener un alto nivel de compresión en imágenes que contengan muchas áreas del mismo color, sin que se produzcan pérdidas de calidad. El problema surge cuando los colores de la imagen son muy dispares, caso en el que se pueden obtener archivos de mayor tamaño que los originales.

RLE es el algoritmo utilizado en los formato gráficos BMP y PCX, aunque cada uno usa un método distinto de implementación.

#### LZW (Lempel-Ziv-Welch)

Sistema de compresión sin pérdidas, actualmente propiedad de la empresa Unisys, desarrollado por los matemáticos Abraham Lempel y Jakob Ziv en los años 1977 y 1978, y refinado por Terry Welch en1984.

Este algoritmo surgió con objeto de que todas las personas de la empresa Compuserve pudieran intercambiar de forma rápida imágenes en formato gráfico GIF, independientemente de la plataforma usada.

<div align="center">
![](http://i.imgur.com/yrylqTG.jpg)
</div>
<br>

LZW es un compresor tipo diccionario, que utiliza para la compresión una tabla de cadenas, reemplazando las cadenas de caracteres iguales del fichero por códigos numéricos únicos que las representan, con lo que es capaz de comprimirlas aunque no se encuentre en sucesión. En el fichero comprimido no aparece explícitamente la tabla de cadenas, sólo la tabla de caracteres individuales y el conjunto de todos los códigos generados. De esta forma se consiguen niveles de compresión máxima de 2:1

Este sistema es recomendable para comprimir ficheros que contengan muchos datos repetidos, como imágenes sencillas, monocromáticas o que contengan áreas de color de gran tamaño, siendo utilizado en los formatos TIFF, GIF y JPG-LS, así como en archivos de lenguaje PostScript.

#### JBIG (Joint Bi-level experts Image Group)

Sistema de compresión sin pérdidas muy robusto para imágenes bi-nivel (en blanco y negro), que opera tanto en modo secuencial como en modo progresivo.

Cuando se decodifica una imagen codificada progresivamente, inicialmente se dispone de una imagen de baja resolución con respecto a la original, imagen que va aumentando su resolución conforme más datos son decodificados.

<div align="center">
![](http://i.imgur.com/ioII0dx.jpg)
</div>
<br>

La codificación progresiva presenta varios beneficios. En primer lugar, una misma base de datos de imágenes puede servir a diferentes dispositivos de salida con resoluciones distintas. Solamente aquella información en el archivo imágenes comprimidas que permita la reconstrucción a la resolución del dispositivo de salida en particular necesita ser enviado y decodificado. En segundo lugar, permite que una imagen de baja resolución sea rápidamente transmitida y mostrada, con el mejoramiento de la resolución deseado. En tercer lugar, permite al usuario un rápido reconocimiento de la imagen, lo que hace posible que pueda interrumpir la transmisión de una imagen indeseada.

Este sistema es el usado en el formato gráfico TIFF, no siendo soportado por ningún navegador web actual.

#### JPEG (Joint Photograph Expert Group)

Sistema de compresión con pérdidas muy perfeccionado, basado en estudios de la percepción visual humana, que permite codificar imágenes en color (24 bits) y en escala de grises (8 bits) mediante la eliminación de datos redundantes que no son importantes y el suavizado de los bordes y áreas que tienen un color similar.

Con ello se producen pérdidas que degradan levemente la calidad de la imagen, pero a cambio proporciona altos índices de compresión, ajustables a la calidad final de la imagen que se desea codificar.

<div align="center">
![](http://i.imgur.com/wTIfOJs.jpg)
</div>
<br>

En realidad, JPEG, estándar internacional 10918, describe una familia de técnicas de compresión basadas en complejas operaciones matemáticas, como conversión del formato de color, transformación separada del coseno (DCT), cuantizaciones y codificación entrópica, definiendo tres sistemas diferentes de codificación:

* Un sistema de codificación básico, con pérdidas, que se basa en la Transformada Discreta del Coseno y es apropiado para la mayoría de las aplicaciones de compresión. la precisión de los datos de entrada y de salida está limitada a 8 bits.
* Un sistema de codificación extendida, para aplicaciones de mayor compresión, mayor precisión, o de reconstrucción progresiva. se usa principalmente para proporcionar decodificación parcial rápida de una imagen comprimida, para que la apariencia general de esta pueda determinarse antes de que se decodifique totalmente.
* Un sistema de codificación independiente sin pérdidas, para la compresión reversible.

JPEG es un algoritmo de codificación simétrico (decodificar lleva tanto tiempo como codificar), que ofrece niveles de compresión de 20:1 o mayores, permitiendo realizar ciertas transformaciones geométricas (por ejemplo, rotación de imagen) directamente en la matriz transformada, sin regenerar la imagen original.

Es el método de compresión más utilizado actualmente para la compresión de imágenes con pérdida, siendo usado en los formatos gráfico JPG, TIFF, FlashPix, en ficheros PDF y en archivos de lenguaje PostScript. Además, es la base del estándar multimedia para imágenes en movimiento, MPEG.

En cuanto a los navegadores web, es soportado desde Internet Explorer 2 y Firefox en todas sus versiones. Por supuesto también en navegadores más modernos como Chrome.

# Gráficos vectoriales
<br>

La palabra vector tiene distintos significados dependiendo el contexto en el que se maneje: matemáticas, geometría, física, en el caso del diseño y la ilustración por computador define la forma en que un gráfico o imagen puede ser producido y representado; así un gráfico vectorial es toda imagen digital formada por diferentes objetos geométricos independientes. Cada uno de estos elementos definido por parámetros matemáticos como la forma, posición, color, el tipo y grosor de contorno, etc.

Los gráficos vectoriales son en su formato completamente distintos a los gráficos de mapas de bits o también llamados matriciales, los cuales están constituidos por pixeles.

Los gráficos vectoriales, también conocidos como gráficos orientados a objetos, son el segundo gran grupo de imágenes digitales. Son más simples que los gráficos de mapas de bits, ya que en ellos las imágenes se almacenan y representan por medio de trazos geométricos controlados por cálculos y fórmulas matemáticas, tomando algunos puntos de la imagen como referencia para construir el resto.

Los vectores tienen la ventaja sobre los pixeles de ser escalables, es decir, se puede aumentar su tamaño conservando su calidad original. Lo que no ocurre con los gráficos a base de pixeles que presentan degradación de la calidad al aumentar el tamaño.

<div align="center">
![](http://i.imgur.com/b9StCRv.jpg)
</div>
<br>

Otra diferencia importante entre estos dos tipos de imágenes digitales es el peso, los vectoriales por ser solamente parámetros matemáticos, suelen ser mucho menos pesados que una imagen rasterizada o de pixeles. De la misma manera los gráficos vectoriales pueden ser transformados (estirar, rotar, mover, distorsionar) de una manera más sencilla y con menos requerimientos de memoria en el equipo.

Sin embargo todos los gráficos vectoriales o vectorizados tienen que ser transformados a pixeles cuando se presentan en una pantalla o cuando se requiere su impresión.

-------- 

### Principales aplicaciones
<br>

**Diseño animación e ilustración**
En la actualidad, muchos ambientes de tercera dimensión son compuestos por gráficos vectoriales que conforman distintos tipos de aplicaciones. También son ampliamente utilizados para animaciones 2D en diseño web por su facilidad de uso y su bajo peso.

**Documentos digitales**
Permiten la descripción grafica de un documento digital, sin la pérdida de calidad de la imagen por aplicaciones o transformaciones de forma.

**Videojuegos**
Utilizados generalmente en la producción de ambientes virtuales de tres dimensiones.

**Tipografía**
Las fuentes son archivos tipográficos que utilizan en la mayoría de las ocasiones imágenes vectoriales. Algunos de los formatos más conocidos son TrueType, OpenType y PostScript.


-----



### Principales formatos de los gráficos vectoriales:

* **SWF Adobe flash:** utilizado para gráficos y animaciones 2D para internet.
* **AI Adobe Ilustrator:** Para gráficos e ilustración para web e impresión.
* **CDR Corel Draw:** Utilizado generalmente para diseño y autoedición para impresos.
* **PDF Adobe Acrobat:** Para intercambio de documentos y flujos de trabajo.
* **Post Script:** Generalmente se utiliza en impresión e intercambio de archivos.

Es importante resaltar que las fotografías no pueden ser vectorizadas sin un pérdida considerable de calidad en la imagen; por lo que en este caso sigue siendo recomendable el uso formatos de pixeles (jpeg, png, tiff, etc.).

# Formatos gráficos en general y nativos de aplicaciones de diseño

El almacenamiento de los datos que componen una imagen digital en un archivo binario puede realizarse utilizando diferentes formatos gráficos, cada uno de los cuales ofrece diferentes posibilidades con respecto a la resolución de la imagen, la gama de colores, la compatibilidad, la rapidez de carga, etc. 

La finalidad última de un formato gráfico es almacenar una imagen buscando un equilibrio adecuado entre calidad, peso final del fichero y compatibilidad entre plataformas. Para ello, cada formato se basa en una o más técnicas diferentes, que pueden incluir codificación especial, métodos de compresión, métodos de dithering, etc. 

Generalmente, todo fichero gráfico comienza con una cabecera (header) de estructura variable, que indica al programa que lo solicite las características de la imagen que almacena (tipo, tamaño, resolución, modo de color, profundidad de color, número de colores de la paleta si la hay, etc). 

<div align="center">
![](http://i.imgur.com/pH1jWqX.gif)
</div>
<br>

A continuación se encuentran los datos propios de la imagen, generalmente comprimidos con un algoritmo específico de ese formato, que contienen información sobre el color de cada píxel de la imagen (mapas de bits) o una tabla con las características propias de cada objeto (gráficos vectoriales). En caso de usarse una paleta de colores, la información sobre dicha paleta también deberá estar contenida en el fichero. 

La imagen puede estar formada por un número diferente de píxeles, dependiendo de su tamaño y resolución, y tener más o menos colores. En función del número de píxeles y del número de colores la imagen tendrá más o menos calidad, pero cuanto más calidad tenga, más ocupará el fichero necesario para almacenarla. En el caso de los gráficos vectoriales no se definen píxeles individuales, dependiendo la calidad y el peso final del formato concreto en que se almacenen. 

<div align="center">
![](http://i.imgur.com/6JOIWey.gif)
</div>
<br>

Los ficheros gráficos de mapas de bits contienen pues una cabecera, los datos de los píxeles (generalmente comprimidos) y la paleta de colores (salvo si se usan 24 bits por píxel, caso en el que no es necesaria ninguna paleta). Los ficheros vectoriales, una cabecera y una tabla con las características de cada vector componente del gráfico. 

Por otra parte, con el paso del tiempo los ficheros gráficos almacenados en nuestro equipo se hacen cada vez más numerosos, haciéndose necesaria una estrategia de gestión de los mismos para conseguir establecer un cierto orden que nos permita saber en todo momento cuántos ficheros tenemos, de qué clase y qué tipo de información contiene cada uno de ellos. 



-----

## Formatos nativos aplicaciones de diseño gráfico

#### AI (.ai) 

El metaformato AI (Adobe Ilustrator) es el utilizado por el programa Adobe Ilustrator para guardar sus ficheros gráficos nativos. 

<div align="center">
![](http://i.imgur.com/UO9MzeW.gif)
</div>
<br>


Los ficheros AI admiten cabecera de previsualización (thumbnail) y pueden trabajar con vectores y mapas de bits. Permiten texturas, degradados, fotos integradas o vinculadas a ficheros externos, textos trazados o con fuentes incluidas y manejo de capas y máscaras. 

Suele producir ficheros de peso medio, dependiendo del contenido, pero se puede rebajar ya que admite algoritmos de compresión sin pérdidas. 

Es un formato muy popular, válido para PC y MAC, apto para intercambiar gráficos entre diferentes aplicaciones, pero teniendo siempre en cuenta la versión de Ilustrator que creó el archivo original, ya que deben de ser versiones compatibles. 

#### CDR (.cdr) 

CDR (Corel Draw) es el formato nativo del programa de gráficos vectoriales Corel Draw, siendo válido para PC y MAC. 

<div align="center">
![](http://i.imgur.com/1jrR4UZ.gif)
</div>
<br>

Es un formato vectorial, pero admite la inclusión de elementos de mapa de bits (integrados o vinculados a ficheros externos), pudiendo llevar además cabecera de previsualización (thumbnail). Junto a AI es uno de los formatos con más posibilidades con respecto al color, a la calidad de los diseños y al manejo de fuentes, pudiendo contener los textos trazados o con fuentes incluidas. 

Una de las principales desventajas de este formato es su falta de compatibilidad con el resto de aplicaciones gráficas, al ser éstas incapaces de almacenar imágenes bajo este formato. 

#### DXF (.dxf) 

El formato DXF (Drawing Interchange Format) es un formato vectorial que la empresa Autodesk lanzó para permitir el intercambio de archivos de dibujo entre los diferentes programas de CAD. Soporta hasta 256 colores (8 bits). 

<div align="center">
![](http://i.imgur.com/3OiFo7Q.gif)
</div>
<br>

Existen dos versiones de DXF (ASCII y binario), que no utilizan ningún algoritmo de compresión. Los ficheros de la versión ASCII contienen números y órdenes a realizar escritos en codificación ASCII, por lo que pueden ser abiertos y leídos con cualquier editor de texto, como el Notepad de Windows. Esta información indica la ubicación de puntos flotantes matemáticos o floating points, utilizados para exhibir la imagen en pantalla. Este sistema, más lento que el de otros formatos, requiere hardware avanzado para poder funcionar correctamente. 

Los ficheros en formato DXF son reconocidos por la mayoría de sistemas CAD y por algunos programas de diseño gráfico vectorial, como Corel Draw y Adobe Ilustrator, que pueden manejarlo sin mayores dificultades. 

No son soportados por ningún navegador web. 


#### DRW (.drw) 

Formato grafico vectorial usado por diferentes programas que funcionan bajo DOS y Windows, como Micrografx Designer o Windows Draw. Los gráficos .drw pueden ser incluidos en presentaciones creadas con PowerPoint, en diagramas de Microsoft Visio 2000 o en documentos de Microsoft Word. 

<div align="center">
![](http://i.imgur.com/g7PvdQx.jpg)
</div>
<br>

No es soportado por ningún navegador web. 

#### EMF (.emf) 

EMF (Enhanced MetaFile) es un metaformato gráfico vectorial de 32 bits, reconocido por casi todas las aplicaciones de diseño gráfico y compatible con los sistemas operativos Windows, pudiendo ser usado en las aplicaciones del paquete Office. 

<div align="center">
![](http://i.imgur.com/Ziuh8kN.gif)
</div>
<br>

Junto a las características propias de los formatos vectoriales presenta la ventaja adicional de que sus ficheros pueden ser creados rápidamente, ya que lo que se encola en la impresora son comandos de dibujo, con lo que se puede evitar la sobrecarga en el caso de impresión remota de ficheros gráficos. 

Además, este formato es más eficiente porque genera un archivo relativamente pequeño y genérico, que es compatible con todas las impresoras. 

Como desventaja, los archivos de formato EMF no contienen la misma cantidad de detalles que los de otros tipos de formatos gráficos vectoriales, como los archivos DWF. 

Por lo que respecta a la web, es soportado por Internet Explorer, aunque hay algunos gráficos que no son interpretados correctamente. 

#### FH10 (.fh10) 

Formato nativo del programa de gráficos vectoriales Frenad 10, válido para PC y MAC. Puede llevar cabecera de previsualización (thumbnail) y se puede comprimir, dependiendo el tamaño final del contenido. 

<div align="center">
![](http://i.imgur.com/OykOXkN.gif)
</div>
<br>

Puede llevar las fotos integradas o vinculadas a ficheros externos y textos trazados o con fuentes incluidas. 

Es posible importarlo a diferentes programas gráficos, como Macromedia Flash o Adobe Ilustrator, pero no es soportado por ningún navegador web. 

#### PCX (.pcx) 

PCX es el formato nativo del programa gráfico PC Paintbrush, de la empresa Z-Soft. Es uno de los formatos de mapa de bits más conocidos, que soporta en sus últimas versiones imágenes de hasta 24 bits en color (unos 16,8 millones de colores), no presentando limitaciones respecto al tamaño de las imágenes. 

<div align="center">
![](http://i.imgur.com/hBsOjdc.gif)
</div>
<br>

Usa un algoritmo de compresión RLE de codificación sencilla y alta velocidad de descompresión, orientado más a la rapidez de acceso que a la reducción de tamaño de los archivos. 

Su principal ventaja es la compatibilidad, ya que multitud de aplicaciones gráficas lo soportan (la gran mayoría de los programas de desktop publishing y de tratamiento de imágenes), siendo utilizado por las aplicaciones de dibujo de Windows. 

Actualmente está en desuso en el campo multimedia, pero no así en el terreno profesional, donde se sigue utilizando con frecuencia. 

#### PIC (.pic) 

PIC es un formato utilizado en muchas aplicaciones gráficas que funcionan bajo MS-DOS y Windows, como PC Paint y Pictor. 

<div align="center">
![](http://i.imgur.com/KJv2yff.gif)
</div>
<br>

Este formato puede almacenar una imagen de mapa de bits con dos posibilidades: 256 colores a una resolución máxima de 320 x 200 píxeles y 16 colores a una resolución de 640 x 480 píxeles. También puede almacenar una secuencia de imágenes en cada fichero, siendo en este caso sólo posible imágenes en tonos de gris. 

Los datos de la imagen en el fichero vienen expresados como una matriz de bytes sin comprimir, en la que se almacena por filas el valor de los píxeles de la imagen o imágenes que lo forman. 

Hay que tener mucho cuidado al manejar ficheros con extensión .pic, ya que es utilizada por diferentes programas gráficos que producen ficheros incompatibles entre sí, como Lotus 1-2-3, Dr-Halo y Micrografx. 

Las principales desventajas de este formato son la escasez de colores posibles en altas resoluciones y la incompatibilidad entre formatos PIC, que hacen que sea uno de los menos utilizados en la actualidad. 

#### PSD (.psd) 

PSD (Photoshop Digital Format) es el formato de mapa de bits (aunque con funcionalidades avanzadas) nativo del programa de tratamiento de imágenes Adobe Photoshop, válido para MAC y PC. 

Es un formato sin compresión, por lo que no produce pérdidas de calidad, y admite todos los Modos de Color, canales alfa, tintas Planas, guías, trazados, selecciones, textos, capas simples y de ajuste y máscaras. 

<div align="center">
![](http://i.imgur.com/TYAYwEe.gif)
</div>
<br>

Soporta hasta 32 bits de profundidad de color en cualquier modo de color, produciendo imágenes de alta calidad que se pueden exportar, sin pérdida de calidad, a programas de auto edición y diseño como PageMaker, QuarkXpress, Ilustrator, etc. Incluso existen programas como CorelDraw que pueden abrir ficheros PSD manteniendo la estructura de capas original. 

#### TGA (.tga) 

El formato TGA (TrueVision Targa) es un formato gráfico de mapa de bits desarrollado por la empresa Truevision para las tarjetas Targa y Vista, válido para PC y MAC, que permite guardar imágenes monocromáticas (2 bits) y con diferentes niveles de profundidad de color (8, 16, 24 y 32 bits), utilizando o no una paleta gráfica. Puede trabajar en Escala Grises, Color Indexado, RGB (16 y 24 bits sin canales alfa) y RGB de 32 bits (un solo canal alfa). 

<div align="center">
![](http://i.imgur.com/pUhrRjq.jpg)
</div>
<br>

Permite almacenar los archivos comprimidos o sin comprimir, aunque la mayoría de programas que lo soportan solo pueden abrir archivos TGA sin compresión, siendo entonces el que el peso de los ficheros es muy elevado. 

Este formato está especialmente indicado para retocar diseños profesionales que se vayan a reproducir en pantalla, debido a que la amplia gama de colores produce un efecto muy realista y sumamente elaborado. También es muy útil cuando se trabaja con escáneres de alta calidad y para la exportación de imágenes a edición profesional vídeo. Sin embargo, en impresión es poco usado, ya que con profundidades de color de 16 bits o menos las imágenes pierden detalles. 

Las principales desventajas de este formato son el tamaño de los archivos, que ocupan bastante más espacio que otros formatos de igual calidad, y que no guarda muchos detalles a veces necesarios, como la resolución que soporta. 

#### TIFF (.tif / .tiff) 

El formato TIFF (Tagged Image File Format) es un formato de mapa de bits desarrollado por Aldus Corporation capaz de almacenar imágenes en blanco y negro (1 bit), escala de grises (9 bits), RGB (24 bits), CMYK (32 bits) con más de diez técnicas de compresión disponibles (sin compresión, LZX, JPEG, MAC Packbit, etc.) y Color Lab. 

Soporta el algoritmo de compresión sin pérdidas LZW, almacenando las imágenes en una serie de bloques que pueden contener información sobre la imagen en sí, su tamaño, su manejo del color, información a las aplicaciones que utilicen ese archivo, texto e incluso una miniatura (thumbnail), pequeña representación de la imagen, a la cual el programa accede rápidamente y no pierde tiempo descomprimiendo toda la imagen. 

<div align="center">
![](http://i.imgur.com/lA5aSSq.jpg)
</div>
<br>

Es válido para PC y MAC, siendo soportado por multitud de programas gráficos de pintura e ilustración, por lo que es muy utilizado para intercambiar archivos entre diferentes aplicaciones y plataformas. 

Es uno de los formatos más utilizados en artes gráficas, así cómo en fotografías en las que queremos que no haya ninguna perdida, bien para imprimirla o bien para interpolarla para aumentar su resolución. También es el formato más usado cuando se trabaja con escáneres, debido a su útil manejo del color. 

Como desventajas, no tiene soporte para vectores ni texto, por lo que todos los tipos deben ser convertidos a mapas de bits antes de aplicarse al archivo. También, que debido a la flexibilidad que presenta respecto a los sistemas de compresión y a la compatibilidad entre aplicaciones, los programas diseñados para leer archivos TIFF deben disponer de la misma flexibilidad para entender los datos contenidos en ellos, lo que desafortunadamente no siempre ocurre. 

#### WMF (.wmf) 

WMF (Windows MetaFile Format) es un metaformato de 16 bits de los sistemas operativos Windows, siendo un estándar de intercambio de gráficos entre las diferentes aplicaciones Microsoft (Word, Excel, Access, etc.). 

<div align="center">
![](http://i.imgur.com/yYk6u7F.jpg)
</div>
<br>

WMF es un formato vectorial (aunque no basado en curvas de Bézier) y escalable, que funciona copiando en un archivo los comandos para realizar la imagen en cuestión, ahorrando con ello una cantidad considerable de espacio. Teóricamente puede almacenar cualquier elemento gráfico, ya sean imágenes bitmap, textos o gráficos vectoriales complejos. 

Gracias a su facilidad de manejo, hay muchas aplicaciones que lo utilizan en la actualidad, siendo compatible con la mayoría de programas vectoriales. Con la aparición del sistema operativo Windows 95 se creó un nuevo formato, EMF, que ampliaba las capacidades del WMF.

# Formatos gráficos para las imágenes de la web


-----



#### GIF (.gif)

El formato GIF (Graphic Interchange Format) es uno de los más habituales en imágenes de mapa de bits. 

El formato GIF (Graphic Interchange Format, Formato de intercambio de gráficos) es un formato de archivos de gráficos de mapa de bits (una trama) desarrollado por Compuserve.

Existen dos versiones de este formato de archivos desarrolladas en 1987 y 1989 respectivamente:

* El GIF 87a, que es compatible con la compresión LZW, puede entrelazar, (permitir la visualización progresiva) una paleta de 256 colores y tiene la posibilidad de crear imágenes animadas (llamadas GIF animados) almacenando varias imágenes en el mismo archivo.
* El GIF 89a, que tiene como agregado la posibilidad de designar un color transparente para la paleta y especificar el tiempo de las animaciones.

**Características del formato GIF**

Una imagen GIF puede contener entre 2 y 256 colores (2, 4, 8, 16, 32, 64, 128 ó 256) entre 16,8 millones de su paleta. Por lo tanto, dado que la paleta tiene un número de colores limitado (no limitado en cuanto a colores diferentes), las imágenes que se obtenían con este formato por lo general eran muy pequeñas.

Sin embargo, dado que el algoritmo de compresión LZW estaba patentado, todos los editores de software que usaban imágenes GIF debían pagarle regalías a Unisys, la compañía propietaria de los derechos. Esta es una de las razones por las que el formato PNG se está volviendo cada vez más popular, en perjuicio del formato GIF.

La gran ventaja de los archivos GIF no es pues su gran resolución, su calidad ni su precisión, sino su portabilidad, su facilidad de transmisión y además y sobre todo, su compatibilidad. Casi todos los dispositivos del mercado permiten usar estos gráficos, sin necesidad de tener que convertirlos, lo que como hemos dicho, facilita su uso. Otra ventaja bastante importante es que actualmente es un formato totalmente gratuito, al haber expirado la patente del formato de compresión LZW, que obligaba a pagar a los autores un canon por usarlo para crear imágenes. Es por ello que hoy en día puedes encontrarte millones de GIFs libres por la web.
<br>

#### JPEG (.jpg / .jpeg)

JPEG es, junto con GIF, uno de los formatos estándares en las páginas web, lo que ha hecho que su uso se haya disparado enormemente. Sus ficheros son válidos tanto para PC como para MAC, es soportado por los navegadores más importantes (Internet Explorer y Netscape Navigator) y puede trabajar en Escala de grises, RGB y CMYK. 

<div align="center">
![](http://i.imgur.com/vvoKq4p.jpg)
</div>
<br>

Este formato de mapa de bits fue desarrollado por el Joint Photographic Experts Group, asociación de fotógrafos profesionales de Estados Unidos que buscaba un formato gráfico que permitiera el almacenamiento de imágenes fotográficas de calidad con unos pesos de fichero configurable y relativamente bajo. 

JPEG es un formato comprimido de imagen digital que ocupa poco espacio en comparación con la misma imagen sin comprimir, se usa en todas las cámaras de fotos y en las páginas web; su principal ventaja es el espacio que ahorra, su principal defecto es la pérdida de calidad.
<br>

#### PNG (.png)

El formato PNG (Portable Network Graphic) es un formato de mapa de bits de libre distribución, válido para PC y MAC, desarrollado para su uso en la web como alternativa a los formatos GIF y JPG, sobre todo al primero de ellos, propiedad de la empresa Unisys Corporation, más simple. 

<div align="center">
![](http://i.imgur.com/Djrsvkv.jpg)
</div>
<br>

PNG utiliza un esquema de compresión sin pérdidas para reducir el tamaño del archivo, manteniendo intacta la calidad original de la imagen. 

Puede trabajar en modo Escala de Grises (con un canal alfa), en modo Color Indexado (8 bits, hasta 256 colores, paletas de colores) y en modo RGB (24 bits, 16,8 millones de colores y 48 bits, con 24 bits para canales alfa), por lo que admite 256 niveles de transparencia. 

Las transparencias conseguidas con PNG son de mayor calidad que las puede conseguir el formato GIF, ya que, al trabajar con muchos más colores, genera transparencias de fondo sin bordes dentados. 

También permite imágenes entrelazadas (de visualización progresiva) y detección de errores, pero no implementa animaciones, punto en el que se encuentra en desventaja respecto al formato GIF. 

**Características del formato PNG**

El formato PNG permite almacenar imágenes en blanco y negro (una profundidad de color de 16 bits por píxel) y en color real (una profundidad de color de 48 bits por píxel), así como también imágenes indexadas, utilizando una paleta de 256 colores.

Además, soporta la transparencia de canal alfa, es decir, la posibilidad de definir 256 niveles de transparencia, mientras que el formato GIF permite que se defina como transparente sólo un color de la paleta. También posee una función de entrelazado que permite mostrar la imagen de forma gradual.

La compresión que ofrece este formato es (compresión sin pérdida) de 5 a 25% mejor que la compresión GIF.

Por último, el PNG almacena información gama de la imagen, que posibilita una corrección de gama y permite que sea independiente del dispositivo de visualización. Los mecanismos de corrección de errores también están almacenados en el archivo para garantizar la integridad.

# Elección y optimización del formato gráfico


-----

### Elección del formato gráfico más adecuado

Disponiendo de diferentes formatos gráficos para incluir en nuestras páginas web, cabe preguntarse cuál de ellos es el más apropiado. La respuesta a esta pregunta no es simple ni única, ya que depende de qué tipo de imagen contenga el fichero. 

Los formatos de mapa de bits más usados son JPEG (.jpg), GIF (.gif) y PNG (.png). Si comparamos la calidad obtenida por cada uno de ellos y el peso del fichero resultante en el caso de una imagen con muchos colores y gradaciones, como una fotografía, los resultados son los siguientes: 

<div align="center">
![](http://i.imgur.com/8eyy9l7.jpg)
GIF - 16,6 K      	JPG - 15,8 K      	BMP - 132 K    	PNG - 25,6 K 
</div>
<br>

Vemos que la mejor calidad y el menor peso en este tipo de imágenes corresponde al formato JPEG. Le sigue en peso el formato GIF, aunque la calidad de la imagen en muy baja, debido a que este formato sólo puede trabajar con 256 colores. El formato PNG da buena calidad, pero un peso mucho mayor, mientras que el formato BMP da un peso enorme, lo que lo hace poco recomendable para la web. 

Si ahora cogemos una imagen con pocos colores y gradaciones, los resultados cambian: 

<div align="center">
![](http://i.imgur.com/0nZ3JvC.gif)
</div>
<br>

En este caso es el formato GIF el que da menos peso, con una calidad más que aceptable, mientras que el formato BMP sigue siendo el más pesado, sin aumento de calidad apreciable. El formato JPEG da buenos resultados también, pero presenta varios inconvenientes en este tipo de imágenes, sobre todo si llevan textos, ya que crea difuminados alrededor de los mismos que desmejoran la imagen. Por su parte, PNG da mayores pesos, que aumentan en relación al número de colores de la imagen y al tamaño de la misma. 

**En cuanto a gráficos vectoriales, disponemos para su uso en la web de los formatos SWF y SVG.** 

Sin lugar a dudas, actualmente el premio se lo lleva SWF, entre otras cosas porque se ha hecho muy popular, es soportado por los navegadores más importantes, almacena imágenes de alta calidad en ficheros de poco peso y permite presentar en las páginas web vistosas y útiles animaciones interactivas, que en las últimas versiones del formato permiten la implementación de formularios, la interacción con código de servidor y el uso del lenguaje XML. 

En cuanto a SVG, actualmente se encuentra en fase de desarrollo y sus aplicaciones reales a la web quedan muy limitadas por factores como el escaso soporte por parte de los navegadores y la necesidad de instalación de un plugin no muy conocido que ocupa mucho espacio (sobre 4 Mb). Sin embargo, es un formato recomendado por el W3C como futuro estándar para gráficos vectoriales destinados a la web, permite crear animaciones interactivas y presenta una total integración con XML, por lo que es de esperar que en un futuro no muy lejano sea una verdadera alternativa libre al formato SWF (que es propiedad de Macromedia, dueña absoluta por ahora de su desarrollo).

### Optimización de un fichero gráfico

La preparación de imágenes para la web exige algunas precauciones cuando se parte de una imagen escaneada o cualquier otro tipo de imagen con alta resolución. Debemos tener presente que la resolución del monitor es aproximadamente de sólo 72dpi (puntos por pulgada). Si escaneamos a 300 dpi, estamos obteniendo imágenes que serán innecesariamente grandes y que no se verán en absoluto mejor que la imagen adquirida al mínimo de resolución. Una imagen mastodóntica puede tardar una eternidad en descargarse, ocupará espacio innecesario en vuestro servidor y probablemente los visitantes no tengan paciencia para esperar.

Uno de los errores más comunes en los principiantes al incluir imágenes es el tomarlas directamente del escaner y simplemente escalarlas al tamaño que desean en el programa de edición de páginas. La solución es muy sencilla; en el programa de tratamiento de imágenes, buscamos la opción que permita cambiar la densidad de la imagen (la resolución) o efectuar un nuevo muestreo (resample.) para ajustar el tamaño a la resolución de pantalla.

Después de preparar los ficheros para las páginas web, debe guardarse siempre una imagen original con el tamaño, resolución y número de colores necesarios para podrla manipular sin limitaciones. Si queremos recuperar toda esta informaciòn después de alterar la imagen para optimizarla en pantalla, pueden surgir todo tipo de imperfecciones. En pocas palabras, los "originales" deben guardarse en un formato que no pierda calidad, y que conserve íntegra la información de los colores. Para los ficheros de mapa de bits, sirven TIFF y BMP, y los formatos nativos de Photoshop, PaintShop Pro, Photopaint... para los ficheros vectoriales, no hay problema: basta con guardar en el formato original del programa (AI -EPS, FH-, CDR, XAR...)

Como norma general, una pagina completa no debe pesar más de 30 Kb - 40 Kb (la página inicial de Yahoo pesa unos 20 Kb). Se hace preciso pues controlar el número de imágenes incluidas en cada página y la realización de un proceso de optimización de los ficheros gráficos en el que, además de elegir el formato de almacenamiento más adecuado, se busque la relación calidad/peso más acertada. 

La mayoría de los programas gráficos de calidad ofrecen una herramienta para optimizar el peso de un fichero gráfico destinado a la web, mediante la que podemos fijar el peso del mismo, el número de colores que va a tener la imagen y si queremos que sea entrelazada, progresiva, con transparencias, etc. Deberemos buscar que las imágenes resulten con buena calidad y con el menor peso posible. El ensayo y la práctica son las bases para conseguir buenos resultados. 

<div align="center">
![](http://i.imgur.com/43A92f3.gif)
</div>
<br>

Si estamos manejando una imagen en formato GIF, el peso de ésta va asociado al número de colores que tenga, por lo que podemos jugar con la paleta de colores que asociemos a la imagen para variar su peso. El siguiente ejemplo muestra una imagen en formato GIF guardada con diferentes números de colores: 

Si estamos manejando una imagen en formato GIF, el peso de ésta va asociado al número de colores que tenga, por lo que podemos jugar con la paleta de colores que asociemos a la imagen para variar su peso. El siguiente ejemplo muestra una imagen en formato GIF guardada con diferentes números de colores: 

<div align="center">
![](http://i.imgur.com/wn65KEX.jpg)
</div>
<br>


Como vemos, la diferencia es evidente, y eso que hemos elegido una imagen con pocos colores. En caso de una imagen más compleja, las diferencias aumentan mucho más. 

Vamos a ver ahora el caso de una imagen en formato JPG, donde el peso no va a depender del número de colores, sino del porcentaje de compresión aplicado: 


<div align="center">
![](http://i.imgur.com/cD4ZSRL.jpg)
</div>
<br>

Al igual que en el caso anterior, hemos elegido una imagen que pierda poco con la compresión para que se aprecie la disminución que se puede conseguir a veces a costa de no perder mucha calidad. 

**En el caso de una imagen con muchos colores y gradaciones suaves, como una fotografía, se nota más la pérdida de calidad: **

<div align="center">
![](http://i.imgur.com/r40UYGr.jpg)
</div>
<br>

Donde vemos que de la calidad máxima a la media la pérdida de calidad no es excesiva, pero el peso baja considerablemente, mientras que el paso de calidad media a baja no disminuye mucho el peso, pero sí la calidad de la imagen. 

Otro factor a tener en cuenta es el tamaño físico de la imagen. A mayor tamaño, mayor peso en Kb. Debemos pues buscar un tamaño suficiente para que la imagen se vea bien, pero que no de un fichero de un peso excesivo.

# Otros formatos gráficos para web


-----
#### SVG (.svg)

SVG (Scalable Vector Graphic) es un nuevo formato de gráficos vectoriales para la web desarrollado por el W3C con vistas a ofrecer a los desarrolladores un formato gráfico de alta calidad y totalmente integrado con los lenguajes HTML y XML. 

SVG maneja gráficos vectoriales que almacena mediante un lenguaje de etiquetas propio, semejantes a la que se utilizan en HTML, por lo que pueden ser editados y modificados con cualquier editor de texto simple. 

<div align="center">
![](http://i.imgur.com/djA2cUE.gif)
</div>
<br>

Podemos pues definir el formato SVG como un puente entre diseño gráfico y programación, entre arte y tecnología. Efectivamente, debido a su naturaleza puramente matemática, un gráfico SVG es una sucesión de objetos y puntos posicionados y orientados en el lienzo de trabajo, elementos que son definidos por fórmulas matemáticas y que pueden ser accedidos por código de programación para modificar sus propiedades. 

**Por ejemplo, el código para definir una elipse con fondo azul claro es el siguiente: **

```
<?xml version="1.0" standalone="no"?> 
<!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.0//EN" 
   "http://www.w3.org/TR/2001/REC-SVG-20010904/DTD/svg10.dtd"> 
<svg width="200" height="200"> 
    <ellipse cx="99" cy="100.5" rx="77" ry="35.5" style="fill:rgb(0,192,192);opacity:0.3"/> 
</svg>
```

Maneja 24 bits de profundidad de color, pudiendo además usarse en su definición cualquiera de los sistemas estándar (RGB, CMYK, etc.). 

Entre las ventajas del formato SVG podemos citar que trabaja con gráficos vectoriales editables, admiten curvas Bézier, transparencias, suavizados y rastrillados, admite textos editables y fuentes TrueType y Type 1, pueden incluir sonidos y etiquetas explicativas, permite la creación de animaciones en escala de tiempo y que es una tecnología de código libre, no propietaria, con las ventajas que eso representa para los desarrolladores. 
<br>

#### SWF (.swf)

SWF (Shockwave Flash) es el formato de salida del programa de gráficos vectoriales y animaciones Macromedia Flash, resultado de la compresión de los ficheros FLA de trabajo de esta aplicación. 

Su posibilidad de uso en las páginas web y su compatibilidad con los navegadores más comunes (previa instalación del plugin necesario, aunque los navegadores más importantes lo traen ya por defecto) ha revolucionado el mundo de la web, ya que es posible ofrecer a los usuarios unos gráficos vectoriales de calidad, que pueden ser escalados (cambiados de tamaño) sin pérdidas de calidad y que permiten al usuario interactuar con ellos, así como complejas animaciones basadas en fotogramas. 

Además, los ficheros SWF pueden ser visualizados independientemente de la web, en una ventana propia, permitiendo la construcción de verdaderas aplicaciones multimedia interactivas, como juegos, presentaciones, etc. 

El formato SWF produce ficheros de un tamaño verdaderamente reducido, sobre todo si las imágenes que contiene son de naturaleza vectorial, ya que no almacenan información píxel a píxel, sino fórmulas matemáticas. Incluso la interactividad de los objetos está definida mediante un lenguaje propio de script, Action Script), que apenas carga el fichero. No obstante, el tamaño aumentará mucho si se introducen en el fichero imágenes de mapa de bits. 

Dentro de un archivo SWF se pueden incluir elementos vectoriales y de mapa de bits, textos en fuentes escalables, sonidos y vídeos, pudiendo programarse acciones de respuesta a eventos y animaciones mediante código de script. 
<br>

#### BMP (.bmp)

BMP (Bitmapped File Format) es probablemente el formato de fichero para imágenes más simple que existe. Aunque teóricamente permite compresión (en imágenes de 4 y 8 bits puede usar RLE), en la práctica nunca se usa, guardando las imágenes descomprimidas, lo que significa mayor velocidad de carga pero también mayor peso del fichero gráfico. Admite de entrada cualquier tipo de resolución y profundidades de color de 1, 4, 8 y 24 bits. 

<div align="center">
![](http://i.imgur.com/w5aZOeA.jpg)
</div>
<br>

La estructura de los ficheros BMP es sencilla, estando formados por una cabecera que contiene las características generales de la imagen (tamaño, número de colores y paleta de colores si es necesaria) y por la información de la imagen en sí, píxel a píxel, de izquierda a derecha, comenzando desde la última línea inferior, motivo por el cual las imágenes en formato BMP se trazan en pantalla de abajo hacia arriba. 

BMP es un formato muy utilizado, válido para MAC y PC. Es el estándar de imagen de mapa de bits en sistemas operativos DOS y Windows e IBM OS/2, siendo usado habitualmente en aplicaciones como Word, Excel, PowerPoint, etc. Las versiones de Windows e IBM OS/2 son incompatibles entre sí, aunque hay programas gráficos, como Paint Shop Pro, que pueden trabajar con ambas. 

Sus principales ventajas son su sencillez y la calidad de la imagen. Su gran desventaja, el enorme tamaño de los ficheros. 

Es soportado tan solo por Internet Explorer.

# Photoshop: Espacio de trabajo, herramientas, capas. Tipos de imagen / color


-----

## Espacio de trabajo 

El espacio de trabajo de inicio de Photoshop le proporciona acceso rápido a sus archivos, bibliotecas y ajustes preestablecidos recientes. Según el estado de la suscripción, este espacio de trabajo también puede mostrar contenido adaptado a sus necesidades. También puede buscar el recurso adecuado de Adobe Stock para su proyecto, directamente desde el espacio de trabajo.

Photoshop muestra el espacio de trabajo de inicio al iniciarse o siempre que no haya ningún documento abierto.

A continuación mostramos el espacio de trabajo de inicio:

<div align="center">
![](http://i.imgur.com/9af2EWe.jpg)
</div>
<br>

### Un primer acercamiento al espacio de trabajo de Photoshop

<div align="center">
![](http://i.imgur.com/rRX7T0B.jpg)
</div>
<br>
**A:** Panel Herramientas |** B**: Panel Historia | **C:** Panel Color |** D:** Panel Bibliotecas de Creative Cloud | **E:** Panel Capas

### Descripción general del espacio de trabajo

* La barra Aplicación de la parte superior contiene un conmutador de espacio de trabajo, menús (solo en Windows) y otros controles de la aplicación. En ciertos productos para Mac, puede mostrarla u ocultarla con el menú Ventana.

* El panel Herramientas incluye utilidades para crear y editar imágenes, ilustraciones, elementos de página, etc. Las herramientas relacionadas están agrupadas.

* El panel de control de la barra de opciones muestra opciones específicas de la herramienta seleccionada en el momento. 

* La ventana Documento muestra el archivo en el que se trabaja. Las ventanas Documento se pueden organizar como fichas y, en ciertos casos, también se pueden agrupar y acoplar.

* Los paneles ayudan a controlar y modificar el trabajo. Los paneles se pueden agrupar, apilar o acoplar.

* El Marco de aplicación agrupa todos los elementos del espacio de trabajo en una ventana única e integrada que permite tratar la aplicación como una sola unidad. Si mueve el marco de aplicación o alguno de sus elementos o si cambia su tamaño, todos los elementos que integra responden en consecuencia para evitar su superposición. Los paneles no desaparecen si cambia de aplicación o si hace clic sin querer fuera de esta. Cuando trabaje con dos o más aplicaciones, puede colocarlas una al lado de la otra en la pantalla o en varios monitores.

Si está utilizando Mac y prefiere la interfaz de usuario libre tradicional, tiene la opción de desactivar Marco de aplicación. 

### Funciones para facilitar el uso

El espacio de trabajo de Photoshop es muy fácil de usar e incluye diversas opciones con este propósito:

* Distintos niveles de brillo: elija Edición > Preferencias (Windows) o Photoshop > Preferencias (Mac OS) y seleccione una muestra de Tema de color en la sección Interfaz.
* Pantallas en las imágenes: reciba información mientras usa sus herramientas favoritas. Las pantallas en las imágenes muestran dimensiones de selección, ángulos de transformación y mucho más. Para cambiar la posición de las pantallas, elija una opción en Mostrar valores de transformación en las preferencias de Interfaz. 
* Espacio de pantalla maximizada: haga clic en el botón situado en la parte inferior de la barra de herramientas para cambiar entre los modos de pantalla Estándar y Pantalla completa.


-----

## Herramientas

Cuando inicie Photoshop, el panel Herramientas aparece en la parte izquierda de la pantalla. Algunas herramientas de este panel cuentan con opciones que aparecen en la barra de opciones contextuales.

Puede expandir algunas herramientas con el fin de ver las que contiene ocultas. Un triángulo pequeño en el lateral inferior derecho del icono de herramienta indica la presencia de herramientas ocultas.

Para ver información sobre una herramienta basta con colocar el puntero sobre ella. En la información de herramientas que se muestra debajo del puntero aparece el nombre de la herramienta.

**Nota:** en Photoshop CS6, algunas herramientas estaban disponibles como parte de Photoshop Extended. Todas las funciones de la antigua oferta de Photoshop Extended ahora forman parte de Photoshop CC. Photoshop CC no tiene una oferta independiente para Extended.

<div align="center">
![](http://i.imgur.com/b71BB34.png)
</div>
<br>

### Galería de herramientas

#### Herramientas de selección

<div align="center">
![](http://i.imgur.com/UnG1qR5.png)
</div>
<br>

#### Herramientas para cortar y crear sectores

<div align="center">
![](http://i.imgur.com/bsUdrDJ.jpg)
</div>
<br>

#### Herramientas de retoque 

<div align="center">
![](http://i.imgur.com/MA0k3E2.jpg)
</div>
<br>

#### Herramientas de pintura

<div align="center">
![](http://i.imgur.com/ePbx4Oe.jpg)
</div>
<br>

#### Herramientas de dibujo y texto

<div align="center">
![](http://i.imgur.com/puOsinh.jpg)
</div>
<br>

#### Navegación, notas y herramientas de edición

<div align="center">
![](http://i.imgur.com/CfAjIdA.jpg)
</div>
<br>

#### Herramientas 3D

<div align="center">
![](http://i.imgur.com/HVIPoQN.jpg)
</div>
<br>



-----

## Capas

Las capas resultan muy útiles porque permiten añadir componentes a una imagen y trabajar con ellos de uno en uno, sin cambiar de forma permanente la imagen original. Para cada capa, puede ajustar el color y el brillo, aplicar efectos especiales, cambiar de posición su contenido, especificar valores de fusión y opacidad, etc. También puede reorganizar el orden de apilamiento, enlazar capas para trabajar en ellas simultáneamente y crear animaciones Web con capas.

Las capas son como láminas apiladas de vidrio transparente sobre las que puede pintar imágenes. A través de las áreas transparentes de una capa puede ver las capas que hay debajo. Puede trabajar en cada capa de forma independiente, experimentando para crear el efecto deseado. Cada capa es independiente mientras no las combine (fusione). La capa inferior del panel Capas, la capa Fondo, está siempre bloqueada (protegida), lo que significa que no puede cambiar su orden de apilamiento, su modo de fusión ni su opacidad, a menos que la convierta en una capa normal.

<div align="center">
![](http://i.imgur.com/CvZbkQu.png)
</div>
<br>

Las áreas transparentes de una capa permiten ver las capas inferiores.

Las capas se organizan en el panel Capas. Es recomendable tener este panel visible mientras se trabaja con Adobe Photoshop Elements. De un solo vistazo, puede ver la capa activa (la capa seleccionada que está editando). Puede enlazar las capas para facilitar su manejo, de forma que se muevan como una unidad. Dado que varias capas en una imagen aumentan el tamaño del archivo, puede reducirlo si combina las capas que ha terminado de editar. El panel Capas es una fuente de información importante a medida que edita las fotografías. Además, puede usar el menú Capa para trabajar con capas.

Las capas normales son capas basadas en píxeles (imágenes). Puede utilizar otros tipos de capa para crear efectos especiales:

* **Capas de relleno:** Contienen un degradado, color uniforme o un motivo.

* **Capas de ajuste:** Permiten optimizar el color, el brillo y la saturación sin realizar cambios permanentes en la imagen (hasta que acople o contraiga la capa de ajuste).

* **Capas de texto y capas de formas:** Permiten crear formas y texto basados en vectores.

No puede pintar en una capa de ajuste, aunque puede pintar en su máscara. Para pintar en capas de texto o de relleno, primero debe convertirlas a capas de imagen normales.

#### Acerca del panel Capas

En el panel Capas (Ventana > Capas), aparecen todas las capas de una imagen, desde la capa superior hasta la capa Fondo de la parte inferior. En el modo Experto, si trabaja en el Espacio de trabajo personalizado, puede arrastrar el panel Capas para extraerlo y adjuntarlo a otros paneles.

La capa activa, o la capa en la que trabaja, está resaltada para identificarla con facilidad. Cuando trabaja en una imagen, conviene comprobar cuál es la capa activa para asegurarse de realizar los ajustes y las ediciones en la capa correcta. Por ejemplo, si selecciona un comando y parece que no ocurre nada, compruebe que está mirando la capa activa.

El uso de los iconos del panel permite llevar a cabo muchas tareas, por ejemplo, crear, ocultar, enlazar, bloquear y eliminar capas. Con algunas excepciones, los cambios solo afectan a la capa seleccionada o activa, que aparece resaltada.

<div align="center">
![](http://i.imgur.com/sqTE7gL.png)
</div>
<br>

**A.** Menú Modo de fusión** B.** Mostrar u ocultar capa **C.** La capa está enlazada a otra capa **D**. Previsualización de una capa **E.** La capa resaltada es la capa activa **F.** Capa bloqueada **G**. Se ha aplicado un estilo a la capa 


-----


## Tipos de imagen/color

El Formato de un archivo fotográfico va depender exclusivamente del uso que hagamos de él, Photoshop nos va a permitir abrir y guardar en distintos formatos, si estamos guardando una imagen Photoshop te permitirá guardar tanto en el formato nativo(*.psd ó *.pdd ) ó en otros formatos (*.jpg, *.gif, *.png, *.tif, etc.).

**Formatos más utilizados:

**PSD:** Es el formato nativo de photoshop, que siempre es interesante que lo guardes cuando estés haciendo algún tipo de proceso de datos, ya que te permite guardar el diseño completo junto con las capas para así posteriormente puedas abrir y seguir retocando o diseñando.

**TIFF:** Es también un formato conocido sobre todo cuando vas a guardar para imprenta que te permite guardar con componentes de capa, las nuevas versiones de photoshop te permiten guardar en este tipo de formatos, pero no es conveniente el espacio que ocupa este formato es mal elevado que formato de photoshop o de algún otro, pero si estas pensando en llevar a una imprenta sería interesante que lo guardes en este formato.

**JPG:** Es un formato estándar que comprime la imagen por lo tanto habrá una variación de color y este formato lo utilizaras cuando tengas que publicar en un Sitio Web o visualizar en monitores, Photoshop te permitirá guardar en este formato en diferentes calidades (Alta, Media, Baja).

**GIF:** Es un formato estándar que también comprime la imagen y por lo tanto habrá una variación de calidad y este formato también lo para publicar en Sitios Web o visualizar en monitores, este formato te permite guardar en 256 niveles de color, también permite guardar transparentes y animaciones.

**PNG:** También es un formato estándar, pero este tiene las mejores características de los 2 formatos anteriores, tanto PNG-8 ó PNG-24 te permite guardar Zonas transparentes, permite una compresión, este formato también es usado para las publicaciones en sitios web o mostrar en monitores.

**RAW:** Formato original de cámara este guarda la información bruta de la lente de una cámara, es importante siempre en cuando sea posible trabajar con este formato y configurar sus parámetros antes de pasar a Photoshop, y posteriormente pasar a photoshop para hacer los retoques o manipulaciones que quieras realizar sobre esa imagen fotográfica.

En photoshop al igual que en cualquier otro tipo de programa de la misma índole se pueden distinguir dos tipos de imágenes.

* Imágenes Vectoriales
* Mapa de bits

### Tipo de color

#### RGB, modo de color

El modo Color RGB de Photoshop utiliza el modelo RGB y asigna un valor de intensidad a cada píxel. En imágenes de 8 bits por canal, los valores de intensidad varían de 0 (negro) a 255 (blanco) para cada uno de los componentes RGB (rojo, verde, azul) de una imagen en color. Por ejemplo, un color rojo fuerte podría tener un valor R de 246, un valor G de 20 y un valor B de 50. Si los valores de los tres componentes son idénticos, se obtiene un tono de gris neutro. Si los valores de todos los componentes es 255, el resultado es blanco puro, y negro puro si el valor es de 0.

Las imágenes RGB utilizan tres colores o canales para reproducir los colores en la pantalla. En imágenes de 8 bits por canal, los tres canales se convierten en 24 (8 bits x 3 canales) bits de información del color por píxel. En imágenes de 24 bits, los tres canales pueden reproducir hasta 16,7 millones de colores por píxel. En imágenes de 48 bits (16 bits por canal) y 96 bits (32 bits por canal), pueden reproducirse incluso más colores por píxel. Además de ser el modo por defecto en las imágenes nuevas de Photoshop, el modelo RGB lo utilizan los monitores de los ordenadores para mostrar los colores. Esto significa que, si se trabaja en modos de color distintos a RGB, como CMYK, Photoshop convierte la imagen CMYK a RGB para la visualización en pantalla.

Aunque RGB es un modelo de color estándar, puede variar el rango exacto de colores representados, según la aplicación o el dispositivo de visualización. El modo Color RGB de Photoshop varía de acuerdo con el ajuste del espacio de trabajo especificado en el cuadro de diálogo Ajustes de color.

#### Modo de color CMYK

En el modo CMYK, a cada píxel se le asigna un valor de porcentaje para las tintas de cuatricromía. Los colores más claros (iluminaciones) tienen un porcentaje pequeño de tinta, mientras que los más oscuros (sombras) tienen porcentajes mayores. Por ejemplo, un rojo brillante podría tener 2% de cian, 93% de magenta, 90% de amarillo y 0% de negro. En las imágenes CMYK, el blanco puro se genera si los cuatro componentes tienen valores del 0%.

Utilice el modo CMYK en la preparación de imágenes que se van a imprimir utilizando cuatricromía. Convertir una imagen RGB a CMYK crea una separación de color. Lo más aconsejable al comenzar a trabajar con una imagen RGB es editarla en RGB y convertirla a CMYK al final del proceso de edición. En el modo RGB, puede utilizar los comandos Ajuste de prueba para simular los efectos de una conversión a CMYK sin cambiar los datos reales de la imagen. También puede utilizar el modo CMYK para trabajar directamente con imágenes CMYK escaneadas o importadas de sistemas de alta resolución.

Aunque CMYK es un modelo de color estándar, puede variar el rango exacto de los colores representados, dependiendo de la imprenta y las condiciones de impresión. El modo Color CMYK de Photoshop varía de acuerdo con el ajuste del espacio de trabajo especificado en el cuadro de diálogo Ajustes de color.

#### Modo de color Lab

El modelo de color CIE L*a*b* (Lab) se basa en la percepción humana del color. Los valores numéricos de Lab describen todos los colores que ve una persona con una capacidad de visión normal. Como Lab describe la apariencia del color en lugar de la cantidad de colorante necesaria para que un dispositivo (como un monitor, una impresora de escritorio o una cámara digital) produzca el color, Lab se considera un modelo de color independiente de dispositivo. Los sistemas de gestión de color utilizan Lab como referencia de color para transformar un color de forma predecible de un espacio de color a otro.

El modo de color Lab contiene un componente de luminosidad (L) que varía entre 0 y 100. En el Selector de color de Adobe y el panel Color, el componente a (eje verde-rojo) y el componente b (eje azul-amarillo) pueden estar comprendidos entre +127 y –128.

Las imágenes Lab se pueden guardar en distintos formatos: Photoshop, EPS de Photoshop, Formato de documento grande (PSB), PDF de Photoshop, RAW de Photoshop, TIFF, DCS 1.0 de Photoshop o DCS 2.0 de Photoshop. Las imágenes Lab de 48 bits (16 bits por canal) se pueden guardar en estos formatos: Photoshop, Formato de documento grande (PSB), PDF de Photoshop, RAW de Photoshop y TIFF.

#### Modo de escala de grises

El modo Escala de grises utiliza distintos tonos de gris en una imagen. En imágenes de 8 bits, puede haber hasta 256 tonos de gris. Cada píxel de una imagen en escala de grises tiene un valor de brillo comprendido entre 0 (negro) y 255 (blanco). En imágenes de 16 y 32 bits, el número de tonos de una imagen es mucho mayor que en las imágenes de 8 bits.

Los valores de la escala de grises también se pueden medir como porcentajes de cobertura de la tinta negra (0% es igual a blanco, 100% a negro).

El modo Escala de grises utiliza la gama definida en el ajuste del espacio de trabajo especificado en el cuadro de diálogo Ajustes de color.

#### Modo de mapa de bits

El modo Mapa de bits utiliza uno de los dos valores de color (blanco o negro) para representar los píxeles de una imagen. Las imágenes en modo Mapa de bits se denominan imágenes de 1 bit en mapa de bits porque tienen una profundidad de bits de 1.

#### Duotono, modo

El modo Duotono crea imágenes en escala de gris monotonos, duotonos (dos colores), tritonos (tres colores) y cuadritonos (cuatro colores) utilizando de una a cuatro tintas personalizadas.

#### Modo de color indexado

El modo Color indexado produce archivos de imágenes de 8 bits con un máximo de 256 colores. Al convertir a color indexado, Photoshop crea una tabla de colores de consulta (CLUT) que almacena y genera el índice de los colores de la imagen. Si un color de la imagen original no aparece en la tabla, el programa selecciona el más parecido o emplea el tramado para simular el color utilizando los colores disponibles.

Aunque la paleta de colores es limitada, el modo Color indexado puede reducir el tamaño de archivo manteniendo la calidad visual necesaria para presentaciones multimedia, páginas web y usos similares. En este modo está disponible la edición limitada. Para ediciones extensas es necesario convertir temporalmente al modo RGB. Los archivos de color indexado se pueden guardar en los siguientes formatos: Photoshop, BMP, DICOM (Digital Imaging and Communications in Medicine), GIF, EPS de Photoshop, Formato de documento grande (PSB), PCX, PDF de Photoshop, RAW de Photoshop, Photoshop 2.0, PICT, PNG, Targa® o TIFF.

#### Modo Multicanal

Las imágenes de este modo contienen 256 niveles de gris en cada canal, por lo que se utilizan en impresión especializada. Las imágenes de modo Multicanal se pueden guardar en formato Photoshop, Formato de documento grande (PSB), Photoshop 2.0, RAW de Photoshop o DCS 2.0 de Photoshop.

Se aplican las pautas siguientes al convertir imágenes al modo Multicanal:

* Las capas no se admiten y, por lo tanto, se acoplan.
* Los canales de color de la imagen original se convierten en canales de tinta plana en la imagen convertida.
* Convertir una imagen CMYK al modo Multicanal crea canales de tintas planas cian, magenta, amarilla y negra.
* Convertir una imagen RGB al modo Multicanal crea canales de tintas planas cian, magenta y amarilla.
* La eliminación de un canal de una imagen RGB, CMYK o Lab convierte automáticamente la imagen al modo Multicanal y acopla las capas.
* Para exportar una imagen multicanal, guárdela en el formato DCS 2.0 de Photoshop.

# Optimización de imágenes para web

No es nada nuevo que las imágenes son un pilar fundamental en nuestra página web: es lo que nos va a ayudar a captar la atención de nuestras visitas y hasta puede ser el elemento detonador de una compra... si lo hacemos bien. Subir una foto de mala calidad, o tener una pésima organización de ellas, puede ocasionar el efecto contrario claro está.

### ¿Por qué es importante optimizar las imágenes?

Las razones son muchas pero nos quedamos con las tres más importantes:

* **SEO:**  uno de los factores que contribuye al posicionamiento es la velocidad de la carga de la página o dicho de otra manera, una página cuya carga en el navegador sea lenta, tendrá menos posibilidades de posicionar correctamente. Las imágenes pesadas (muchos KB o MB) hacen que la velocidad de carga de una página se vea ralentizada.
* **Conversión:** Una página cuya estructura y la combinación de imágenes y textos sea organizada, tendrá más posibilidades de atraer, retener y "convertir" en clientes a las visitas.
* **Estética:** las imágenes  de pésima calidad hacen de todo menos transferir una imagen seria y profesional de nuestro negocio.

### Calidad de las imágenes

¿Puedes ver la diferencia entre estas dos imágenes de abajo? A simple vista no hay ninguna diferencia, pero sin embargo una está optimizada para la web y la otra no. ¿Quieres saber cuál es la diferencia?

<div align="center">
![](http://i.imgur.com/qAMv9sl.jpg)
</div>
<br>

Vamos a explicar porqué una está optimizada y la otra no: 
 
* **PÍXELES**

El tamaño en píxeles de la imagen original es el tamaño de largo y ancho. Piensa que 32 píxeles son 1 centímetro: por lo que la imagen original de la derecha (no optimizada) sería de 187,5 cm (que es la altura de un hombre adulto). Este es un tamaño innecesario para una imagen dentro de una columna. Podemos tener imágenes de 1000 o 2000 píxeles por ejemplo en el área superior de algunas plantillas (que está destinada para tener una imagen).
 
* **RESOLUCIÓN**

Ppp significa píxeles por pulgadas (también puedes verlo en inglés como dpi -dot per inch- o ppi -pixels per inch﻿)﻿. Cuanto mayor sea el número de pp, mayor será la calidad, pero eso servirá para la impresión de una imagen. Por ejemplo, para una página web, 72 pp será suficiente; mientras que para un imagen de un periódico se necesita al menos 300 pp.
 
* **TAMAÑO**

Efectivamente, la imagen optimizada será menos pesada (33KB) que la imagen no optimizada para web (10, 3 MB) y eso influye en la velocidad de carga de la página. Existen diferentes formas para guardar imágenes para web o incluso plataformas online como pixlr donde puedes optimizarlas. Como decíamos, lo importante es la forma de guardar el archivo para web: podemos incluso lograr que una imagen de 2000px, optimizada para web y que no sea demasiado pesada.

**En resumen, tendremos que buscar el equilibrio entre el tamaño y la calidad que queremos de la imagen para poder subirla correctamente a nuestra página web.**

----------------

### ¿Qué formato utilizar? ¿.jpg, .png o .gif?

* **Formato .png:** se utiliza sobretodo para las imágenes que están hechas con formas geométricas y tienen colores planos. La gran ventaja de este formato es que conserva las transparencias y que no pierde mucha calidad en la compresión de la imagen, por eso se utiliza para logotipos.

* **Formato .jpg:** es el formato universal que se utiliza sobre todo para las imágenes, pues aunque se pierde un poco de calidad al comprimir las imágenes, no se pierden colores o tonalidades.
 
* **Formato .gif:** este formato se utiliza para animaciones sobretodo. Dado que se utilizan varias imágenes o un vídeo para hacer el gif, el tamaño en kb puede ser muy grande; por eso, en ocasiones se comprime la imagen y pierde calidad.

------------------------------

### Combinación imágenes y textos

No sirve de nada que hayamos optimizado las imágenes si al final vas a hacer esto:

<div align="center">
![](http://i.imgur.com/nT8l3k3.png)
</div>
<br>

Para que un diseño sea efectivo y que las imágenes capten la atención de las visitas, es fundamental que estén bien combinadas. En el ejemplo superior, vemos imágenes de diferentes tamaños y con un alineación distinta (derecha, centrada...).
 
Para que las imágenes ayuden a organizar el contenido y funcionen como un elemento de atracción, debemos hacer que tengan el mismo tamaño (ancho x largo) o el mismo ratio (16:9, 4:3, 1:1) como en el ejemplo de la imagen inferior.

<div align="center">
![](http://i.imgur.com/DG5hiRC.png)
</div>
<br>

**El orden y la armonía de las imágenes y los textos hacen que las personas encuentren el diseño agradable y no; y eso es lo que hace que sea efectivo o no.**

### En resumen...

* Utiliza imágenes con un tamaño en píxeles adecuado en función de para lo que lo quieras utilizar (imagen de fondo, para una columna...)
* Optimiza la imagen para web para que no sea muy pesada (KB) pues eso ayudará a la velocidad de carga de tu página.
* Guarda las imágenes según el formato que más convenga a la imagen.
* Haz que las imágenes tengan el mismo tamaño o ratio para que el diseño sea más efectivo.
