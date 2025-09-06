# **Guía 2 de ejercicios de JavaScript**

## Introducción (leer!)
<p>
Esta guía presenta ejercicios prácticos para aprender a integrar el lenguaje JavaScript dentro del framework Flask para poder trabajar en los posteriores trabajos prácticos de la materia.<br>
</p>

<p>
Vamos a practicar como integrar Flask + HTML + CSS + JS, todo trabajando en conjunto. Aprenderemos a invocar código JavaScript desde HTML y a modificar elementos HTML desde JavaScript. También veremos por encima el manejo de propiedades y estilos CSS utilizando código JS.

El uso de Jinja lo vamos a obviar, ya que no es necesario para realizar esta guía.
</p>

<p>
Los únicos ejercicios sí o sí necesarios que hagan son el ejercicio 0 y los ejercicios marcados con el emoji del ojito ("👁️"). El resto de ejercicios son para practicar manejo avanzado del DOM, el cual probablemente no necesiten utilizar a menos que tengan ganas de hacer animaciones copadas 😉.
</p>

<p>
Se incluyen además ejercicios marcados con el emoji del alien ("👽"), que corresponden a temas que <b><i>no entran en la materia y no serán evaluados en los parciales ni en el final</i></b>; pero si los utilizan para el TP final, se los <i>evaluaremos en la defensa</i>, asi que cuidado!
</p>

<center>
⚠️ <i>AVISO: debido a que en la cátedra utilizamos como mínimo el estándar EcmaScript 2015 (ES6), está <span style="text-decoration: underline;">prohibido</span> el uso de la palabra reservada <code>var</code> para declarar variables.</i> ⚠️
</center>

## Indicadores para realizar los ejercicios

### Indicadores de dificultad:
<ol style="list-style-type: disc;">
  <li><i>(Sin emoji)</i> NORMAL</li>
  <li>😈 AVANZADO</li>
  <li>🥵 AVANZADO PLUS</li>
  <li>☢️ PRO</li>
</ol>

### Indicadores misceláneos:
<ol style="list-style-type: disc;">
  <li>👁️ RECOMENDADO QUE LO HAGAN</li>
  <li>😺 OPCIONAL</li>
  <li>👽 TEMAS ADICIONALES (NO LOS VAN A USAR NI LOS EVALUAMOS)</li>
</ol>

## Recursos
### Probar rápido código de HTML+CSS+JS online
  * https://playcode.io/html5
### Guía 1 de JavaScript
  * https://www.w3schools.com/JS/js_es6.asp
  * https://www.w3schools.com/js/js_looping.asp
  * https://www.w3schools.com/js/js_array_methods.asp
  * https://www.w3schools.com/js/js_string_methods.asp
### Manejo del DOM (todos los ejercicios)
  * https://www.w3schools.com/js/js_htmldom.asp
  * https://www.w3schools.com/js/js_htmldom_methods.asp
  * https://www.w3schools.com/js/js_htmldom_document.asp
  * https://www.w3schools.com/js/js_htmldom_elements.asp
  * https://www.w3schools.com/js/js_htmldom_events.asp
  * https://www.w3schools.com/js/js_htmldom_eventlistener.asp
  * https://www.w3schools.com/js/js_htmldom_nodes.asp

## Ejercicios

<p>
Les damos el siguiente template <code>index.html</code> para trabajar en todos los ejercicios:

```
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <body>
    <h1>Mi pagina web</h1>
    <p>Parrafo 1</p>
    <p>Parrafo 2</p>
    <p>Parrafo 3</p>
    <div class="lorem-ipsum">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</div>
    <p id="saludo">Hola Flask!</p>
  </body>
</html>
```

(Todo el código JS se tiene que colocar dentro del archivo `script.js`.)
</p>

## Antes de comenzar (OBLIGATORIO):
### Ejercicio 0:
> Levantar una aplicación web de Flask en el puerto `8993`. Crear un template `index.html` con el contenido mostrado más arriba. Crear un archivo de JavaScript llamado `script.js` que contenga el código para ejecutar una alerta con la frase `"Hola JavaScript!"` <i>(tarea: revisar como se hace una alerta en JS)</i> y enlazarla al template `index.html`.
<br><br>
<i>(Tarea: revisar cómo se enlazan archivos JS en Flask. Pista: etiqueta `script` en HTML + `url_for()` de jinja)</i>

## Ejercicios
### Ejercicio 1 👁️:
> Obtener el objeto del DOM correspondiente al segundo párrafo y cambiarle el texto a `"VIVA HTML"`
<br><br><i>(Pista: ver los recursos `js_htmldom_elements.asp` y `js_htmldom_document.asp`)</i>

### Ejercicio 2 👁️:
> Obtener el objeto del DOM correspondiente al elemento `div` con la clase `"lorem-ipsum"` y mostrar su elemento por la consola.

### Ejercicio 3 👁️:
> Obtener el objeto del DOM correspondiente al párrafo con el id `"saludo"` y mostrar su elemento por la consola.

### Ejercicio 4:
> Remover el último párrafo de la página web. 
<br><br><i>(Pista: ver el recurso `js_htmldom_nodes.asp`)</i>

### Ejercicio 5 😈:
> Dada una lista de cadenas:

	const nombres = ["Parrafo 4", "Parrafo 5", "Parrafo 6"]

> comenzando por el último párrafo de la página, insertar al final del cada párrafo un nuevo objeto DOM de tipo párrafo cuyo contenido sea cada cadena de la lista `nombres`.
<br><br><i>(Pista: ver el recurso `js_htmldom_nodes.asp`).</i>

### Ejercicio 6 😈:
> Insertar un nuevo párrafo con el texto `"PEPITO PEREZ"` <b><i>dentro</i></b> del elemento con el texto `"Párrafo 3"`. 
<br><br><i>(Pista: ver el recurso `js_htmldom_nodes.asp`)</i>

### Ejercicio 7 👁️😈:
> Mostrar una alerta en el navegador Web <i>al hacer click</i> sobre un párrafo, mostrando como mensaje de la alerta el contenido de ese párrafo. 
<br><br><i>(Pista: ver los recursos `js_htmldom_methods.asp`, `js_htmldom_events.asp` y `js_htmldom_eventlistener.asp`)</i>

### Ejercicio 8 😺:
> Cambiar el color del elemento `h1` sin usar CSS. 
<br><br><i>(Pista: hay que modificar una propiedad del DOM)</i>

### Ejercicio 9 👁️🥵:
> Crear un botón para ocultar todos los párrafos al ser presionado, y al ser presionado de vuelta, volver a mostrar todos los párrafos.
<br><br><i>(Pista: buscá en Google la "property" para ocultar un elemento del DOM)</i>

### Ejercicio 10 😺☢️:
> Crear un botón `"Ocultar un párrafo"` para ocultar todos los párrafos al ser presionado de 1 en 1 y de abajo hacia arriba, hasta que no quede ninguno visible. Luego, cambiar el texto del botón a `"Mostrar un párrafo"` y hacer el camino inverso, es decir, ir mostrando nuevamente los párrafos de 1 en 1 y de arriba hacia abajo, y cuando queden todos los párrafos visibles otra vez, volver a cambiar el texto del botón a `"Ocultar un párrafo"`. 
<br><br><i>NOTA: la cantidad de párrafos no se conoce (no es 3 necesariamente).</i>

### Ejercicio 11 👽:
> Lectura: Uso de `fetch` y objetos de tipo `Promise`:
<br><br> https://www.w3schools.com/js/js_promise.asp
<br><br> https://www.freecodecamp.org/espanol/news/javascript-fetch-api-para-principiantes/

### Ejercicio 12 👽:
> Lectura: Uso de `async` y `await` en conjunto con los objetos de tipo `Promise`:
<br><br> https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Statements/async_function
<br><br> https://es.javascript.info/async-await