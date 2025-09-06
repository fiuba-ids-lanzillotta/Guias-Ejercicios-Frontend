# **Guía 1 de ejercicios de JavaScript**

## Introducción
<p>
Esta guía presenta ejercicios prácticos para aprender el lenguaje JavaScript.<br>
✨La integración de JavaScript con Flask se ve en la <i>guía 2 de JS.</i>✨
</p>

<p>
ℹ️ Para resolver los ejercicios de esta guía, utilicen la consola de desarrollador del navegador Web.

En Chrome & Firefox hay 2 formas de abrir dicha consola:
* Pulsan <i>CTRL + SHIFT + J</i>
* Pulsan <i>F12</i> y se van al apartado <i>Console</i>
</p>

<p>
	Indicadores de dificultad:
	<ol style="list-style-type: disc;">
		<li><i>(Sin emoji)</i> NORMAL</li>
		<li>😈 AVANZADO</li>
    <li>😺 OPCIONAL</li>
    <li>👁️ RECOMENDADO QUE LO HAGAN</li>
	</ol>
</p>
<p>

<p>
Recursos (por favor, úsenlos):

* Sintaxis ES6 -> https://www.w3schools.com/JS/js_es6.asp
* Bucles `for` -> https://www.w3schools.com/js/js_looping.asp
* Listas       -> https://www.w3schools.com/js/js_array_methods.asp
* Strings      -> https://www.w3schools.com/js/js_string_methods.asp
</p>

<center>
⚠️ <i>AVISO: debido a que en la cátedra utilizamos como mínimo el estándar EcmaScript 2015 (ES6), está <span style="text-decoration: underline;">prohibido</span> el uso de la palabra reservada <code>var</code> para declarar variables.</i> ⚠️
</center>

## Ejercicios

### Ejercicio 1:
> Imprimir por consola `"Hola mundo! Tengo N años"` reemplazando `N` por la <i>edad de ustedes</i>, por ejemplo, `21`.

### Ejercicio 2:
> Dada una lista de números:

	const nums = [2, 17, 39, 0, 20, -6]

> imprimir por pantalla `nums` en orden ascendente (números de menor a mayor).

### Ejercicio 3 👁️:
> Dada una lista de cadenas:

	const profes = ["pala", "leo", "caro", "bruno", "martin", "tomi", "flavio", "franco"]

> imprimir por pantalla solamente por los nombres de los profes que tengan un largo de <i>exactamente</i> `4` caracteres. Los nombres filtrados deben estar guardados en una lista nueva llamada `profes2`.

### Ejercicio 4:
> Dado un <i>diccionario/mapa/array asociativo/objeto</i> con la siguiente estructura:
```
const person = { 
  "nombre": "Pepito", 
  "apellido": "Perez", 
  "edad": 27, 
  "isAdmin": true 
}
```
> cambiar el apellido de `person` a `"Messi"` e imprimir `person` por pantalla con el nuevo nombre.

### Ejercicio 5 😈:
> Dada una lista de números:

	const nums = [1, 2, 3, 4, 5, 6]

> y una <i>"función que recibe un número por parámetro y devuelve otro número"</i>:
```
const toSquared = function (x) { 
  return x * x 
}
```
> crear una nueva lista `squared` que contenga el resultado de aplicar la funcion `toSquared` a cada elemento de la lista `nums`, e imprimir esa nueva lista por pantalla. ¿Qué son los números de la lista nueva? <i>(Pista: podés usar uno de los métodos de `Array` en JS mas conocidos)</i>.

### Ejercicio 6 😺:
> Dada una lista de listas de números:

	const nums = [[1, 2, 3], [4, 5]]

> <i>"aplanar"</i> la lista e imprimirla por pantalla. La nueva lista tiene que quedar de la siguiente forma:
```
const nums2 = [1, 2, 3, 4, 5]
```
> <i>(Pista: podés usar uno de los métodos de `Array` de JS)</i>.

### Ejercicio 7 👁️ 😈:
> Reemplazar todas las ocurrencias del caracter guion (`"-"`) por el caracter espacio en blanco (`" "`) en la siguiente cadena/string:

	const saludo = "Hola-soy-pepito-perez"

> luego insertar una coma (`","`) justo después del `"Hola"` y un signo de exclamación (`"!"`) al final. La frase final debe quedar: 
<br><br>
<i>"Hola, soy pepito perez!"</i> .
<br><br>
Imprimir la frase resultante por pantalla.

### Ejercicio 8 👁️ 😺:
> Revisar el uso de los operadores `==` <i>(loose equality)</i> y `===` <i>(strict equality)</i> en JavaScript.
<br>https://www.w3schools.com/Js/js_comparisons.asp
