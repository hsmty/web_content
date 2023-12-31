---
layout: post
title: "Layer Shortcuts - Eagle"
author: Edén Candelas
draft: True
---

![img1][all]

EAGLE TIPS  Atajos de teclado.

Cuando se empieza a utilizar eagle de forma continua nos vemos en la necesidad de automatizar ciertos procesos repetitivos para aumentar la velocidad con la que trabajamos, esto lo logramos mediante atajos de teclado (keyboard shortcuts).


Estas automatizaciones se llevan a cabo asignando secuencias de comandos a combinaciones de teclas. La forma de accesar a ello es mediante la opcion Assign en el menu Options.

![img2][menuPath]

Esto nos muestra el panel de shortcuts, donde aparecen los shorcuts que actualmente estan asignados en entorno. 

![img2][assignEnv]

En la parte inferior podemos ver las opciones que tenemos. Por ahora utilizaremos New.
Al acceder vemos que nos muestra tres secciones, una donde seleccionamos la tecla principal, otra donde seleccionamos los modificadores y una tercer area para los comandos.

![img2][assignNew]

En el area de los comandos se nos es permitido concatenar comandos y sus opciones, los comandos son separados por ";", las opciones de los mismos por " " (espacios).

En este caso para lo que se visualiza en el editor de layouts se utiliza el comando "display". Diplay permite activar layers si estos se añaden como opcion. De esta forma '''display 1 17 18 20" nos mostrara el layer 1 (top), 17 (pads), 18 (vias) y 20 (dimension)'''.
El comando por si solo añadira esos layers en el area de visualizacion. Si queremos remover ciertos layer anteponemos "-" al numero del layer. Asi ''' display -16 -22 -24''' remueve del area de visualizacion los layers 16 (bottom), 22 (bPlace) y 24 (bOrigins).
Otra opcion de remover los layers que no necesitamos es mediante la opcion "none", asi '''display none''' quitara el contenido de todos los layers.
Por ultimo '''display all''' mostrara todo el contenido de todos los layers. (poco recomendable).

En este caso asigno a la secuencia Ctrl-1 (^1) los comandos '''display none; display 1 17 18 20 21 23 25 51 ''' para mostrar en pantalla el layer superior.

![img2][topCmd]

Para visualizar el layer inferior utilizo Ctrl-4(^4) con los comandos ''' display none; display 16 17 18 20 22 24 26 52'''

![img2][bottomCmd]

Hay una razon por la que salte del 1 al 4, los diseños que estoy realizando actualmente requieren 4 layers, asi asigno las teclas 2 y 3 a la visualizacion de los layers intermedios.

Tambien cabe destacar que los comandos se pueden teclear directamente en la barra de comandos y obtener el mismo resultado.


[all]: /assets/post_img/eagle/all.png  "all"
[menuPath]: /assets/post_img/eagle/  "menuPath" 
[assignEnv]: /assets/post_img/eagle/assignEnv.png  "assignEnv"
[assignNew]: /assets/post_img/eagle/assignNew.png  "assignNew"
[topCmd]: /assets/post_img/eagle/topCmd.png  "topCmd"
[bottomCmd]: /assets/post_img/eagle/bottomCmd.png  "bottomCmd"






















