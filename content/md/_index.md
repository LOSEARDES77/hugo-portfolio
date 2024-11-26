+++
title = 'Sintaxis de Markdown'
date = 2024-11-26T09:28:05+01:00
draft = false
+++

## Párrafo

Al escribir texto normal, básicamente estás escribiendo un párrafo.

```md
Esto es un párrafo.
```

Esto es un párrafo.

---

## Encabezados

Hay 6 variantes de encabezamiento. El número de símbolos «#», seguidos de texto, indica la importancia del encabezamiento.

```md
# Título 1

## Título 2

### Título 3

#### Título 4

##### Título 5

###### Título 6
```

# Título 1

## Título 2

### Título 3

#### Título 4

##### Título 5

###### Título 6

---

## Énfasis

Modificar el texto es muy limpio y fácil. Puedes poner el texto en negrita, cursiva y tachado.

```md
Usando dos asteriscos **este texto está en negrita**.
Dos guiones bajos **también sirven**.
Pongámoslo _en cursiva_.
Lo has adivinado, _un guión bajo también es suficiente_.
¿Podemos combinar \__ambos_?\*\* Absolutamente.
¿Y si quiero tachar?
```

Usando dos asteriscos **este texto está en negrita**.
Dos guiones bajos también funcionan.
Hagámoslo _cursiva ahora_.
Adivinaste, _un guión bajo también es suficiente_.
¿Podemos combinar ambos? Por supuesto.
¿Y si quiero tachar?

---

## Blockquote

¿Quieres resaltar la importancia del texto? No digas más.

```md
> Esto es un blockquote.
> ¿Quieres escribir en una nueva línea con espacio intermedio?
>
> > ¿Y anidado? No hay ningún problema.
> >
> > PS. puedes **estilizar** tu texto _como quieras_.
```

> Esto es un blockquote.
> ¿Quieres escribir en una nueva línea con espacio intermedio?
>
> > ¿Y anidado? No hay ningún problema.
> >
> > P.D. Puedes **estilizar** tu texto _como quieras_. :

---

## Imágenes

La mejor manera es simplemente arrastrar y soltar la imagen desde su ordenador directamente. También puede crear una referencia a la imagen y asignarla de esa manera.
Aquí está la sintaxis.

```md
![texto si la imagen no se carga](https://user-images.githubusercontent.com/46372998/212541682-9907aaea-5198-45a9-8961-2acc8a98a0db.png)

[logo]: https://user-images.githubusercontent.com/46372998/212541682-9907aaea-5198-45a9-8961-2acc8a98a0db.png

![texto de error][logo]
```

![texto si la imagen no se carga](https://user-images.githubusercontent.com/46372998/212541682-9907aaea-5198-45a9-8961-2acc8a98a0db.png)

[logo]: https://user-images.githubusercontent.com/46372998/212541682-9907aaea-5198-45a9-8961-2acc8a98a0db.png

![texto de error][logo]

---

## Enlaces

Al igual que las imágenes, los enlaces también pueden insertarse directamente o creando una referencia. Se pueden crear tanto enlaces en línea como en bloque.

```md
[Pagina de ejemplo]: https://example.com/
[docs]: https://github.com/adam-p/markdown-here

[Ir a la pagina ejemplo][Pagina de ejemplo]
Encuentra algunos grandes documentos [aquí][docs]
```

[Pagina de ejemplo]: https://example.com/
[docs]: https://github.com/adam-p/markdown-here

[Ir a la pagina ejemplo][Pagina de ejemplo]
Encuentra algunos grandes documentos [aquí][docs]

---

## Código

Puedes crear fragmentos de código tanto en línea como en bloque. También puede definir el lenguaje de programación que estaba utilizando en su fragmento. Todo ello mediante el uso de backticks.

````md
Para iniciar el la programacion `php` necesitas primero crear un archivo `index.php`

```php
$var = "Hello World";
echo $var;
```
````

Para iniciar el la programacion `php` necesitas primero crear un archivo `index.php`

```php
$var = "Hello World";
echo $var;
```

---

## Listas

Al igual que en HTML, Markdown permite crear listas ordenadas y desordenadas.

### Lista ordenada

```md
1. HTML
2. CSS
3. Javascript
4. React
5. Soy Frontend Dev ahora 👨🏼‍🎨
```

1. HTML
2. CSS
3. Javascript
4. React
5. Soy Frontend Dev ahora 👨🏼‍🎨

### Lista Desordenada

```md
-   Node.js

*   Express

## Nest.js

-   Aprendiendo Backend ⌛️
```

-   Node.js

-   Express

-   Nest.js

-   Learning Backend ⌛️

### Lista Mixta

También puedes mezclar ambas listas y crear sublistas.
**PS.** Intenta no crear listas de más de dos niveles. Es la mejor práctica.

```md
1. Aprender lo básico
    1. HTML
    2. CSS
    3. Javascript
2. Aprender un Framework
    - React
        - Router
        - Redux
    * Vue
    - Svelte
```

1. Aprende lo básico
    1. HTML
    2. CSS
    3. Javascript
2. Aprender un Framework
    - React
        - Router

-   Redux
    -   Vue
    *   Svelte

---

## Tabla

Gran manera de mostrar datos bien ordenados. Utilice el símbolo «|» para separar las columnas y el símbolo «:» para alinear el contenido de las filas.

```
| Alinear a la izquierda (por defecto) | Alinear al centro | Alinear a la derecha |
| :----------------------------------- | :---------------: | -------------------: |
| React.js                             |      Node.js      |                MySQL |
| Next.js                              |      Express      |              MongoDB |
| Vue.js                               |      Nest.js      |                Redis |
```

| Alinear a la izquierda (por defecto) | Alinear al centro | Alinear a la derecha |
| :----------------------------------- | :---------------: | -------------------: |
| React.js                             |      Node.js      |                MySQL |
| Next.js                              |      Express      |              MongoDB |
| Vue.js                               |      Nest.js      |                Redis |

---

## Lista de tareas

Llevar la cuenta de las tareas que están hechas, y las que faltan por hacer.

```md
-   [x] Aprender Markdown
-   [ ] Aprender Desarrollo Frontend
-   [ ] Aprender Desarrollo Full Stack
```

-   [x] Aprender Markdown
-   [ ] Aprender desarrollo frontend
-   [ ] Aprender Desarrollo Full Stack

---

## Línea horizontal

Puede utilizar asteriscos, guiones o subrayados (\*, -, \_) para crear una línea horizontal.
La única regla es que debe incluir al menos tres caracteres del símbolo.

```markdown
Primera línea horizontal

---

Segunda

---

Tercera

---
```

Primera línea horizontal

---

Segunda

---

Tercera

---

## Graficos simples

````md
```maremind
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

<div class="mermaid">
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;

</div>

---

## Nota al pie

¿Quieres describir algo al final del archivo? ¡Usa el pie de página!

```md
#### Estoy trabajando en un nuevo proyecto. [^1]

[^1]: Stack es: React, Typescript, Tailwind CSS

El proyecto es sobre música y películas.

##### Espero que te guste. [^ver]

[^ver]: Cargando... ⌛️
```

#### Estoy trabajando en un nuevo proyecto. [^1]

[^1]: Stack es: React, Typescript, Tailwind CSS

El proyecto es sobre música y películas.

##### Espero que te guste. [^ver]

[^ver]: Cargando... ⌛️
