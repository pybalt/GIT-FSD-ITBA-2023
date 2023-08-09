---
description: >-
  En esta seccion vamos a hablar de los metodos de autenticacion y como
  autenticarte a GitHub a traves del SSH
---

# 🔧 Configurando GIT







Dado que la finalidad de este gitbook es explicar conceptos complicados, por y para alumnos, encuentro que es más explicativo dejarles un vídeo mientras les dejo algunos comentarios.

{% embed url="https://www.youtube.com/watch?v=kYd5T6FTvUA" %}

Hace un año solíamos utilizar el método HTTP, el cual está deprecado (ya no se usa más) por razones de seguridad. De manera que una gran barrera de entrada es comenzar a utilizar la consola para poder configurar nuestra fingerprint (una clave alfanumérica irrepetible que permite identificar nuestra máquina) para realizar la conexión SSH.

Una vez agreguen GIT a su entorno local, y configuren sus credenciales de autenticación, no necesitarán hacerlo nuevamente, salvo que formateen la pc, o en su defecto, cambien de computadora.

Nuevamente, en caso de que tengas algo más de experiencia, te dejo el link de la [documentación de GitHub](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent).

Lo que debemos de hacer es, después de instalar GIT, es configurar nuestro avatar personal.

```bash
git config --global user.name "Tu nombre"
```

Luego de setear nuestro nombre, introducimos el email que usamos en GitHub.

```bash
git config --global user.email "tu_email@ejemplo.com"
```

Luego de setear nuestro avatar, vamos a asociar el fingerprint de nuestro ordenador con la cuenta de GitHub.

Vamos a introducir este comando en la consola:

```bash
ssh-keygen -t ed25519 -C "tu_email@ejemplo.com"
```

Debemos reemplazar la parte "tu\_email@ejemplo.com" con el email que usamos para la cuenta de GitHub, la misma que ademas usamos en nuestro GIT local.

<figure><img src="assets/image (18).png" alt=""><figcaption><p>Es mejor dejar por default la ubicacion del fingerprint, para evitar perderla.</p></figcaption></figure>

Luego de esto, se nos pedira una frase que nos servirá de contraseña

<figure><img src="assets/image (19).png" alt=""><figcaption><p>Se nos pedirá la frase de contraseña</p></figcaption></figure>

Luego, activamos el gestor ssh.

```bash
eval "$(ssh-agent -s)"
```

Después de esto, debemos de introducir la nueva fingerprint dentro del gestor ssh.

```shell
ssh-add ~/.ssh/id_ed25519
```

Para poder acceder a la key, introducimos este comando.

```bash
ssh-agent sh -c 'ssh-add; ssh-add -L'
```

Copiamos el resultado, que comienza con `ssh-ed`

Vamos a la pagina donde están listadas [nuestras llaves](https://github.com/settings/keys). Creamos una nueva llave, y luego de copiar el contenido del comando listado más arriba, debería de verse algo similar a lo siguiente:

<figure><img src="assets/image (20).png" alt=""><figcaption></figcaption></figure>

Luego de esto, estamos listos para establecer una comunicación entre los repositorios remotos y nuestro entorno local.
