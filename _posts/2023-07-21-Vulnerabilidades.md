---
layout: single
title: Tipos de Vulnerabilidades
excerpt: "Ningún sistema es 100% seguro, al momento de crearse tiene fallas, errores, durante su ciclo de vida sigue teniendo fallas y errores, es por ello que aquí se explican que son este tipo de fallas y que tan grave puede afectar en los sistemas."
date: 2023-07-21
classes: wide
header:
  teaser: /assets/images/20230721/Intro.jpg
  teaser_home_page: true
categories:
  - Vulnerabilidades
  - Hacking
tags:
  - Fundamentos
---

![](/assets/images/20230721/Intro.jpg)

Una vulnerabilidad no es más que un fallo, un fallo de seguridad, un defecto en la seguridad, un punto débil en algún activo, ya sea físico o lógico, que pueda poner en riesgo la confidencialidad, integridad y disponibilidad de la información.

Cuando hablamos de este tipo de fallos de seguridad tenemos que tener en cuenta los siguientes conceptos:

- Exploit
- Payload
- 0-day

## Exploit

Continuamente se habla en el contexto de un ciberataque del uso de exploits que aprovechan una vulnerabilidad, pero, ¿qué es realmente un exploit y cómo funciona?

Las definiciones habituales hablan de un programa o código que se aprovecha de una vulnerabilidad o fallo de seguridad en una aplicación o sistema, de forma que un atacante podría aprovechar ese fallo en su beneficio.

Trasladado a la vida real, sería como si un modelo de cerradura (sistema o aplicación) tuviera un fallo de diseño que permite a un tercero crear llaves que abran esa cerradura (exploit). Con esta llave o exploit un actor malintencionado podría acceder a un sitio o entorno vulnerable y realizar actos delictivos. Por ejemplo, ejecutar malware.

Existe confusión entre los usuarios y cierto mito de que un exploit puede considerarse malware. La realidad es que, tal y como hemos visto en el ejemplo, no es un código malicioso en sí mismo, sino que es la llave para que estos accedan a nuestro sistema y luego realicen otras acciones maliciosas.

Por lo tanto, un exploit puede darle a un atacante los permisos necesarios para poder ejecutarse en un sistema e infectarlo.

### Tipos de exploit

Ahora que sabemos qué es un exploit podemos distinguir entre dos tipos: los conocidos o desconocidos (zero-day).

Los exploits conocidos son aquellos que fueron desarrollados para aprovechar vulnerabilidades conocidas y que fueron corregidas mediante actualizaciones. Algunos son utilizados a lo largo de los años ya que muchos equipos no son actualizados. Lo bueno es que podemos tomar medidas para evitar ver nuestros sistemas afectados con solo instalar las actualizaciones. Suelen ser los que aparecen en la mayoría de noticias de seguridad y aparecen varios cada día, de la misma forma que van apareciendo las vulnerabilidades que tratan de aprovechar.

En el caso de los exploits desconocidos, son aquellos que se desarrollan para aprovechar vulnerabilidades zero-day; es decir, fallos de seguridad que no han salido a la luz y para los cuales no existe un parche que permita evitar su explotación o abuso. Las zero-day son particularmente peligrosas cuando se utilizan en ataques dirigidos a empresas o gobiernos. Es importante comprender que cuando un atacante utiliza un exploit para una vulnerabilidad zero-day no suele haber medidas que puedan bloquear el malware que intenta aprovechar el fallo, por lo tanto estos ataques son muy difíciles de detectar. Es por eso que son muy cotizados entre los delincuentes que compran y venden estos exploits en foros de la dark web, ya que les permiten lanzar ataques para robar información importante de una empresa o gobierno o, en casos extremos, atacar cierto tipo de infraestructuras críticas.

Una vulnerabilidad remota se extiende a través de una red y explota las brechas de seguridad sin necesidad de ningún acceso previo al sistema que ataca.

Por el contrario, una vulnerabilidad local sí requiere que se haya accedido antes al sistema vulnerable, normalmente con la intención de aumentar los privilegios para la persona que, posteriormente, va a ejecutar el exploit.

También existen exploits específicos contra aplicaciones de cliente (aquellas que requieren contacto con un servidor) que normalmente se originan en la modificación de los servidores para que estos envíen entonces el exploit al equipo. Las vulnerabilidades contra las aplicaciones cliente también puede requerir cierta interacción con el usuario, por lo que en ocasiones se utilizan en combinación con métodos de ingeniería social para manipular a las víctimas.

## Payload

Son las instrucciones de un fragmento de código, una vez que la vulnerabilidad se explotó con éxito, este pequeño fragmento de código (Payload) son todas aquellas instrucciones que se le dará al activo ya comprometido.

## 0-day

Las vulnerabilidades de Día Cero (también conocidas como 0-day exploits) son las brechas de seguridad en el software desconocidas hasta el momento del ataque. Desde ese punto hasta que la vulnerabilidad es suprimida se entra en el momento en el que los hackers pueden explotarla para lograr el máximo impacto en programas, datos, ordenadores adicionales o en toda una red.

Así, los exploits dirigidos contra ese tipo de vulnerabilidades se denominan zero-day exploits, o ataques zero-day. Cuanto más masivo sea el ataque y menos días hayan transcurrido desde ese Día Cero, mayor será la probabilidad de que no se haya desarrollado ninguna solución o mitigación y los daños pueden ser más extensos.

E incluso después de haber desarrollado la corrección, esos primeros días no todos los usuarios de software habrán podido aplicarla. El caso de WannaCry fue paradigmático en este sentido: el malware se aprovechaba de un exploit de Windows desarrollado por la Agencia de Seguridad de Estados Unidos y revelado en las semanas previas por Wikileaks.

En los primeros días el problema fue corregido por Microsoft mediante una actualización, pero todos los equipos que no hubieran realizado la puesta al día los días posteriores seguían siendo vulnerables. La activación el lunes de estos equipos que no habían sido utilizados durante el fin de semana inició una segunda oleada de propagación.

**Amenaza oculta**

Cuando se hace público un exploit los autores del software afectado toman medidas: la vulnerabilidad se arregla -a menudo a través de un parche- y el exploit se vuelve inutilizable. Por esa razón algunos black hat hackers, así como los hackers de agencias militares o servicios de inteligencia, no publican esas incursiones sino que las mantienen en privado para continuar explotándolas.

Muchos exploits están diseñados para proporcionar acceso a como administrador o superusuario de un sistema. Sin embargo, también es posible que los hackers utilicen varios exploits diferentes para este mismo fin: primero para obtener acceso de bajo nivel, luego para escalar privilegios repetidamente hasta llegar al nivel administrativo más alto (también menudo llamado root).

# Vulnerabilidades

## Naturales

Son aquellas que van en consecuencia con las condiciones ambientales, condiciones que puedan poner en riesgo la información.

## Físicas

Son debilidades que hay en lugares donde la información se almacena o se trata de forma física (mala gestión a la hora de almacenar la información).

## En Software

Son fallos de seguridad y/o malas configuraciones en aplicaciones, sistemas operativos o servicios instalados que pueden poner en riesgo la información.

## En Hardware

Son defectos que pueden tener los componentes de hardware de un equipo, defectos de fábrica, configuración o deterioro que puedan poner en riesgo la información.

## En Conexión

Son debilidades que puedan comprometer la información que viaja a través de distintos medios de comunicación (cables, inalámbricos).

## Humanas

Son debilidades en la parte humana muy difíciles de corregir que pueden ser aprovechados por un atacante para poder obtener información confidencial.

# Recomendaciones

* Mantener todas nuestras aplicaciones y sistemas actualizados: sabiendo que los exploits se aprovechan fallos de seguridad, resulta vital corregirlos cuanto antes. Por eso es necesario mantener una política de actualizaciones eficaz para evitar dejar una ventana de tiempo que pueda ser aprovechada por los atacantes

* Contar con una solución de seguridad avanzada como algún antivirus de una firma reconocida, capaz de detectar y bloquear exploits pensados para aprovechar vulnerabilidades en navegadores web y lectores PDF, entre otros.

* Realice una copia de seguridad de sus archivos. Si bien el software actualizado le protegerá de los ataques de exploit conocidos, no hay mucho que hacer cuando un hacker descubre una vulnerabilidad de día cero. Pero con una copia de seguridad actualizada de todos los archivos más importantes, estará cubierto en caso de que un ciberdelincuente use un exploit para instalar en su ordenador ransomware u otro tipo de malware que dañe los archivos. Cuando realice la copia de seguridad en una unidad externa, desconecte la unidad cuando no la esté usando y almacénela por separado del ordenador. Esto evitará que el malware afecte al contenido de la unidad.

* Utilice software de proveedores de confianza. Este consejo se aplica a aplicaciones independientes, así como a extensiones y conectores de navegador. Los desarrolladores de software confiables garantizan que sus productos cuentan con la máxima resistencia posible frente a los exploits. Y, si se produce un exploit de día cero, responderán en seguida con un parche de seguridad.

# Siguiente Nivel

* [Vulnerabilidades a Detalle](https://vulnerabilidades.4rlekiing.net/)
