---
cover: >-
  https://images.unsplash.com/photo-1556075798-4825dfaaf498?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHxnaXR8ZW58MHx8fHwxNjkxMzUzNzczfDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🤓 Los sistemas de control de versiones

Ahora pasemos de este grupo numeroso a un grupo reducido, somos cinco amigos tratando de escribir en la misma hoja. ¿Deberíamos intentar escribir todos al mismo tiempo? ¿Qué sucedería si intentásemos hacerlo?

Tal como podrás imaginar, el trabajo simultáneo de diferentes personas, puede llevarnos a la situación en la que uno escribe por encima del otro.

Un sistema de control de versiones, permite que los desarrolladores aúnen esfuerzos en una dirección, en la que minimicemos la posibilidad de reescribir el trabajo de otros.

Ahora bien, este modelo de trabajo, el sincrónico, es una perfecta explicación de los modelos más antiguos de este software de trabajo, los sistemas de control de versiones **centralizados**.

Los sistemas de control de versiones centralizados, consistían en una conexión constante a un servidor que contenía el código fuente de la aplicación, forzando al desarrollador a estar continuamente sincronizado con el servidor.\
Este modelo, aparte de la conexión constante, dada su naturaleza, no era muy eficiente para manejar las _**fusiones**_ y _**conflictos**_ entre las _**ramas**_.

¿Ramas? ¿Fusiones? ¿Conflictos? ¿De qué estamos hablando?

<figure><img src="https://res.cloudinary.com/practicaldev/image/fetch/s--SuAdPSjR--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/2aridnng7k6bly55lic9.jpeg#gh-light-mode-only" alt=""><figcaption><p>Esto es lo que se llama un git tree</p></figcaption></figure>



Antes de empezar con el concepto de ramas, fusiones y conflictos, terminemos de definir qué es **GIT**.

#### La descentralización en el mundo de la programación

GIT es un sistema de control de versiones **descentralizado.** El que sea descentralizado trae ventajas e inconvenientes, como todo. Pero en general, consideramos que es un paso hacia adelante.

| Ventajas                                                                                        | Desventajas                                      |
| ----------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| No requiere una conexión permanente con un servidor.                                            | Requiere un nivel técnico mucho más alto.        |
| Es más rápido y ligero, ya que las operaciones se realizan localmente, es decir, en la máquina. | Tiene comandos más tediosos.                     |
| GIT facilita la creación y el manejo de ramas.                                                  | Su interfaz y su accessibilidad son deficientes. |
| GIT es ahora mismo el estándar de control de versiones, además de ser open source.              | Consume muchos recursos.                         |

