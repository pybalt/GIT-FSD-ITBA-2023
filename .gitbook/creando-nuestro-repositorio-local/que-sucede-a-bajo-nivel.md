---
description: ¿Qué sucede por detrás, cuando hacemos un commit y lo subimos al repositorio?
---

# 🔍 Qué sucede a bajo nivel

Cuando nosotros hacemos staging de un archivo, ya estamos guardando los cambios del archivo, aunque sin impactarlos definitivamente en el repositorio local.

Esto nos sirve porque quizas el entorno local no es seguro (quizas corremos scripts que borran archivos, por ejemplo),[^1] o queremos guardar los cambios y resguardarlos.

De modo que, al meter un archivo en la fase staging, estamos preparando los cambios que van a ser introducidos en el repositorio local.

Si hacemos mas cambios y los metemos al staging, entonces el archivo se sobreescribe con nuestra nueva version.

Cuando ya estamos seguros, metemos los cambios al repositorio local a traves del commit.

Cuando estemos seguros de que hayamos terminado una feature (alguna funcionalidad), podemos sincronizar los repositorios remotos y local, a traves del mecanismo push, que introduce los cambios desde el repositorio local, hacia el remoto. Es decir, desde nuestro entorno local, subimos los cambios a la nube.

<figure><img src="../assets/Untitled.png" alt=""><figcaption></figcaption></figure>

[^1]: 
