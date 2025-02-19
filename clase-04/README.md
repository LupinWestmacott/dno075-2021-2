# Infografía digital: HTML, CSS y JavaScript

### Clase 04 → 06/09/202

A diferencia de las tres clases anteriores, el contenido de la clase lo encuentran a continuación:
 
- [HTML](https://github.com/profesorfaco/dno075-2021-2/wiki/HTML) es un lenguaje descriptivo que podemos reconocer por sus elementos demarcados con `<etiqueta atributo="…"></etiqueta>`.

- [CSS](https://github.com/profesorfaco/dno075-2021-2/wiki/CSS) es un lenguaje descriptivo que podemos reconocer la regla que se estructura con `selector{propiedad:valor;}` que podemos encontrar en el documento HTML entre etiquetas `<style></style>` o vincularse mediante `<link rel="stylesheet" href="…" />`.

- [JavaScript](https://github.com/profesorfaco/dno075-2021-2/wiki/JavaScript) que aporta interactividad a través de la manipulación de la estructura del documento HTML (el DOM), sin manipular el documento mismo; no cambia el código fuente que describe el sitio, pero pude modificar la interpretación de tal descripción según ciertas condiciones: La hora en el lado del cliente, la cantidad de scroll que haya hecho quien lee, sus respuestas en un formulario, etc.

Del listado recién presentado, el "complicado" podría ser JavaScript, porque es el que trabaja directamente con las "complejidades" de la interacción. Con JavaScript (y sus bibliotecas) se programa. Con los demás se describe.

Para esta clase, lo important es tener claro que **HTML (HyperText Markup Language) es un lenguaje estándar que describe la estructura de las páginas web (qué es lo que contiene la página)**. Y este se complementa con otro lenguaje estándar, el **CSS (Cascading Style Sheets) que describe la presentación de las páginas web (cómo se muestra lo que contiene la página)**. 

**Existen marcos de trabajo de código abierto que nos pueden ayudar a avanzar más rápido en la construcción de una infografía digital desde relaciones predefinidas de HTML y CSS**. Por su popularidad, corresponde mencionar a:

- [Bootstrap](https://getbootstrap.com/): *The world’s most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.*

- [Foundations](https://get.foundation/): *The most advanced responsive front-end framework in the world* 

- [Semantic UI](https://semantic-ui.com/): *A development framework that helps create beautiful, responsive layouts using human-friendly HTML*

Hemos trabajado dos clases con [Bootstrap](https://getbootstrap.com/), con lo que nos hemos relacionado con su lógica de las 12 columnas (`col`) en las que se puede dividir una fila (`row`) que se va ajustando dentro de un contenedor (`container`), una lógica con la que [Bootstrap](https://getbootstrap.com/) se adapta a distintos tamaños de pantalla.

Digamos que en este contenedor (`container`) quiero dividir la fila (`row`) en dos partes del mismo ancho, para que una se muestre al lado de la otra. Para lograrlo debo tomar 6 y 6 columnas (`col`). Dentro del cuerpo del documento HTML, esto se vería así:

```
<div class="container">
 <div class="row">
  <div class="col-6">Primera división</div>
  <div class="col-6">Segunda división</div>
 </div>
</div>
```

Ahora, quiero hacer la misma división pero sólo desde una pantalla mediana ([mayor a 768px de ancho](https://getbootstrap.com/docs/5.0/layout/breakpoints/#available-breakpoints)). En las pantallas que tengan un ancho menor, ambas divisiones ocuparán todo el ancho, poniéndose la segunda debajo de la primera:

```
<div class="container">
 <div class="row">
  <div class="col-md-6">Primera división</div>
  <div class="col-md-6">Segunda división</div>
 </div>
</div>
```

Cambiemos de ejemplo, considerando que Robert Bringhurst (2008) escribe:

> La cantidad que se considera satisfactoria como longitud de línea para una página de una sola columna compuesta en una fuente con remates va entre 45 u 75 caracteres. La línea de 66 caracteres (contando tanto las letras como los espacios en blanco) se considera ideal. Para un trabajo de varias columnas, 40 a 50 caracteres es un buen promedio.

Podríamos necesitar una imagen a todo lo ancho de la fila dentro del contenedor, y bajo ella un párrafo centrado que utilice menos columnas en la medida que éstas se ensanchan junto a la pantalla, así mantener una anchura de párrafo cómoda a la lectura. El código del documento completo debería verse así:

```
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
    <title>Hola mundo</title>
  </head>
  <body>
  <div class="container">
   <div class="row">
    <div class="col-12">
     <img src="https://picsum.photos/1600/900?grayscale" class="w-100 my-4" alt="esta es una imagen random">
    </div>
    <div class="col-11 col-sm-10 col-md-9 col-lg-8 col-xl-7 col-xxl-6 mx-auto">
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla in molestie felis, eget egestas lacus. Etiam orci magna, dignissim at dolor eu, finibus molestie mi. Suspendisse fringilla sem magna, eget pharetra orci faucibus sit amet.</p>
    </div>
   </div>
  </div>    
  </body>
</html>
```

Una vez leído y comprendido el código en el ejemplo recién presentado, se puede pasar al ejercicio.

- - - - - - - 

#### Ejercicio

Pendiente

- - - - - - - 

#### Tarea

Revisar la página web JavaScript Para Gatos :cat:  

https://jsparagatos.com/

- - - - - - - 

###### [← CLASE PASADA](https://github.com/profesorfaco/dno075-2021-2/tree/main/clase-03) — [CLASE SIGUIENTE →](https://github.com/profesorfaco/dno075-2021-2/tree/main/clase-05) 
