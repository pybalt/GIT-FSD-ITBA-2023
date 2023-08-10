---
description: En esta sección vamos a explicar más a detalle qué es el merge
---

# 🧠 El merging

El merge es básicamente colapsar todos los commits de la nueva rama, dentro de un commit en la rama main.

<figure><img src="../assets/image (46).png" alt=""><figcaption></figcaption></figure>

Les va a suceder que tengan el mismo archivo, con las mismas lineas siendo ocupadas, y tendrán que tomar una decisión sobre qué línea quedarse, o al resolver el merge, tendrán que modificar el archivo resultante.

Cuando eso suceda, el merge no estará disponible.

<figure><img src="../assets/image.png" alt=""><figcaption><p>Un ejemplo de un conflicto a resolver para fusionar ramas</p></figcaption></figure>

Cuando le damos a resolver conflicto, tendremos esta situacion

<figure><img src="../assets/image (1).png" alt=""><figcaption></figcaption></figure>

Acá, lo que esto significa, es que estas líneas estan ocupando la misma porción de código, y hay que decidir qué versión quedarnos, si main-1 o main.\
Lo más fácil suele ser borrar todo y reescribir la versión que va a ir publicada. Dado que estamos en una situación complicada, es importante prestar atención.

<figure><img src="../assets/image (2).png" alt=""><figcaption></figcaption></figure>
