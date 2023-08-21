---
layout: single
title: Protección y Seguridad en Internet
excerpt: "Todos estamos vulnerables a acoger un malware en nuestros dispositivos, desde seleccionar un link, descargar un archivo PDF, recibir y abrir un email, descargar un juego o software crackeado, pero entre mejor estemos informados, menos serán las posibilidades de regalar nuestra información personal, aquí se muestran algunas de las herramientas o técnicas para poder saber si hay algo más atrás de la descarga o archivo."
date: 2023-07-22
classes: wide
header:
  teaser: /assets/images/20230722/Intro.jpg
  teaser_home_page: true
categories:
  - Hacking
tags:
  - VirusTotal
  - bitly
  - ExpandURL
---

![](/assets/images/20230722/Intro.jpg)

## Análisis de archivos y URL

Cuando descargamos algún archivo desde internet nuestra mejor herramienta para verificar que esté libre de malware es [Virustotal](https://www.virustotal.com/gui/home/upload); en esta página puedes cargar el archivo y lo analizará en cuestión de minutos o segundos, esta página cuenta con motores de búsqueda de malware de diferentes proveedores de antivirus.

Además de analizar archivos, también puede analizar URL, es decir si creemos que la página no es segura, solo necesitamos copiar el link de la página que vamos a ingresar y la pegamos en este portal, automáticamente la analizará y nos dirá si esconde algo.

## URL acortadas

Existen varios proveedores de servicios en internet que lo que hacen es acortar una URL extensa [bitly](https://bitly.com/), por ejemplo, para evitar escribir *"https://4rleking.github.io/"* lo acortan haciendo *"https://bit.ly/45u7dxs"* que es mucho más fácil de escribir o de "pasar desapercibido", para hacerlo un poco más amigable pueden crear un código QR.

<center>
    <img src='./../assets/images/20230722/QR.png' height="200px" width="200px">
</center>

Muchas de las empresas de marketing, y no solo de este ramo utilizan este tipo de servicios de acortadores de URL, por lo regular lo utilizan para detectar de donde tienen más visitantes, ya que estos servicios de acortadores al registrar un nuevo link, automáticamente le designan un contador de "visitas" a ese link.

Así como puede ser beneficioso para unas cosas, puede ser utilizado para robarte información o en su defecto infectarte con malware, por ejemplo, un sitio "clon" (phishing) de algún banco, tienda departamental, tienda online, el típico "te ganaste un IPhone" si llenas el siguiente formulario y lo compartes con tus amigos; muchas de las veces son sitios como "https:/promociones5000.com" y con este dominio nadie o muy poca gente caería en sus estafas, es por esto que utilizan el acortador, para disfrazar la URL y así garantizar o tratar de garantizar que más personas caigan en sus estafas.

Para evitar esto, existe un servicio online gratuito [ExpandURL](https://www.expandurl.net/), el cual copias la URL acortada y la pegas en este sitio, automáticamente seguirá la ruta de esta URL acortada (sin entrar a ese sitio) y te dirá cuál es el sitio final; y ahora sí ya depende del usuario final si entra o no al sitio.

## Comprobar la seguridad de una contraseña