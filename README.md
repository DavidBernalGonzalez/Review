# Review
Repositorio con los conceptos vistos en cada clase

Día 1: Presentación y HTML

Qué utilizaremos en este curso:
- Herramientas de colaboración: Slack, Trello, Github
- Herramientas de desarrollo: Visual Studio Code, Navegador, Codepen.io
- Herramientas de trabajo: Técnicas Agile: Scrum, Kanban

La Página Web
Se desarrolla con un editor de texto, se exporta a un servidor de hosting, se asocia a un dominio.

HTML
Una página web consta de tres etiquetas obligatorias: html, head y body
Los elementos de una página web se construyen con etiquetas:
Títulos - h1,h2,h3,...
Párrafos - p
Imágenes - etiqueta sin cierre
Listas ordenadas y desordenadas

Clonamos la TRIBUTE PAGE:Ejercicio entregable

Día 2

Estructura de una página web:

Construimos la estructura general de la web mediante elementos semánticos estructurales:
header, main, section, article, footer, aside, nav...

Desarrollamos cada uno de los bloques utilizando el resto de elementos semánticos:
h1,h2,..., ul, ol, p, table, etc.

Todo el contenido que mostrará la página siempre dentro de la etiqueta body.
Toda la información no visual, que sirve para dar información al navegador, dentro de la etiqueta head.

Utilizamos atajos para trabajar en codepen.io, recogidos en esta [página de resumen](https://docs.emmet.io/cheat-sheet/)
Clonamos el blog de la página Andén 27: https://codepen.io/rglepe/pen/OJNYwXy

Día 3

Comenzamos reunión de proyecto sprint

Montamos Visual Studio Code, la herramienta de desarrollo que utilizaremos. Extensiones interesantes: BrowserSync, Colorize, ...


Repaso de estructura de HTML

Inicio CSS:
formato de una regla CSS
concepto de herencia de estilos
selectores de id y de clase

Ejercicio con selectores de clase
Recepta de la iaia. EJercicio entregable

Día 4

Comenzamos con reunión diaria

Hablamos de Git, el sistema de control de versiones:
  - Guarda Versiones del código
  - Permite trabajo colaborativo
  - Trabajamos con GitHub
 
 Instalamos desde la página oficial de git.
 
 Para trabajar con un repositorio de GitHub: `git clone <url del repositorio de Github>`
 
 Para subir cambios a GitHub:
 1. Preparamos el código: `git add .`
 2. Hacemos commit: `git commit -m 'Escribimos el mensaje que queramos'
 3. Subimos los cambios a Github: `git push`
 
 CSS:
 Trabajamos con los distintos selectores CSS, para aumentar la especificidad a la hora de aplicar los estilos:
 
 Jugamos a [CSS Diner](https://flukeout.github.io/)
 
 Comenzamos [la página personal](https://codepen.io/freeCodeCamp/full/zNBOYG)
 
 Día 5
 
 Problemas con las fuerzas del orden.
 
 Hoy toca Git, comenzando desde local. Si partimos de un código ya existente en local, realizaremos los siguientes pasos para subir a Github:
 1. Sólo la primera vez: `git init`
 2. `git add .`
 3. `git commit -m 'message'`
 4. Sólo la primera vez. Creamos un repositorio vació en github y copiamos su url.
 5. Sólo la primera vez, damos de alta el repositorio remoto: `git remote add origin <<url repositorio>>`
 6. Subimos al repositorio: `git push origin master`
 
 Vemos pseudo-elementos que permiten modificar o añadir contenido al html: before, after, first-letter, first-line, ...
 Vemos pseudo-clases que permiten añadir estilos a estados concretos de algunos elementos: link, visited, hover, ...
 
 El modelo de caja (model box): 
 - Ancho de caja = margen izqdo + borde izqdo + padding izqdo + contenido + padding dcho + borde dcho + margen dcho
 - Alto de caja = margen superior + borde superior + padding superior + contenido + padding inferior + borde inferior + margen inferior
 
 Propiedad `box-sizing` permite fijar la referencia al ancho estándar (border-box) o al contenido (content-box)
 
 Positioning
  - display: fijamos cómo aparecen los elementos en el flujo de la página: block vs inline (inline-block, otros...)
  - position: fijamos dónde aparecen los elementos en el flujo de la página. Se establece el inicio de coordenadas (0,0) en el vértice superior izdo de la pantalla. Los valores posibles: relative, absolute, fixed, sticky
  - float: los elementos "flotan", dejan de ocupar el espacio original y se desplazan hacia arriba.
  
 Comenzamos Programación 
 - Introducimos el concepto de DOM. La página web se modela como un árbol de nodos ocupados por los elementos html.
 - Hablamos del editor de javascript (repl) y realizamos nuestro primer programa con salida a consola y a web.
 
 Día 6
 
 Fundamentos de Javascript: variables.
  Variables son estructuras de memoria para almacenar información de nuestra app
  Una palabra reservada: var, let y const. Ej.: let miVariable = 5;
   let num = 1;  tipo number
   let text = "hola mundo"; tipo string
   let isPresent = true; tipo boolean
   let sinValor; tipo undefined
  
  Program
   Mediante un pop-up del navegador: window.prompt("Dame un num"); window.alert(resultado)
   
  FLEXBOX
    Se aplica sobre los hijos, pero se define en el padre con display:flex, justify-content, order, ...
  
  Clonamos la _landing-page_ de Spotify, ejercicio evaluable.
  
  Día 7
  
  Fundamentos de Javascript: Objeto String y toma de decisiones (if..else)
  Ejercicio encontrar la letra de un texto con salida a terminal y web.
  
  CSS Responsive
  reglas de _media query_ nos permiten adaptarnos a un ancho concreto de dispositivo
  Programación mobile first
  Unidades de medida responsive (vh y vw)
  
  Ejercicio: responsive-slack, ejercicio evaluable
  
  Día 8
  
  Fundamentos de JavaScript: Hablamos de condiciones complejas: if...else if...else, switch...case
   - Operadores lógicos: && (y) || (o)
  Ejercicio: bar y bebidas.
  
  Tiempo de desarrollo libre.
  
  Día 9
  
  Fundamentos de Javascript: Bucle For
  Basics-JS.
  
  CSS: Transformaciones, transiciones y animaciones.
  Mandamos el reloj.
  
  Día 10
  
  Funciones JavaScript: 
    
```js
    function generarRandom(parametros){
        let aleatorio = Math.floor((Math.random()*10)+1);
        return aleatorio;
    }
    
    const numeroRandom = function(parametros){
        let aleatorio = Math.floor((Math.random()*10)+1);
        return aleatorio;
    }
    
    const numeroRandomFlecha = (parametros) => {
        let aleatorio = Math.floor((Math.random()*10)+1);
        return aleatorio;
    }
    
    let numero1 = generarRandom();
    let numero2 = numeroRandom();
    let numero3 = numeroRandomFlecha();
    
    console.log(numero1);
```
    
Funciones en JavaScript _First-class functions_:
Son OBJETOS. 
Si se pasan por parámetro son funciones de callback: 
    
```js
     const functionOne = (x) => console.log(x);
     
     const functionTwo = (var1, var2) => var2(var1); 
     
     functionTwo(2, functionOne) ~ functionTwo(2, (x)=>console.log(x));
```
     
Dos ejercicios: Travel-agency y Averigua un número.
    
Día 11
    
Funciones en JavaScript: Arrays
    
Arrays: colecciones ordenadas de elementos.
    
Se define con su literal: [ ];
Son objetos: `let miArray = [ ];`

```js
let numeros = [1,2,3,4,5];
let mascostas = ["perro","gato",4, null, true,{nombre: Osama}, [1,2,3,4]]
    
console.log(numeros[0]); // -> 1
    
for(let i = 0; i< numeros.length; i++){
console.log(numeros[i]);
}
``` 

Ejercicio funciones-arrays con testing.
    
Día 12
    
Funciones de Array iteradoras: `array.map(callback)` `array.reduce(callback)`
    
Ejercicios de Arrays.
    
Objetos: {_key:value_, _key:value_}. 
    - NombreObjeto.nombrePropiedad => inserta la prop en el obj si no existe y si existe sustituye el valor.
    - NombreObjeto["nombrePropiedad"]
    
Recorrer objetos: for(let prop in array){ console.log(array[prop]) }
    
Ejercicio de academia.
    
  
Día 13
  
Monográfico de CSS Grid. 
  - Se aplica sobre el contenedor (= flex)
  - Grid primero definimos la cuadrícula:

    ```CSS
    .grid{
      display:grid;
      grid-template-row: repeat(4, 5rem);
      grid-template-column: repeat(4, 5rem);
      }
     
     .grid-item1{
     grid-row: 1 /span 2;
     grid-column: 4;
     }
    .grid{
       width: 100%;
       height: 100vh;
       display:grid;
       grid-template-areas: 
       "header header"
       "main   aside"
       "footer footer"
    }
   
    header{
    grid-area: header;
    }
    ```
Corregimos el ejercicio de arrays-guapos. array.Map y array.Reduce
  
Día 14
  
Trabajando con arrays y objetos dentro de funciones. Ejercicio del cluedo. 
  
Introducción al DOM. La representación de un documento html en forma de árbol. La necesita JavaScript para poder interaccionar con la página.
  1. Obtener el elemento que queremos manipular
  2. Después modificamos estilos, añadimos nuevos nodos hijos, etc.


Día 15

Intro al DOM manipulation:
    - Selecció de elements.
    - Modificació de estils.
    - Exercicis de manipulació del dom: tres botons i formulari
    
Dia 16:

- CSS
```css
    .yellow{
    background-color:yellow;
    }
```

- javascript
```js
    let parrafo = document.getElementsByTagName('p')[0];
    
    const callback = (event) => {
//      parrafo.style.backgroundColor = 'yellow';
      parrafo.classList.add = '.yellow';
    }
    parrafo.onmouseover = callback;
    parrafo.onclick = callback;
    
    parrafo.addEventListener('mouseover',callback);
    parrafo.addEventListener('click', callback);
    
    parrafo.removeEventListener('mouseover',callback);
```
Ejercicio: Hackaton
    
   
   
  

 
