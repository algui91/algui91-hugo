---
author: alex
categories:
- dev
mainclass: dev
date: '2016-01-01'
lastmod: 2017-10-08T19:00:53+01:00
url: /pylabra-aplicacion-para-almacenar/
title: "Pylabra. Aplicación para almacenar vocabulario"
tags:
- python
---

Hace bastante tiempo que Haitike y yo dejamos de desarrollar [Pylabra][1], y nunca creé una entrada hablando de la aplicación en sí, asi que me he decidido a escribirla.

Antes de nada, el programa necesita instalar algunas dependencias, entre ellas la libreria sqllite y las librerias de wxWidgets (python-wxgtk2.8), que podemos instalar de la siguiente manera:

```bash
sudo aptitude install libsqlite python-wxgtk2.8
```

<!--more--><!--ad-->

Una vez instaladas podemos ejecutar el programa haciendo clic en el archivo llamado main.py, o bien desde consola con:

```bash
./main.py
```

Podéis descargar Pylabra desde <a target="_blank" href="https://github.com/elbaulp/PyLabra">Github</a>

Una vez lo ejecutéis, vereis la pantalla principal:

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://3.bp.blogspot.com/_IlK2pNFFgGM/TUB3RT8nvII/AAAAAAAAASY/EoeMulJUyJU/s800/principal.png" width="800"></img>
</figure>

La interfaz es muy simple con 5 botones arriba (En esta imagen falta uno, el botón &#8220;Acerca de&#8221;), pero en las siguientes imágenes aparecerá.

Bien, lo primero que vamos a probar es a añadir una palabra, para ello hacemos clic en el primer botón de la parte superior izquierda, lo que nos abrirá esta ventana:

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://1.bp.blogspot.com/_IlK2pNFFgGM/TUB3APm2yfI/AAAAAAAAAR4/b-EUFZtkKJY/s800/AddPalabra.png" width="800"></img>
</figure>

En un principio esta aplicación estaba pensada para almacenar palabras en Alemán, por eso aparecen unos RadioButton con los distintos géneros en Alemán, podeis ignorar esa parte y almacenar palabras del idioma que queráis. Si no os gusta que aparezca, decidmelo y os digo la parte de código que tenéis que eliminar.

En esta pantalla simplemente rellenamos los campos que queramos y le damos a &#8220;Guardar y salir&#8221;

Ahora vemos que se ha generado una fila en la pantalla principal con la palabra que avabamos de crear:

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://2.bp.blogspot.com/_IlK2pNFFgGM/TUB3Al5R7dI/AAAAAAAAASA/W1nLDdgvH6A/s800/condatos.png" width="800"></img>
</figure>

Si hacemos clic con el botón derecho sobre una fila, podemos editar la palabra o borrarla, si le damos a editar nos sadrá la siguiente pantalla:

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://4.bp.blogspot.com/_IlK2pNFFgGM/TUB3BJpBsVI/AAAAAAAAASQ/_yeeBiG9AcM/s800/EditarPalabra.png" width="800"></img>
</figure>

También podemos ordenar las palabras por los distintos campos (No, palabra, genero etc), solo tenemos que hacer clic en el nombre del campo, así como también podemos buscar palabras con la caja de texto que hay en la parte superior.

En la parte derecha tenemos un buscador de wordreference para buscar palabras Inglés-Español que podemos ocultar con su botón correspondiente de la parte superior.

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://4.bp.blogspot.com/_IlK2pNFFgGM/TUB3A77mKsI/AAAAAAAAASI/jDL9aDs2bss/s800/diccionario.png" width="800"></img>
</figure>

Si ocultamos el navegador la pantalla principal queda de la siguiente manera:

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://2.bp.blogspot.com/_IlK2pNFFgGM/TUB3RgQpV7I/AAAAAAAAASg/86OmTn34j3s/s800/QuitarNavegador.png" width="800"></img>
</figure>

Si haceis clic en el botón con forma de estrella, se abrirá una ventana con información del programa y de los desarrolladores:

<figure>
    <img sizes="(min-width: 800px) 800px, 100vw" on="tap:lightbox1" role="button" tabindex="0" layout="responsive"  height="640" src="https://3.bp.blogspot.com/_IlK2pNFFgGM/TUB3AAFAq5I/AAAAAAAAARw/hPadST7-nyc/s800/AcercaDe.png" width="800"></img>
</figure>

Para terminar la entrada quiero decir que es un programa bastante simple, pero nos sirvió para aprender algo más de python y sobre todo para aprender a trabajar en equipo.

Os lo dejo a vuestra disposición y ojalá que os sea útil.


 [1]: https://elbauldelprogramador.com/pylabra-aplicacion-para-almacenar/
