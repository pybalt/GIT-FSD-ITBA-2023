---
description: Con Visual Studio Code, vamos a comenzar el último tramo de esta actividad.
---

# ☺ Introduciendo cambios

Nos posicionamos en el archivo README.md

<figure><img src="../assets/image (26).png" alt=""><figcaption></figcaption></figure>

Como indica el archivo, dejamos nuestro nombre en una nueva línea.

A partir de acá, tenemos dós metodos para subir cambios. Les enseñaré ambos, y ustedes decidirán.

El que yo suelo usar, es el que viene integrado con el propio editor:

<figure><img src="../assets/image (27).png" alt=""><figcaption><p>En el apartado "Source control" en el simbolo del git tree, podemos ver los cambios que sufre cada archivo.</p></figcaption></figure>

Alternativamente, podemos utilizar el comando en la consola

```bash
git status
```

<figure><img src="../assets/image (28).png" alt=""><figcaption><p>El commando nos dirá cuáles archivos han sido modificados</p></figcaption></figure>

Luego, agregamos los archivos que tenemos intención de commitear.

<figure><img src="../assets/image (29).png" alt=""><figcaption></figcaption></figure>

En el símbolo `+` podemos agregar los cambios, a esto se le llama _staging._ El staging es guardar provisoriamente los archivos, preparándolos para hacer commit.

<figure><img src="../assets/image (30).png" alt=""><figcaption><p>Los cambios que estan en fase staged son los que van a ser introducidos en el commit</p></figcaption></figure>

Alternativamente, podemos hacer lo mismo por consola, a través del comando `git add`

```bash
git add nombre_del_archivo.extension
```

<figure><img src="../assets/image (32).png" alt=""><figcaption></figcaption></figure>

Podemos quitar este archivo de la fase de staging, a través del comando

```bash
git restore --staged nombre_del_archivo.extension
```

Mientras que, en el IDE Visual Studio Code, sería presionando el botón `-`

<figure><img src="../assets/image (33).png" alt=""><figcaption><p>El botón - cumple la misma función que lo detallado anteriormente</p></figcaption></figure>

Y ahora, vamos a hacer el commit.

<figure><img src="../assets/image (34).png" alt=""><figcaption><p>Es importante dejar un mensaje descriptivo en el commit, para después poder diferenciarlos entre sí.</p></figcaption></figure>

Al hacer commit, nos va a saltar lo siguiente

<figure><img src="../assets/image (35).png" alt=""><figcaption></figcaption></figure>

Nos fijamos en el historial del repositorio remoto, para comprobar que los cambios han sido introducidos:

<figure><img src="../assets/image (36).png" alt=""><figcaption><p>Ahi esta nuestro commit con su mensaje descriptivo</p></figcaption></figure>
