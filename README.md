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

Exercicis de manipulació del dom: tres botons i formulari
    
Dia 15:

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
    
Día 16:

- Ejercicios dom manipulation: eventos


- Sass

Dia 17:

- Validación formularios con JavaScript. 
    API validación js que podemos consultar para saber si se han pasado los filtros de validación:
      filtro de validación en html: required, minlength, maxlength, min, max, pattern
      Informan una propiedad validate. tooShort, patternMismatch, rangeUnderflow, rangeOverflow.
      
      ```html
        <form novalidate>
        <input type="text" name="nombre" minLength="3">
        </form>
      ```
      ```css
          input[type="text"]:invalid{
            border: 1px solid red;
          }
       ```
      ```javascript
        let nombre = document.getElementsName('nombre')[0];
        
        if(nombre.validate.tooShort)
            mensaje = `Has introducido ${nombre.value} carácter`;
      ```
        
- the shopping cart

Día 18:

Programación Orientada a Objetos: Clases

Clases: Objetos utilizados como moldes para crear otros objetos. 
ES6: class Student {}

Objetos creados a partir de la clase se llaman instancias: `let john = new Student();`

Ejemplo:
```js
//estudiantes, profesores, miembros de administración


class Persona {
  name;
  edad;
  rol;

  constructor(name, edad, rol){
    this.name = name;
    this.edad = edad;
    this.rol = rol;
  }
}

let persona = new Persona('Luis',25,'estudiante');

console.log(persona.name);

class Estudiante extends Persona{
  
  #calificaciones;

  constructor(name, edad, rol){
    super(name,edad,rol);
    this.#calificaciones = [];
  }

  get calificaciones(){
    return this.#calificaciones;
  }

  set calificaciones(calificacion){
    this.#calificaciones.push(calificacion);
  }

}

class Profesor extends Persona {
  materia;

  constructor(name,edad, rol, materia){
    super(name,edad,rol);
    this.materia = materia;
  }

  hacerTutorias(){
    return `horario de ${this.materia} de 12:00 a 14:00`;
  }
}

let estudiante = new Estudiante('Ana',22,'estudiante');

let profesorReact = new Profesor('Sara', 30, 'profesor','React');

console.log(profesorReact.hacerTutorias());

console.log(estudiante);
```

Día 19

JavaScript Asíncrono:
  - setTimeout(callback, delay); -- devuelven un id que podemos utilizar para parar la función con clearTimeout(id);
  - setInterval(callback, interval); -- clearInterval(id)
  
 ... AJAX - API 
 
 Día 20
 
Promises
Ejercicios: codingame, margarita, codewars, suma+potencia.

Día 21

HTTP: protocolo o conjunto de reglas para establecer las comunicaciones via web.
  - Método o Verbo de comunicación:GET, POST, PUT, DELETE, HEAD, OPTIONS,...
  - URL: dirección donde se encuentra el recurso.
CORS: Cross-Origin Resource Sharing (CORS)
  - API Countries: no hay problema porque la petición es una Simple Request.
  - API Neighbours: ?key=ASDFLKASDFOI&Country_code=
  
Request: headers Method, URL, authentication
Response: headers, status codes: 200, 404, 500, 401,201

---

API fetch()
  Trabajar con recursos via HTTP.
  Devuelve una promesa con la respuesta.
    - response.json(); --> array de objetos javaScript.
    - response.arrayBuffer; --> streaming para visionar video
    - response.text(); 
 
---
Destructuring de arrays y objetos: 
   - arrayNew = [...array]
   - {name, surname}= user;
   - {name:nombre, surname: apellido}= user;
   
Día 22

- API Geolocalización. Extraer coordenadas de un punto. Donde nos encontramos. 
   `navigator.geolocation`
   Objeto: Position
- Representación de unas coordenadas en un mapa: google.Maps, leaflet.js Open Street Map, Bing.com/maps, entre otras.

Ejercicio de los mapas.

Día 23

TypeScript: JavaScript fuertemente tipado. Tipamos propiedades, objetos, funciones...
  -Utilizamos tipos básicos: string, number, boolean, Symbol, Object
  -Tipos personalizados: 
    - Se declaran con `type` + un alias: `type stringArray = Array<string>`
    - Declarar tipos con `interface`: `interface {name: string, age: number}`. Manera de dar forma a los datos.
  - Incluir ESNext
  - Anotaciones: @templateUrl: Metadatos que modifican el compartamiento de objetos
  
Compilación: configuramos TypeScript en el archivo `tsconfig.json`:
  - a qué versión de JavaScript queremos compilar,
  - checking de errores, grado de rigurosidad.

TypeScript permite exportar información que se puede utilizar con herramientas Linting. ESLint, TSLint.

Es el lenguaje de programación de Angular y cada vez de más frameworks de front-end y de back-end.

Ejercicio de la calculadora

Día 24
  Rehicimos la calculadora para aceptar cualquier número de parámetros.
  Vimos como compilar typescript via tsc para generar el build.
  Explicamos lo que eran los __módulos__
    - Estructuras para limitar el ámbito de los bloques de código que contiene. 
    - Normalmente un módulo coincide con un fichero. Ej:
        - calculadora.ts --función calculator // multiplier();
        - multiplier.ts -- función multiplier
    - exportar un bloque de código lo convierte en un módulo. export class{}, export function(){}
    - para utilizar la información de un módulo desde otro módulo hay que importar el bloque de código. `import multiplier from 'multiplier'`
   
   - Caso de export parcial del módulo
    + funciones...
    `export const miFunc = () =>{}`   ||| import {miFunc} from 'miModulo';
    
    - Caso de export total del módulo
    `export default miFunc`           ||| import miFunc from 'miModulo';

  npm package, npm module que se guarda `node_modules`
   - ámbitos privados que tengo que extraer mediante un import.
   
 Hicimos ejercicios difíciles de TypeScript
 TypeScript basics.
 
 Dia 25
 
 ### Angular
 
 FRAMEWORK de desarrollo de FRONTEND basado en JavaScript (TypeScript) junto con otros frameworks como React, Vue, Svelte,... sirven para hacer aplicaciones SPA (Single Page Application).
 
 SPAs: Una web que no hace falta refrescar para actualizarse. Sólo tiene un html. 
 
 Aplicación Angular: 
 
 Instalación a nivel global:
 - Tengo que instalar Node.Js, para utilizar el gestor npm:
 - Instalo el @angular/CLI cliente para línea de comando en angular
 
 Para construir una aplicación angular desde terminal: ng new my-app. 
 
 Único repositorio de Angular: workspace => ng new nombre --createApplication=false  --directory=frontend --interactive=false
 
 Para crear aplicaciones dentro del workspace: ng generate application my-app --style=scss --skipTests=true --routing
    Reconoce que está dentro de un workspace y ya no duplica el fichero Node_modules
    Modifica el angular.json añade una entrada al array projects.
    Genera un subdirectorio llamado projects

El repositorio único permite reutilizar elementos de unos proyectos en otros.


Día 26

Módulos y Routing de Angular

Estructurar el código en funcionalidades dentro de módulos. Los módulos sirven para encapsular, para enrutar de forma lazy (los componentes se cargan en diferido, no con la carga inicial)
  - Módulos de características - Feature Modules
  - Módulos de utilidades compartidas - Shared Modules
  - Módulo raíz - AppModule
  - Módulos reutilizables - Reusables Modules
  
 Para generar módulos: `ng g m commons --routing`
 Dentro de los módulos creamos componentes: `ng g c commons/header --export`
 
 Un componente está formado: una vista(html), una hoja de estilos (scss) y un controlador (.ts)
 Los componentes se incluyen en el componente raíz (app.component) mediante su selector (ej.: app-header) DE FORMA ESTÁTICA
 Los componentes se pueden incluir DE FORMA DINÁMICA mediante la etiqueta (directiva) `<router-outlet>`
  - Hay que enrutar los componentes en el fichero de routing: `AppRoutingModule`.
  - Utilizamos la propiedad routes para redirigir la navegación a un componente.
  
 Día 27
 
 Angular routing:
  - Navegación entre componentes.
  - enrutamiento desde la barra navegación cargando un componente:
    1. Definimos el path y el componente al que se navega - AppRoutingModule: `routes = []`
    2. Definir el routerLink dentro del menú de navegación.
    3. Tiene que existir una etiqueta <router-outlet> que es donde se carga el componente.
        - Si el enrutamiento está definido a nivel de root - el componente se carga en el AppComponent
        - Si el enrutamiento está definido a nivel de root pero como children - el componente se carga dentro del componente padre
  
   - Paso de parámetros a través de la ruta: ":id" - ActiveRoute se trabaja a nivel de componente.ts. Es un objeto asíncrono que devuelve un Observable. Para obtener información de un observable hay que subsribirse al observable.
   
   - Carga diferida de módulos: AppRoutingModule -> loadChild() difiere la carga a un módulo.
  
  Día 28
  
  Pasar información de la clase del componente a la vista.
    - Interpolación de variables: {{ miVariable }} -> Evalúan la expresión que contiene y si resulta en un string lo muestra. Se utiliza para meter texto en las etiquetas o para dar valora a atributos del tipo src, href, ...
     `<p>{{miParrafo}}</p>`
    - Binding de propiedades: Pasamos información de variables a atributos, de cualquier tipo. Esto requiere una notación especial:
      [atributo]='nombreVariable'.
        `<button [disabled]='isTrue'>`
    - Binding de eventos: Asociamos métodos de la clase a eventos de la vista:
      `<button (click) = 'onClick()'>`
  
  Ejercicio de los botones.
  
  Día 29
  
  Directivas: son clases que extienden las propiedades del HTML.
  
    - Añadir o quitar elementos del DOM: **directivas estructurales** ==> *ngFor, *ngIf, ngSwitch
        ```html
        <ul *ngFor="let animal of animals, let i = index, let x = odd">
        <ng-container *ngIf="animal.category === 'felino'">
           <li [ngClass]='{impar:x}'><a href="https://assets/images/{{animal.id}}"> {{animal.name}}</a>
        </ng-container>
        </ul>```
    
    Para hacer un if..else <ul *ngIf="true then cuadro_felino; else cuadro_canino ">
    
    <ng-template #cuadro_felino>
    <li></li>
    </ng-template>
    <ng-template #cuadro_canino>
    </ng-template>
    
   - Directivas de atributos: Modifican estilos del DOM.
     [ngClass] -- añade o quita clases
     [ngStyle] -- para aplicar estilos directamente.
    
        
  - ngModel: Directiva de formularios. Bidireccional. Se pasa información de la plantilla a la clase del componente y viceversa.
    <input [(ngModel)]='miVariable'>
    
    <p>{{miVariable}}</p>
    
    
    Día 30
    
Pipes: Herramientas  para manipular un dato de entrada. Entra un dato y sale un dato convertido.
  
  - Se utilizan en la vista: `{{variable | miPipe }}`
  - Pipes prediseñadas: UppercasePipe, LowercasePipe, Decimal Pipe, CurrencyPipe, JSONPipe, DatePipe,...TitlecasePipe
  - Pipes personalizadas: `ng g pipe miPipe`
  
      Método => transform(dato: any, numMax: number){
      return <<dato transformado>>
      }
  
   - capitalize, smartTruncate  
 
 
 Día 31
 
 Pipe filter => filtrar un Object[] pasando un campo de ese objeto y una cadena a buscar.
 
 El valor del input corresponde al filtro del pipe:  
 
        <ul *ngFor = " for let alimento of foods | filter : 'name' : input.value>
          <li>{{alimento.name}}</li>
        </ul>
 Formularios:
    Form01 --> probar estructuras de Material 
           --> la información se recoge de los campos input y se envía mediante un botón submit
           //html       - <form #form01 = 'ngForm' (ngSubmit)=enviarDatos(form01) >
                      
                      <input #username name='username'> 
                      <button type='submit'>Enviar</button>
                    </form>
          //ts  
          username:string;
          enviarDatos(formulario) {
              this.username = formulario.controls.username.value;
          }
          
          enviarALaBaseDeDatos(username);
        
           
Día 32

Form02: Utilizamos clases para manejar la información.
    `ng g class shared/classes/user`
    
    Una clase está formada por propiedades y métodos representa a un user.
        export class User {
          private _username: string;
          private _password: string;
          
          constructor(){
            this._username = '';
            this._password = '';
          }
          //Métodos accessors
          
          public get username(){
            return this._username;
          }
          public set username(username:string){
            this._username = username;
          }
          
        }
        
      Formulario template-driven con validaciones:
        
        <form #form02 = 'ngForm' >
            <mat-form-field>
              <mat-label>Name</mat-label>
              <input matInput 
                     name = 'username'
                     #username = 'ngModel'
                     ngModel // hace que se generen una serie de propiedades dentro del control: errors, valid|invalid, pristine|dirty, touched|untouched
                     required // username.errors.required => true | false
                  />
              <mat-hint></mat-hint>
<!--              <mat-error *ngIf='username.invalid; else success'> -->
               <mat-error *ngIf='username.dirty || username.touched'>
                   <mat-error *ngIf='username.errors.required'> Error el campo no puede estar vacío</mat-error>
              </mat-error>
            <mat-form-field>
          
        </form>
        <ng-template #success>
        El formulario es correcto
        </ng-template>
        
        
 
 
 
 
 
