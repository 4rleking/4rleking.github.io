---
layout: single
title: Protección y Seguridad en Internet
excerpt: "Todos estamos vulnerables a acoger un malware en nuestros dispositivos, desde seleccionar un link, descargar un archivo PDF, recibir y abrir un email, descargar un juego o software crackeado, pero entre mejor estemos informados, menos serán las posibilidades de regalar nuestra información personal, aquí se muestran algunas de las herramientas o técnicas para poder saber si hay algo más atrás de la descarga o archivo."
date: 2023-09-28
classes: wide
header:
  teaser: /assets/images/Proteccion/Intro.jpg
  teaser_home_page: true
categories:
  - Hacking
tags:
  - VirusTotal
  - bitly
  - ExpandURL
---

![](/assets/images/Proteccion/Intro.jpg)

## Análisis de archivos y URL

<center>
    <img src='./../assets/images/Proteccion/Virustotal.jpeg' alt="" width="70%" height="70%" />
</center>

Cuando descargamos algún archivo desde internet nuestra mejor herramienta para verificar que esté libre de malware es [Virustotal](https://www.virustotal.com/gui/home/upload); en esta página puedes cargar el archivo y lo analizará en cuestión de minutos o segundos, esta página cuenta con motores de búsqueda de malware de diferentes proveedores de antivirus.

Además de analizar archivos, también puede analizar URL, es decir si creemos que la página no es segura, solo necesitamos copiar el link de la página que vamos a ingresar y la pegamos en este portal, automáticamente la analizará y nos dirá si esconde algo.

### Cómo usarlo

Si desea verificar un archivo, debe subirlo al servicio presionando el botón "Elegir archivo" y localizándolo. Recuerde que el tamaño máximo de carga es de 650 MB, y el tiempo de carga depende en gran medida de su conexión a Internet. Es posible que deba ser un poco paciente de vez en cuando.

VirusTotal puede ser un servicio útil, pero no es un reemplazo antimalware. No puede protegerlo de la manera en que lo haría su solución antimalware tradicional. En cambio, es una solución de asistente o segunda opinión que cualquier otra cosa. Puede usarlo para verificar un archivo / URL con más motores antimalware que el que usa. Debe saber que los motores de los proveedores pueden estar optimizados para el análisis para obtener resultados más rápidos. Eso significa que podrían no ser tan exhaustivos como una solución completa para menos recursos y optimización del tráfico. Por lo general, son más que suficientes, pero debes tenerlo en cuenta. Los falsos positivos también son un hecho. Además, la privacidad es algo que debe considerar.

Es mejor evitar analizar archivos de información personales o confidenciales. Como VirusTotal establece claramente en su acuerdo, no deberías hacerlo. La razón principal es que su archivo se procesa y se comparte con su comunidad. Para ayudar más a la comunidad, usar menos recursos es algo necesario, pero aún así, la privacidad puede ser un problema. Tenga mucho cuidado con lo que puede elegir cargar. Con un gran poder también viene una gran responsabilidad.

<img src='./../assets/images/Proteccion/urlvoid.webp' alt="" width="50%" height="50%" />

Aparte de VirusTotal, también tenemos otras opciones, por ejemplo [urlvoid](https://www.urlvoid.com/), en este sitio podemos analizar las direcciones URL que necesitemos, además nos brindan una serie de herramientas el cual podemos utilizar para "escanear" de cierta manera un dominio:

* WHOIS
* DNS
* PING
* SCREENSHOT
* PASSWORD (Genera una contraseña robusta)
* SORT
* DNSSEC
* BASE64

Entre muchas más ...

## URL acortadas

<center>
    <img src='./../assets/images/Proteccion/bitly.png'>
</center>

Existen varios proveedores de servicios en internet que lo que hacen es acortar una URL extensa [bitly](https://bitly.com/), por ejemplo, para evitar escribir *"https://4rleking.github.io/"* lo acortan haciendo *"https://bit.ly/45u7dxs"* que es mucho más fácil de escribir o de "pasar desapercibido", para hacerlo un poco más amigable pueden crear un código QR.

<center>
    <img src='./../assets/images/Proteccion/QR.png' height="200px" width="200px">
</center>

Muchas de las empresas de marketing, y no solo de este ramo utilizan este tipo de servicios de acortadores de URL, por lo regular lo utilizan para detectar de donde tienen más visitantes, ya que estos servicios de acortadores al registrar un nuevo link, automáticamente le designan un contador de "visitas" a ese link.

Así como puede ser beneficioso para unas cosas, puede ser utilizado para robarte información o en su defecto infectarte con malware, por ejemplo, un sitio "clon" (phishing) de algún banco, tienda departamental, tienda online, el típico "te ganaste un IPhone" si llenas el siguiente formulario y lo compartes con tus amigos; muchas de las veces son sitios como "https:/promociones5000.com" y con este dominio nadie o muy poca gente caería en sus estafas, es por esto que utilizan el acortador, para disfrazar la URL y así garantizar o tratar de garantizar que más personas caigan en sus estafas.

Para evitar esto, existe un servicio online gratuito [ExpandURL](https://www.expandurl.net/), el cual copias la URL acortada y la pegas en este sitio, automáticamente seguirá la ruta de esta URL acortada (sin entrar a ese sitio) y te dirá cuál es el sitio final; y ahora sí ya depende del usuario final si entra o no al sitio.

## Comprobar la seguridad de una contraseña

