Green Recursos
https://htmlreference.io/
https://developer.mozilla.org/es/
https://colorhunt.co/
https://cssgradient.io/gradient-backgrounds/
https://iconos8.es/
htts://css-tricks.com
labs.jensimmons.com

Green

Red ======== DOM, CSSOM, Render Tree y proceso de renderizado de la Web

DOM: Document object model

CSSOM: El codigo CSS lo convierte en objetos para que el navegador lo entienda.

Render Tree: es la unión del DOM y del CSSOM

    Procesos del navegador 
    1> Procesa el HTML y construye el DOM
    2> Procesa el CSS y construye el CSSOM
    3> DOM+CSSOM = Render Tree
    4> Ejecuta el diseño en el render tree
    5> Pinta el nodo en pantalla

Red ========== Tips para CSS 

1: LOs selectores que se pueden usar para el HTML
Universal <=  *{margin0;}
Tipo      <=  h1{color:Red;}
Clase:    <=  .saludo{font-size:2em;}
ID:       <=  #id{border-radius:20px;}

2: Anatomía de la declaración en CSS:

Declaración
  p{color:Pink;}
  p => selector
  color => propiedad
  Pink => valor

Red =========== Funciones de las etiques HTML más importantes =======

Red ============ Tipos de Errores

> Errores sintácticos:
    
    Errores de escritura en el código que hacen que el programa no funcione 

> Errores lógicos:  

    Errores de sintaxis, el código no hace lo que debería y el programa 
    funciona de manera incorrecta

Red ============ Anatomía de CSS 

*{} => Universal: se aplica a todo en el HTML
fisrt-child: se aplica al primer hijo
last-child: se aplica al ultimo hijo
nth-child: 

> pseudo elementos:

:: before
:: after
etc 

Red =========== Modelo de Caja

margin
______________________
  border
  ______________________
    padding
    ______________________
Red ========== Valores relativos y absolutos 

absolutas 
cm
mm
px
pc
pt
in

relativas

vmax
em
rem
etc ..

Red ============== Displays en CSS 

Block: simula el movimiento de la escritura, de arriba abajo, de izquierda a derecha
      
      <p>, <h1>, <section>, <div>, <ul>, etc.

Inline: simula la escritura igual pero solo de izquierda a derecha
      
      <span>, <em>, <b>

None: Se utiliza para ocultar elementos sin eliminarlos por completo de DOM

Table: Los elementos de este display se comportan como en un <table>

Flex: Centrar elementos a la izquierda o derecha, por defecto alinea a la izquierda
      este display tambien suele estar acompañado de: justify-content y align-items
      
      Green 
      https://css-tricks.com/snippets/css/a-guide-to-flexbox/
      Green 

Grid: Es un sistema de layaout similar a flexbox pero mas potente
      
      Green
      https://css-tricks.com/snippets/css/complete-guide-grid/

Red ======== Funciones y propiedades CSS 

width: Define el ancho de un elemento
height: Define el alto de un elemento
background: Puede definir el color de fondo o la url de fondo de un elemento
background-color: Define el color de fondo de un elemento
color: Define el color de nuestros textos
    
    >Colores con los nombres
    > Sistema hexadecimal
    > RGB
border: Define el tamaño, estilo y color del borde de un elemento
border-radius: Define que tan redondeado quiero mi elemento
margin: Define el margen de un elemento
        
        margin 2px;
        tendrá un margen de 2 pixeles en sus 4 lados
        margin 2px 3px 4px 5px
        tendrá un mergen de 2 px en el top, 3px en el right, 4px en el bottom y
        5px en el left

padding: Define la distancia del borde de un elemento hasta su contenido
font-size: Define el tamaño de la fuente
font-family: Define la familia tipográfica de la fuente
opacity: Dtermina la transparencia del elemento
outline: Hace que los elementos destaquen por defeco con una linea azul
transition: Permiten al CSS cambiar los valores de las propiedades sin problemas
            durante una duración determinada. UNA TRANSICIÓN NO ES UNA ANIMACION
animation: Permite que animar elementos.

Red =========== Pocisionamiento en CSS

El posicionamiento en CSS es una de las cosas más importantes, pues establece 
como van a estar ubicados nuestros elementos en pantalla

Los elementos se posicionan utilizando las propiedades top, bottom, left, right
pero solo funcionarán si la propiedad position está establecida.

La propiedad postion tiene 7 valores diferentes:

relative: Coloca el elemento en relación a su posición normal
absolute: Se ubican en relación al elemento relativo más cercano
          (podemos hacer usao de top, bottom, left, right)
fixed: Se ubica en relación con la ventana del navegador y también se ve afectado 
       por las propiedades top, bottom, left, right
sticky: Se posiciona en función de la posición de desplazamiento del usurario
        si se ubica a la izquierda, siempre está ahí sin importar cuantas veces 
        haga scroll el usuario
static: no se ve afectado por top, bottom, right, left
initial: Ubica el elemento en la posición que tiene  de forma predeterminada
inherital: Hereda la propiedad del elemento padre.

Red ================ Arquitecturas de CSS

Objetivos de la arquitectura CSS

> Predecible: Establecer reglas para que se cumplan
> Reutilizable: evitar escribir más lineas
> Mantenible: 
> Escalable: 

Buenas practicas:

Establece reglas con el equipo.
Explicar la estructura base
Establecer estándares de codificación: Definido desde el principio
Evitar larjas hojas de estilo:
Documentación

=================== OOCSS, BEM, SMACSS, ITCSS, Atomic Design

OOCSS: CSS orientado a objetos
SMACSS: arquitectura de CSS escalable y modular
        dividir el css en componentes bases
        layaout: elementos en la página que se usan una vez
        modulo: componentes que se usan más de una vez
        estado: acciones de los componentes
        temas: que cambien los temas y colores desde el codigo

BEM: Bloque, elemento, modificador

ITCSS: Triangulo invertido de CSS
Permite dividir los archvios de css para que no se convinen entre sí
Se habla de especificidad, cada elemento tiene más peso que otro.

Atomic Design: Es CSS es modular, atomos son elementos chiquitos(ex: botones)
               va creciendo hasta tener una clase completa.

Red ================== Componentes 

Los elementos por defecto tienen un display que es block, hace que los 
elementos se pociciones uno debajo del otro 

Red ===================== Flexbox

Maquetación y responsive design 
Practicar con el juego de los sapos. 

Red =============== CSS Grid
Ayuda al responsive design

Practicar con el juego de grid garden 

Red =================== Media queries
Es lo que nos premite el responsive designe 
 
Red =================== Preprocesadores
Un preprocesador de CSS es un programa que permite generar CSS a partir
de la syntax unica de del preprocesador.

  https://sass-lang.com/guide
  http://lesscss.org/
  http://stylus-lang.com/

Red ===================== SASS

Ahora con SASS podemos crear variables, crear bloques de código CSS
para poder reutilizarlos y no escrbir muchas líneas de código

> Declaración de variables

    $nombreVariable: valor;
      
        valor => puede ser un color en formato hexadecimal 
                 tambien admite formato RGB y RGBA

  > para llamar la variable 
  example:
      
        color: $nombreVariable;

  y listo!
  
> Anidamiento

Cuando tenemos clase que tiene propiedades pero tambien existen clases
dentro de esta clase en el HTML, entonces para reutilizar código
se puede de igual manera en el .scss tener anidación de elementos
donde los elementos internos de una clase van a heredar las propiedades
que tiene su clase padre.

> Herencia

Podemos crear una clase en el .scss para poder colocar bloques de código
repetitivos para luego llamarlo a estilos donde se necesiten y así
minimizamos el códio y/o flujo de trabajo en el CSS

SYNTAXIS

  .claseNuevaParaHeredar{
      propiedades: deClase;
  }

  .body{
      @extend .claseNuevaParaHeredar;
  }

> Mixin
Es similar a la herencia solo que este puede recibir argumentos para propiedades
y su sintaxis es diferente

  @mixin nombreMixin{
    propiedades: tamañopx;
  }

  .body{
    @include nombreMixin;
  }
