---
description: >-
  Un concepto clave a la hora de trabajar en GIT, es del de las ramas. En este
  capítulo hablaremos de las ramas remotas y locales, lo que nos servirá para
  hablar de las operaciones más cotidianas.
cover: >-
  https://images.unsplash.com/photo-1607799279861-4dd421887fb3?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwzfHxwcm9ncmFtbWluZyUyMGdpdCUyMGJyYW5jaHN8ZW58MHx8fHwxNjkxMzU0NDM5fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🤓 Ramas | branchs

El paradigma de control de versiones, se basa en, lo que podríamos describir gráficamente, como un árbol el cual crece con cada _**commit**_ que añadimos al código fuente.&#x20;

El código fuente no es más que la suma de los archivos que componen a nuestro proyecto, y contiene la lógica de nuestra aplicación.&#x20;

Un commit, es una actualización del código que queda guardada en la historia del código.

Cuando usamos un sistema de versionado, podemos recorrer la historia del código commit a commit, de modo que podríamos viajar al pasado 😎.

<figure><img src="../assets/image.png" alt=""><figcaption><p>Esto es una representación de un arbol git, donde cada círculo es un commit.</p></figcaption></figure>

¿Algúna vez viste Flash? ¿Quizás te guste Marvel?

Cuando estamos desarrollando por ramas, estamos creando un multiverso de versiones de la misma aplicación, hasta que decidimos que cada multiverso colapse en la versión principal, que va a ser la que el usuario final va a recibir.

Se considera buena práctica un desarrollo por ramas, puesto que se mantiene un orden y se vuelve menos caótico.
