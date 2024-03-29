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
  
 Día 33
 
 Formularios Reactivos: programación reactiva:
    - Importar en el módulo: `ReactiveFormModule`,
    - Crear un formulario reactivo:
      - Instaciamos la clase FormGroup: 
      ```ts
      formGroup = new FormGroup({
      name: new FormControl('', [Validators.required, Validators.minLength(4),...]),
      dni: new FormControl()
      })
      ```
     - Inyectando el Servicio FormBuilder en el constructor del componente: `constructor(private formBuilder: FormBuilder){}`
     ```ts
     formGroup: FormGroup;
      ngOnInit(){ 
      this.formGroup = this.formBuilder.group({
      name:['',[Validators.required]],
      dni:['',[Validators.required]]
      })
      }
      ```
    - Conectar el formulario al HTML:
     ```ts
     <form [formGroup]='formGroup' >
     <input [formGroupName]='name'>
     <input [formGroupName]='dni'>
     </form>
     ```
 Día 34
    Jerarquía de componentes:
    
    - smart components | container components: componentes contienen la lógica del componente
    - dumb components | presentational components: componentes contien la vista del componente
    
    - El componente que tiene la lógica tiene que pasar información a los componentes que tienen vistas.
    - Los componentes que tienen vistas pasan información del formulario al comp. contenedor.
    
    Se declaran propiedades que intercambian datos con el decorador: @Input()
    Se declaran métodos que envían información al contenedor con @Output(). Son instancias de la clase EventEmitter<>.
    
    Ejercicio incorporar los botones: borrar y editar.

Día 35
    Services:
    
    - Funcionalidades no directamente relacionadas con la presentación y compartidas por distintos componentes. Ej: interacción con el back-end, autenticación, logging, etc.
    
    - `ng g s <nombre_servicio>`
    
    - Clase con un decorador @Injectable -Hace que la clase se pueda inyectar como dependencia de otras clases.
    - Declarado por un provider: providerIn 'root' dentro del decorador @Injectable.
            @ngModule(providers:[])
            
    - Declarar un parámetro en el constructor de la clase donde se quiere inyectar el servicio:
        ```ts
        ...
        constructor(private nombreServicio: NombreServicio){}
        ```
        
Día 36

  Servicios HTTP, se utilizan para hacer peticiones vía HTTP: GET, POST, PUT, DELETE,...
    Se implementan con una API HTTPClient.
    Para utilizar el HTTPCLient: importar el `HTTPClientModule` desde el `App.Module` e inyectar el servicio `HTTPClient` en el constructor de la clase donde se vayan a hacer las peticiones, normalmente otro servicio.
    
  Los métodos de HTTP, devuelven Observables.
    - Observables: Envolvemos un stream de datos asíncrono que va devolviendo información a los métodos que estén suscritos al observable. FUncionan de forma similar a las Promesas, pero van emitiendo de forma continua en el tiempo.
    - 2 tipos de observables:
      - Frios: Observables sólo devuelven información cuando se suscriben.
      - Calientes: Emiten información independientemente de que haya suscriptores.
    
    - Se implementan a partir de la librería rxjs
    -   `pipe`: concatena funciones de observables. 
    -   `map`, `merge`, `findIndex`,...
    
 Día 37
 
  Una app desde 0: ORDER-LIST:
      Servidor: json-server
      App: Angular y HTTPClient
      Trello: Kanban
      
    1. BBDD: Mis datos son estructurados y necesitan estar relacionados entre si. Mis datos alimentan un front-end y lo que quiero es mucha rapidez i/o, BBDD relacionales o no-sql.
    2. Front-end: Diseño mis pantallas, diseño el wireframe, navegación, componentes.
    3. Para trabajar el front-end no hacen falta datos. Array de datos. placeholders de APIs, de fotografías. 
    4. Arquitectura de la aplicación: Estructura de directorios, módulos, servicios, componentes, clases, interfaces, etc.
    5. Routing.
    6. Funcionalidades x iteración de programación: Pasos del 6 al 8 hasta terminar el proyecto.
        - User stories: yo como usuario quiero logarme en la aplicación con mi nombre de usuario y mi password.
              - UserComponent
                    . Se cargará desde: la url raíz
                    . Validaciones de front-end
                    . Servicio de autenticación
                          Métodos relacionados.
                    . Estrategias de autenticación: bearer token, basic-auth, o-auth (facebook, google, ...)
                
    7. Trabajamos con servidores de desarrollo para hacer pruebas. Integración, Regresión.
    8. MVP al final de la iteración se sube a un servidor de preproducción. Repetición de pruebas. Se enseña la app al cliente.
    (firebase)
    9. Subida a producción pruebas con numero limitado de usuarios.(beta)
    10. Aplicación pasa a versión estable. Los cambios vienen por ramas de hotfix, actualización, etc.
    
   Día 37    
        
   Trabajar con el HTTPCLient la parte de refrescar la lista después de hacer un create, delete, update
     
    Angular.http nos devuelve un Cold Observable. Lo tenemos que transformar en un Hot Observable con BehaviourSubject de la librería rxjs.
    
    Como utilizar cloud firebase.google.com para almacenar datos:
      - Crear un proyecto dentro del cloud
      - Crear una aplicación web
      - Copiamos la variable firebaseConfig dentro del fichero de environments.ts
      - `ng add @angular/fire`
      - Importar en el AppModule:
          - AngularFireModule.initialize.app('firebaseConfig');
          - AngularFirestoreModule
          
      - Creamos un servicio para interactuar con Firebase:
          - Inyectar el AngularFirestore
          - Creamos los CRUD's
          
  Día 38
  
  Subida a producción + retrospectiva
  
  Día 39
  
  Montando aplicación TODO-LIST. Para probar ciclo de vida de un componente:
    Etapas básicas de creación y destrucción: instanciación de la clase (`constructor`), `ngOnInit` (interfaz OnInit), `ngOnDestroy`(interfaz OnDestroy)
    Etapas cíclicas de detección de cambios: `ngOnChanges(SimpleChages)`, `ngDoCheck()`, `ngAfterViewInit`, `ngAfterViewChecked`
    Etapas relacionadas con la proyección de contenido (project-content): `ngAfterContentInit`,`ngAfterContentChecked`
    
    TODO-LIST: Componentes+Servicio+Interface+Firebase.
    
Día 40

  Seguimos con los hooks: ejemplos de `ngOnChanges(SimpleChanges)`
  
  Modal (Material se llaman dialogs)
    Un componente que está controlado por otro componente. 
    - Controlador abre el modal pasándole información.
    - El propio modal es el responsable de cerrarse y enviar información al controlador.
   
   Material Dialogs: 
      - Crear el componente y dentro del módulo se tiene que incluir como __entry component__
      - En el componente __controlador__: inyectamos el MatDialog.
          Definimos un método de abrir Modal: 
              - Configuración del modal: MatDialogConfig donde configuramos el modal
                    - Incluimos los datos a pasar al modal.
              - const dialogRef =  matDialog.open(componente,config)
              - dialogRef.afterClosed().subscribe(data => hago algo con los datos)
     - En el __modal__, definimos los métodos de cerrar el modal:
              - inyectar una propiedad: @Inject() MAT_DIALOG_DATA, data
              - invocamos al método close para cerrar el modal.
              
Día 41

  Estuvimos de nuevo montando la aplicación desde 0. 
  Arquitectura:
    Modules:
    - Componentes presentacionales, dumb components, etc.
    - Componentes controladores, featured components.
    Shared:
    - services: auth.service, user.service,
    - models: clases y/o interfaces
    - guards: auth.guard
    - material
    - components comunes y reutilizables: header, hero, sidebar
    - helpers:
        - interceptors
        - fake-backend
  Autenticación:
    - Enviamos un usr/password desde la app al backend.
    - El backend responde con un token de autenticación (jwt).
    - El cliente guarda el token en el localstorage
    - El cliente envía el token con cada petición de datos.
  
 Día 42
 
 Aplicación angular-auth
 
  - Login
      . Formulario (componente: enrutable (featured component) + presentacional)
      
  1. Aplicación se carga: ruta http://localhost:4200/ => homecomponent
  2. Navega al formulario de login: submit --> @output
  3. LoginComponent carga el servicio de envío de datos
  4. EL servicio AuthService envía información al backend: fake-backend(interceptors) o firebase authentication
  5. Recibe un token de authorization: JWT y lo guarda en localstorage.
  6. Navegas al componente permitido: home o userprofile, etc.
  
  - Profile
  
  1. Obtener los datos del backend. Para ello introducimos token en la cabecera de la petición de datos.
  
  - Register
  
  1. Carga el servicio: AuthService o UserService
  2. Método que es un createUser sin authorization.No permite datos duplicados.
  3. VerifiedEmail --> Firebase
  4. Navegue al Login.
  
  . Encender y apagar elementos de la barra de navegación. Con un flag dentro de localstorage.
  . Proteger las rutas del acceso directo desde el navegador. Mediante Guards. 
  
  
  
  
  - Register
  - Profile
    
  Día 43 - 50
  - Projecte
  
  Día 51
  - Testing Intro
  
      - Testing aporta valor a la empresa y al usuario:
        - Corregir errores,
        - Comprobar funcionalidad,
        - Optimizar procesos
        
      - A nivel de programadores podemos enfrentar dos tipos de testing: Unit Tests y e2e (tests de integración, etc.)
      - Unit Tests: Se basan en el principio de las 3As:
          - Arrange: Ámbito y el escenario de prueba. Cómo aislar nuestra suite de pruebas.
          - Act: Los test cases. Qué queremos probar
          - Assert: La comprobación del resultado. Básicamente es un true|false.
      - Isolated Test Units: Probamos clases.
          - Probamos clases que no tienen dependencias. 
          - Ejemplo del cálculo IMC.
      - Estructura de un test:
      ```ts
        Describe('Test de la clase',()=>{
            
            beforeEach(()=>{
            
              classToTest = new Class();
            
            })
            
            it('debería instanciar la clase',()=>{
              expect(classToTest).toBeTruthy();
            })
            
        })
      ```
  Día 52
  - Testing components
      Tener en cuenta que el componente tiene dos partes:
        - La clase
        - La vista
  - Dependencias de un componente:
        - Necesita un módulo, --> `TestBed.configureTestingModule()` genera NgModule
        - Inyectar un servicio para tener datos. --> `TestBed.inject(<<nombre del servicio>>)`
        
  - componente = new Componente();
        - No tendría acceso a su vista.
        
  - fixture = TestBed.createComponent(Componente);
         - Para acceder a la parte de la clase: fixture.componentInstance
         - Para acceder al DOM: fixture.nativeElement | fixture.debugElement.nativeElement
  - Para poder testar **cambios** en el componente, necesitamos disparar la máquina de detección de cambios:
        - fixture.detectChanges();
  - Hacemos los asserts:
        - expect(fixture.nativeElement.querySelector('.movie').value).toBe('miPelicula');
  
  Colaboradores:
    - Funciones especiales que simulan comportamientos:
        - Sustituyen al servicio: mocks y spies.
        - Valores de retorno de una api: stubs.
    
Día 53

  - Aplicación favorite-movies:
    - Pruebas con smart components y dumb components
      - TestBed y Fixtures
    - Servicios HTTP:
      - Inyectar el cliente de Test: HTTPTestController
      - expectations:
        - expectOne()
        - req.request.url
        - req.request.method
        - ...
       - req.flush(datosMockeados)
       - http.verify()
       
   - Aplicación snappCar: caso de entrevista de trabajo.
    
  Día 1 - Ionic Intro & Web Components  
  
  Día 2 - Ionic Components
    
    Layout en Ionic:
       - Básico: 
       ```html
       <ion-app>
          <ion-header>
          <ion-content>
      
      - Responsive Grid:---> Gallery
        <ion-grid> // Divide el viewport en 12 columnas
          <ion-row>
            <ion-col size-lg="3" size-md="4" size-sm="6" size="12">
                <ion-img>
                <ion-card> ---> Cards
                
     Ejemplos de grid.

      <ion-virtual-scroll> permite la carga diferida de elementos en listas largas.
          <ion-img> carga imágenes en diferido
 
 
 
