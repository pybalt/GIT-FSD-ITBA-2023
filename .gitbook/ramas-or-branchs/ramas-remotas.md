---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Ramas remotas

Las ramas remotas, son las ramas que ya están guardadas en la nube.

Una vez los desarrolladores se sientan conformes con su desarrollo en su entorno local, se preparan para subir sus modificaciones a la rama remota.

Es importante tener en cuenta que existen múltiples ramas, tantas como queramos, pero sólo existe una rama principal, que bien puede llamarse master o main.

Sobre la master, o la main, se suelen subir las versiones oficiales.

Suele haber una rama de desarrollo, que es la versión más nueva de la aplicación, generalmente más inestable puesto que aún se siguen descubriendo bugs. Un ejemplo de esta rama podría ser Windows Insiders, que es un programa de Windows que te permite acceder a las más nuevas actualizaciones de Windows, a cambio de que permitas que ellos obtengan métricas del funcionamiento del sistema.

Y, sobre la rama de desarrollo, se suelen crear nuevas ramas, que son ramas atómicas (muy pequeñas) que consisten en implementar nuevas funcionalidades. Apenas esas funcionalidades estén finalizadas, se **fusionan** con la rama de desarrollo.

<figure><img src="../assets/image (1).png" alt=""><figcaption><p>En celeste, la rama main, en violeta, la rama de desarrollo, y en verde, las nuevas funcionalidades.</p></figcaption></figure>
