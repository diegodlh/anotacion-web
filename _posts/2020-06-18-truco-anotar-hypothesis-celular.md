---
layout: post
title: "Un truco para anotar con Hypothesis en el celular"
author: Diego de la Hera
---

Hace unas semanas Chris Aldrich publicó en su [blog](https://boffosocko.com/2020/05/24/a-hack-for-using-hypothes-is-to-annotate-on-mobile/) una forma simple pero ingeniosa de anotar la web con [Hypothesis](https://web.hypothes.is/) desde un celular con Android (usuarios iOS, ver la sección [Notas finales](#notas-finales)).

En resumen, el método usa la app *URL Forwarder* para minimizar el número de pasos necesarios para obtener una versión anotable de una página web a través del [proxy Via](https://web.hypothes.is/help/what-is-the-via-proxy/) de Hypothesis.

## Instrucciones
Para configurarlo, primero tenemos que instalar la app [URL Forwarder](https://play.google.com/store/apps/details?id=net.daverix.urlforward) desde la Play Store en nuestro celular.

Luego abrimos la app y creamos un nuevo filtro con el botón con el signo '+' abajo a la derecha.

Ahora, configuramos el filtro:
1. En el campo "Filter url" escribimos `https://via.hypothes.is/@url`. Esto le dice al filtro que vuelva a abrir la página que queremos anotar con el proxy Via.
2. En el campo "Filter name" le damos un nombre al filtro, por ejemplo `Hypothesizar`.
3. Desactivamos la opción "Url Encode the forwarded url". Esto parecería ser necesario para URLs con acentos u otros caracteres especiales (por ejemplo, [https://es.wikipedia.org/wiki/Deforestación](https://es.wikipedia.org/wiki/Deforestación)).
3. Finalmente, apretamos la tilde arriba a la derecha para guardar el filtro.

![]({{ site.baseurl }}/images/url-forwarder.jpg)

¡Y listo! La próxima vez que encontremos una página que queramos anotar vamos a *Compartir*, elegimos *Url Forwarder*, seleccionamos nuestro filtro *Hypothesizar*, y la versión anotable de la página se va a abrir en nuestro navegador predeterminado.

## Notas finales
Si bien este método implica dos o tres pasos extra, en comparación con este otro que describo [acá](https://medium.com/@delahera/hypothesis-web-annotation-mobile-358db1f9ec46) (en inglés, pronto también en español), es mucho más sencillo de instalar.

Otra desventaja también es que nos obliga a recargar la página a través del proxy Via, lo cual a veces puede repercutir en el rendimiento, la apariencia e incluso la funcionalidad de la página que estamos anotando.

Por último, aparentemente *Url forwarder* no estaría disponible para iOS. En su artículo original, el autor comentó que la app *Shortcuts* podría servir de alternativa, aunque dice que es una herramienta demasiado sofisticada para el uso que le daríamos acá.