# **Guía de ejercicios de front-end (integración con Flask)**

## Introducción
Esta guía presenta ejercicios prácticos para aprender HTML, CSS y cómo integrar dichos lenguajes con el framework Flask.

<p>
	Indicadores de dificultad:
	<ol style="list-style-type: disc;">
		<li><i>(Sin emoji)</i> NORMAL</li>
		<li>😈 AVANZADO</li>
		<li>☢️ PRO</li>
	</ol>
</p>
<p>
	Para los ejercicios <i>5a, 5b, 5c, 5d, 5e y 5f</i>, revisar estos recursos:
		<li><code>https://playcode.io/html5</code></li>
		<li><code>https://fonts.google.com</code></li>
	</ol>
</p>


## Ejercicios

### Ejercicio 1:
> Desarrollar una aplicación web de Flask que se levante en el puerto `5001`, con el modo "debug" en `True`.

### Ejercicio 2:
> Desarrollar una aplicación web de Flask que se levante en el puerto `5002` y que al llamar a la ruta `"/"` desde el navegador web, devuelva un texto HTML que contenga la frase "Hola Flask!" dentro de una etiqueta `h1`.
<br><br>
<i>Pista: `http://localhost:5002/` debe mostrar en el navegador web `"Hola Flask!"`</i>

### Ejercicio 3:
> A la aplicación del ejercicio 2 reemplazar el texto `"Hola Flask!"` por un template en el archivo `index.html` con el mismo texto.
<br><br>
<i>(Tarea: revisar como se crea un template en Flask)</i>

### Ejercicio 4:
> A la aplicación del ejercicio 2 agregar una función `datos_contacto()` que esté enlazada a la ruta `"/contacto"`. Dicha ruta, al ser invocada desde el navegador web debe devolver un "template" llamado `contacto.html` que contenga en su interior el siguiente texto:
<br><br>
Hola, soy `(poné tu nombre acá)` y mi padrón es `(poné tu padrón acá)`.

### Ejercicio 5:
> A la aplicación del ejercicio 2 agregar un archivo CSS llamado `styles.css` <i>(tarea: revisar donde van los archivos CSS en Flask)</i> que contenga un selector de etiqueta `h1` que cambie el color del texto a rojo, y enlazarlo al archivo `index.html`.

### Ejercicio 5a:
> Agregar un estilo de CSS que al hacer click en el texto, el texto cambie su color a verde.

### Ejercicio 5b:
> Agregar un estilo de CSS que cambie el color del fondo de la página a `#36274a` (violeta azulado oscuro).

### Ejercicio 5c:
> Agregar un estilo de CSS que subraye el texto con línea punteada.

### Ejercicio 5d 😈:
> Agregar un estilo de CSS que cambie la "font" (fuente) del texto a `"Noto Sans"` <i>(Pista: buscar como insertar fuentes externas en HTML)</i>.

### Ejercicio 5e 😈:
> Agregar un estilo de CSS que al pasar el mouse por encima del texto, el texto se amplifique <i>(Pista: propiedad `transform` en CSS)</i>.

### Ejercicio 5f 😈:
> Al estilo anterior agregar la propiedad de que la animación dure `1.5` segundos <i>(Pista: propiedad `transition` en CSS)</i>.

### Ejercicio 6 😈:
> Desarrollar una segunda aplicación web de Flask que se levante en el puerto `5003` que contenga en el archivo principal (`index.html`) un elemento de tipo `button` que al hacerle click redirija el navegador a `http://localhost:5002/contacto` (la aplicación del ejercicio 4).
<br><br>
<i>Pista: hay que levantar las 2 aplicaciones al mismo tiempo</i>.

### Ejercicio 7 ☢️:
> Desarrollar una aplicación web en flask que se levante en el puerto `4856` y que en la ruta `"/maps"` muestre un mapa de <i>Google Maps</i>.
<br><br>
<i>Recursos: https://www.maps.ie/create-google-map/</i>

### Ejercicio 8 😈:
> A la aplicación del ejercicio 7 agregar la ruta `"/"` que redirija el navegador web automáticamente a la ruta `"/maps"`.
<br><br>
<i>Pista: buscar cómo se utilizan las funciones `redirect()` y `url_for()` en Flask</i>.