# Ejercicios - Tema 2: Ramas

A continuación, encontrarás 10 ejercicios prácticos sobre ramas en Git, fusión de ramas, resolución de conflictos y tipos de ramas. Intenta resolverlos antes de consultar la teoría.

---

## Ejercicio 1. Crear y listar ramas

Crea un repositorio nuevo llamado `tema2-ramas` y realiza un primer commit con un archivo `README.md`. Después, crea dos ramas nuevas llamadas `feature/header` y `feature/footer`. Por último, ejecuta el comando necesario para mostrar todas las ramas disponibles e indica cuál es la rama activa.
RESPUESTA:
con git branch se pueden ver las 3 ramas:
feature/footer
feature/header
main
main lleva un asterisco y el asterisco es una marca para indicar que es la rama activa, por lo tanto, main es la rama activa
---

## Ejercicio 2. Cambiar entre ramas

Sitúate en la rama `feature/header` y crea un archivo llamado `header.html` con una estructura básica. Haz un commit con un mensaje descriptivo. Después, cambia a la rama `feature/footer` y comprueba si el archivo `header.html` existe también en esa rama. Explica por qué ocurre ese comportamiento.
RESPUESTA:
se ha borrado el archivo header.html porque el GIT sólo guarda los cambios realizados en la rama
---

## Ejercicio 3. Fusión de una rama sin conflicto

En la rama `feature/footer`, crea un archivo llamado `footer.html` y guarda los cambios con un commit. Después, vuelve a la rama principal y fusiona `feature/footer`. Comprueba el historial de commits y explica qué ha ocurrido tras hacer el merge.
RESPUESTA:
Se ha incluido en la rama main el fichero de Ejercicios-2.md con mis respuestas y el fichero footer.html
---

## Ejercicio 4. Provocar un conflicto sencillo

Crea una rama nueva llamada `feature/title`. Modifica en esa rama una misma línea del archivo `README.md`, por ejemplo el título principal, y haz un commit. Después, vuelve a la rama principal, modifica exactamente esa misma línea con un contenido diferente y haz otro commit. Intenta fusionar `feature/title` en la rama principal y observa qué mensaje muestra Git.
RESPUESTA: dice que hay un conflicto en el AutoMerge de README.md
---

## Ejercicio 5. Identificar archivos en conflicto

Explica con tus palabras por qué se ha producido el conflicto.
RESPUESTA: El conflicto se ha producido porque se han intentado hacer modificaciones sobre el mismo fichero desde ramas diferentes
---

## Ejercicio 6. Resolver un conflicto manualmente

Abre el archivo en conflicto y localiza las marcas `<<<<<<<`, `=======` y `>>>>>>>`. Resuelve el conflicto manualmente dejando una única versión final coherente del contenido. Después, añade el archivo al área de preparación y completa el proceso de fusión con el commit correspondiente.
RESPUESTA: no me salian las marcas en su lugar lo he resulto con la interfaz de conflict de Visual Studio CODE
---

## Ejercicio 7. Conflicto con varias líneas

Crea una nueva rama llamada `feature/about` y añade una pequeña sección de presentación en un archivo `about.md`. Después, desde la rama principal, modifica también esa misma sección pero con un texto distinto. Intenta fusionar ambas ramas y resuelve el conflicto combinando parte del contenido de las dos versiones en lugar de quedarte solo con una.
RESPUESTA: hecho
---

## Ejercicio 8. Resolver un conflicto en VSCode o en GitHub

Provoca de nuevo un conflicto entre dos ramas modificando la misma línea de un archivo. Si antes resolviste los conflictos usando VSCode trata de resolverlo diréctamente en GitHub o viceversa.

---

## Ejercicio 9. Tipos de ramas

Investiga brevemente para qué se suelen utilizar ramas de tipo `feature`, `bugfix`, `hotfix` y `release`. Después, propón un ejemplo de nombre válido para cada una dentro de un proyecto web.

---

## Ejercicio 10. Caso práctico completo

Imagina que estás trabajando en equipo y dos personas han editado la misma parte del archivo `index.html`: una ha cambiado el texto del encabezado y otra ha cambiado ese mismo texto en otra rama distinta. Describe paso a paso cómo resolverías el conflicto, indicando qué comandos usarías desde el momento en que Git detecta el conflicto hasta que la fusión queda completada.

---

## Reto final opcional

Crea un pequeño proyecto con una rama principal y al menos dos ramas secundarias. Haz cambios distintos en varios archivos, provoca al menos un conflicto real al fusionarlas y resuélvelo manualmente. Después, revisa el historial de commits y explica qué estrategia has seguido para dejar una versión final correcta del proyecto.
