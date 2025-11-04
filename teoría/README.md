# Pseudoclases en CSS

## ¿Qué son las pseudoclases?

Las pseudoclases son palabras clave que se añaden a los selectores CSS y que especifican un **estado especial** del elemento seleccionado. Se escriben con dos puntos (`:`) seguidos del nombre de la pseudoclase.

```css
selector:pseudoclase {
    propiedad: valor;
}
```

## Pseudoclases más comunes

### 1. Pseudoclases de enlaces

#### `:link`
Selecciona enlaces que aún no han sido visitados.

```css
a:link {
    color: blue;
    text-decoration: none;
}
```

#### `:visited`
Selecciona enlaces que ya han sido visitados.

```css
a:visited {
    color: purple;
}
```

#### `:hover`
Selecciona un elemento cuando el cursor pasa sobre él.

```css
a:hover {
    color: red;
    text-decoration: underline;
}
```

#### `:active`
Selecciona un elemento mientras está siendo activado (por ejemplo, mientras se hace clic).

```css
a:active {
    color: orange;
}
```

**Orden recomendado para enlaces:** `:link` → `:visited` → `:hover` → `:active` (regla **LVHA**)

### 2. Pseudoclases de formularios

#### `:focus`
Selecciona un elemento cuando tiene el foco (por ejemplo, al hacer clic en un input).

```css
input:focus {
    border: 2px solid blue;
    outline: none;
}
```

#### `:checked`
Selecciona elementos checkbox o radio que están marcados.

```css
input:checked {
    accent-color: green;
}
```

#### `:disabled`
Selecciona elementos deshabilitados.

```css
button:disabled {
    opacity: 0.5;
    cursor: not-allowed;
}
```

#### `:enabled`
Selecciona elementos habilitados.

```css
input:enabled {
    background-color: white;
}
```

#### `:required`
Selecciona elementos de formulario que son obligatorios.

```css
input:required {
    border-left: 3px solid red;
}
```

#### `:optional`
Selecciona elementos de formulario que son opcionales.

```css
input:optional {
    border-left: 3px solid gray;
}
```

#### `:valid` e `:invalid`
Seleccionan elementos según su validación.

```css
input:valid {
    border-color: green;
}

input:invalid {
    border-color: red;
}
```

### 3. Pseudoclases estructurales

#### `:first-child`
Selecciona el primer hijo de su elemento padre.

```css
li:first-child {
    font-weight: bold;
}
```

#### `:last-child`
Selecciona el último hijo de su elemento padre.

```css
li:last-child {
    border-bottom: none;
}
```

#### `:nth-child(n)`
Selecciona elementos basándose en su posición.

```css
/* Elementos pares */
tr:nth-child(even) {
    background-color: #f2f2f2;
}

/* Elementos impares */
tr:nth-child(odd) {
    background-color: white;
}

/* Cada tercer elemento */
li:nth-child(3n) {
    color: red;
}

/* El quinto elemento */
li:nth-child(5) {
    font-size: 20px;
}
```

#### `:nth-last-child(n)`
Como `nth-child` pero contando desde el final.

```css
li:nth-last-child(2) {
    color: blue;
}
```

#### `:first-of-type`
Selecciona el primer elemento de su tipo entre sus hermanos.

```css
p:first-of-type {
    font-size: 18px;
}
```

#### `:last-of-type`
Selecciona el último elemento de su tipo.

```css
p:last-of-type {
    margin-bottom: 0;
}
```

#### `:nth-of-type(n)`
Selecciona elementos de un tipo específico según su posición.

```css
p:nth-of-type(2) {
    font-style: italic;
}
```

#### `:only-child`
Selecciona elementos que son el único hijo de su padre.

```css
li:only-child {
    list-style: none;
}
```

### 4. Pseudoclases de negación

#### `:not()`
Selecciona elementos que NO coinciden con el selector especificado.

```css
/* Todos los párrafos excepto los de clase 'especial' */
p:not(.especial) {
    color: gray;
}

/* Todos los inputs excepto los de tipo submit */
input:not([type="submit"]) {
    border: 1px solid #ccc;
}
```

### 5. Otras pseudoclases útiles

#### `:empty`
Selecciona elementos que no tienen hijos (ni texto).

```css
div:empty {
    display: none;
}
```

#### `:target`
Selecciona el elemento cuyo ID coincide con el fragmento de la URL.

```css
:target {
    background-color: yellow;
    border: 2px solid orange;
}
```

#### `:root`
Selecciona el elemento raíz del documento (generalmente `<html>`).

```css
:root {
    --color-primario: #3498db;
    --fuente-principal: Arial, sans-serif;
}
```

## Combinación de pseudoclases

Puedes combinar múltiples pseudoclases:

```css
/* Botón deshabilitado al pasar el ratón */
button:disabled:hover {
    cursor: not-allowed;
}

/* Primer párrafo que no tiene clase 'intro' */
p:first-of-type:not(.intro) {
    margin-top: 0;
}
```
