## Ejercicio 1: Menú de navegación
Crea un menú de navegación donde:
- Los enlaces no visitados sean azules
- Los enlaces visitados sean morados
- Al pasar el ratón, los enlaces tengan fondo amarillo
- Al hacer clic, los enlaces se pongan en negrita

```html
<nav>
    <a href="#inicio">Inicio</a>
    <a href="#servicios">Servicios</a>
    <a href="#contacto">Contacto</a>
</nav>
```

## Ejercicio 2: Lista rayada
Crea una lista donde las filas impares tengan fondo gris claro y las pares fondo blanco.

```html
<ul class="lista-tareas">
    <li>Comprar leche</li>
    <li>Estudiar CSS</li>
    <li>Hacer ejercicio</li>
    <li>Leer un libro</li>
    <li>Cocinar cena</li>
</ul>
```

## Ejercicio 3: Formulario con validación visual
Crea estilos para un formulario donde:
- Los campos obligatorios tengan un borde izquierdo rojo
- Los campos con foco tengan un borde azul brillante
- Los campos válidos tengan un borde verde
- Los campos inválidos tengan un borde rojo y fondo rosa claro

```html
<form>
    <input type="text" required placeholder="Nombre">
    <input type="email" required placeholder="Email">
    <input type="tel" placeholder="Teléfono (opcional)">
</form>
```

## Ejercicio 4: Botones con estados
Diseña un botón que:
- Tenga fondo azul normalmente
- Cambie a azul más oscuro al pasar el ratón
- Se hunda visualmente al hacer clic (usando transform)
- Esté en gris y no se pueda hacer clic cuando esté deshabilitado

```html
<button>Enviar</button>
<button disabled>Deshabilitado</button>
```

## Ejercicio 5: Galería de imágenes
Crea una galería donde:
- La primera imagen tenga un marco dorado
- La última imagen tenga un marco plateado
- La tercera imagen de cada grupo tenga más opacidad

```html
<div class="galeria">
    <img src="foto1.jpg" alt="Foto 1">
    <img src="foto2.jpg" alt="Foto 2">
    <img src="foto3.jpg" alt="Foto 3">
    <img src="foto4.jpg" alt="Foto 4">
    <img src="foto5.jpg" alt="Foto 5">
    <img src="foto6.jpg" alt="Foto 6">
</div>
```

## Ejercicio 6: Tabla de precios
Estiliza una tabla donde:
- La primera fila (encabezado) tenga fondo oscuro y texto blanco
- Las filas pares tengan fondo gris claro
- Al pasar el ratón sobre una fila, esta se ilumine con fondo amarillo claro

```html
<table>
    <tr>
        <th>Producto</th>
        <th>Precio</th>
    </tr>
    <tr>
        <td>Producto A</td>
        <td>10€</td>
    </tr>
    <tr>
        <td>Producto B</td>
        <td>15€</td>
    </tr>
    <tr>
        <td>Producto C</td>
        <td>20€</td>
    </tr>
</table>
```

## Ejercicio 7: Checkboxes personalizados
Estiliza una lista de tareas donde:
- Los items con checkbox marcado tengan el texto tachado y en gris
- Los items sin marcar estén en negro normal

```html
<ul class="tareas">
    <li><input type="checkbox" id="t1"> <label for="t1">Tarea 1</label></li>
    <li><input type="checkbox" id="t2" checked> <label for="t2">Tarea 2</label></li>
    <li><input type="checkbox" id="t3"> <label for="t3">Tarea 3</label></li>
</ul>
```

## Ejercicio 9: Selector avanzado
Estiliza una lista donde:
- Todos los elementos excepto el tercero tengan punto negro
- El tercer elemento tenga punto rojo y esté en negrita

```html
<ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
    <li>Elemento 3</li>
    <li>Elemento 4</li>
    <li>Elemento 5</li>
</ul>
```

## Ejercicio 10: Campos vacíos
Crea estilos donde:
- Los divs vacíos se oculten automáticamente
- Los divs con contenido tengan padding y borde

```html
<div class="contenedor"></div>
<div class="contenedor">Este tiene contenido</div>
<div class="contenedor"></div>
<div class="contenedor">Este también</div>
```