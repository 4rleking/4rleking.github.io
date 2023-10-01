---
layout: single
title: Metodología del Hackeo
excerpt: "Todo Hacker o ciberdelincuente tiene un modus operandi a la hora de buscar un objetivo e intentar buscar o introducirse en sus sistemas, en este apartado se explicará a detalle como funciona este sistema"
date: 2023-07-20
classes: wide
header:
  teaser: /assets/images/20230720/Intro.jpg
  teaser_home_page: true
categories:
  - Metodología
  - Hacking
tags:
  - Fundamentos
---

![](/assets/images/20230720/Intro.jpg)

La metodología del hackeo contiene los siguientes pasos:

1. Recopilación de información.
2. Intrusión.
3. Opcional: Garantizar un acceso futuro más fácil (Backdoor).
4. Reconocimiento interno.
5. Opcional: Movimiento (Escalamiento de privilegios).
6. Ejecución de la acción prevista.
7. Opcional: Borrado de pistas.

## Recopilación de información.

A menos que una herramienta automatizada lo esté ayudando a acceder de forma aleatoria a cualquier sitio vulnerable posible, el hacker suele tener un objetivo en mente.   Si un hacker quiere introducirse en una empresa determinada, lo primero que debe hacer es investigar todo cuanto pueda acerca de la empresa que lo ayude a entrar.

* Direcciones IP
* Correos electrónicos
* Nombres de Dominios

El hacker descubre sitios y servicios potenciales que puede acceder debido a que están conectados con la empresa. Utiliza medios de comunicación y los informes financieros públicos para averiguar quiénes son los altos cargos y/o encontrar nombres de empleados para implementar ingeniería social. Busca noticias para ver qué tipo de software nuevo han comprado recientemente, qué fusiones o separaciones se están produciendo (estos son siempre asuntos confusos y acompañados a menudo por una relajación o pérdida de la seguridad) y con qué socios interactúa. Muchas empresas se han visto afectadas a través de un socio mucho más débil.

Averiguar a qué activos digitales está conectada una empresa es la parte más importante de la recopilación de información en la mayoría de los ataques. No solo son los sitios y servicios principales (públicos) lo que normalmente se identifica, sino que para el atacante suele ser más útil localizar los sitios y servicios conectados menos populares, como portales de empleados y socios. Los sitios y servidores menos populares son más propensos a tener alguna debilidad en comparación con los sitios principales, con los cuales ya se han luchado durante años.

Todo buen hacker empieza recopilando todos los programas informáticos y los servicios alojados en cada uno de estos sitios, un proceso generalmente conocido como *(fingerprinting)*. Es muy importante saber qué sistemas operativos (OS) se utilizan y en qué versiones. Las versiones del sistema operativo pueden indicar a un hacker qué nivel de parches y errores de software existen o no existen.

Siempre es mejor hacer un inventario completo para obtener una imagen global del objetivo, pero suele pasar que en ocasiones se puede encontrar una vulnerabilidad (grave o crítica) muy pronto y simplemente saltar al paso siguiente. A menos que se detecte una vulnerabilidad tan rápido, cuanta más información tenga acerca de lo que se está ejecutando, mejor. Cada programa informático y versión adicional proporciona posibles vectores de ataque adicionales.

**Nota:** Algunos hackers denominan la recopilación de información general y no técnica como *(footprinting)* y el mapeado del sistema operativo y los programas informáticos como *(fingerprinting)*.

A veces, cuando un hacker se conecta a un servicio o sitio, este responde amablemente con información de versión muy detallada, por lo que no se necesita ninguna herramienta. Cuando esto no es así, existen muchas herramientas de ayuda para el *fingerprinting* del sistema operativo y aplicaciones.

- [Nmap](https://nmap.org)
- [Nikto2](https://cirt.net/Nikto2)

## Intrusión

Este es el paso que da nombre al hacker. El éxito de este paso es crucial para todo el ciclo. Si el hacker ha hecho sus deberes en la etapa del *fingerprinting*, esta etapa realmente no es difícil. Siempre hay software antiguo, cosas sin parchear e, incluso, algo mal configurado en la recopilación de software identificado.

Si, afortunadamente, todo el software y los dispositivos son perfectamente seguros (y nunca lo son), puedes atacar al *elemento humano*, que es siempre la parte más débil de la ecuación. Pero sin la intrusión inicial, el hacker lo tiene todo perdido. Afortunadamente para él, hay muchas maneras de entrar en el objetivo. Estas son las diferentes técnicas que un hacker puede utilizar para ello:

+ Ataque de día cero.
+ Software sin parche.
+ Software malicioso o malware.
+ Ingeniería social.
+ Problemas con contraseñas.
+ Ataque de intermediario (MitM).
+ Fuga de información.
+ Configuración errónea.
+ Ataque de denegación de servicio.
+ Información privilegiada (socio/asesor/proveedor/terceros).
+ Error de usuario.
+ Acceso físico.
+ Escalada de privilegios.

### Ataque de día cero

Los ataques *(Exploits)* de día cero no son tan frecuentes como las vulnerabilidades habituales, que los proveedores normalmente ya han parcheado hace tiempo. Un ataque de día cero es aquel para el cual el software objetivo todavía no ha sido parcheado y la gente (y normalmente el proveedor) lo desconocen. 

Cualquier sistema informático que utilice un software con un error de día cero es esencialmente explotable a voluntad, a menos que la víctima potencial desinstale el software o haya colocado en su lugar algún tipo de solución (cortafuegos, una lista de control de acceso [ACL], segmentación de VLAN, software anti desbordamiento de búfer, entre otros).

Los ataques de día cero son vulnerabilidades menos conocidas que las habituales, dado que no pueden ser ampliamente utilizadas por un atacante. Si un atacante lleva a cabo un ataque de día cero, el valioso agujero será descubierto y parcheado por los fabricantes y colocado en firmas *antimalware*. 

Actualmente la mayoría de los fabricantes pueden parchear nuevas explotaciones en unas horas o hasta pocos días después de su descubrimiento. Cuando se lanza un ataque de día cero, o bien se utiliza contra muchos objetivos al mismo tiempo para una mayor posibilidad de explotación o bien (a fuego lento), que significa con moderación, a veces y solo cuando se necesita. 

Los mejores hackers profesionales del mundo suelen tener colecciones de ataques de día cero que solo utilizan cuando todo lo demás falla, y de tal forma que pasen totalmente desapercibidos. Un ataque de día cero debe utilizarse para conseguir un acceso inicial a un objetivo especialmente resistente; después, todas las pistas deberán ser eliminadas y, a partir de ese punto, se utilizarán métodos más tradicionales.

### Software sin parchear

El software sin parchear es siempre una de las razones más frecuentes por las que un ordenador o un dispositivo es explotado. Cada año, hay miles (normalmente, entre 5,000 y 6,000; o 15 al día) nuevas vulnerabilidades anunciadas públicamente entre todo el software más utilizado; puedes revisar las estadísticas reportadas en cada edición de [Microsoft Security Intelligence Report](Http://microsoft.com/sir).

Por lo general, los fabricantes han mejorado en el desarrollo de código más seguro y la localización de sus propios errores; sin embargo, existe un número cada vez más elevado de programas y billones de líneas de código, por lo que el número total de errores se ha estabilizado relativamente durante las dos décadas anteriores.

La mayoría de los fabricantes realizan un buen trabajo parcheando sus programas de una manera oportuna, especialmente después de que una vulnerabilidad se haga pública. Desgraciadamente, los clientes tardan mucho en aplicar sus parches, llegan incluso a desactivar las rutinas automáticas de aplicación de parches establecidas por el fabricante. Un porcentaje moderado de usuarios no parchean nunca su sistema. Hay quien ignora las múltiples advertencias sobre parches y simplemente le aburren o desconoce que un parche deba aplicarse. (Por ejemplo, muchos sistemas de puntos de venta no notifican al cajero que es preciso aplicar un parche). La mayoría de los ataques de software ocurren contra programas que no han sido parcheados en muchos años.

Aunque una empresa concreta o un usuario parchee una vulnerabilidad crítica en cuanto esta se anuncia, un hacker paciente y persistente puede esperar a que se anuncie dicho parche, que está en el inventario de *fingerprinting* de su objetivo, y lanzar el correspondiente ataque antes de que el defensor tenga tiempo de parchearlo. (Es relativamente fácil para un hacker hacer ingeniería inversa de un parche y descubrir como explotar una vulnerabilidad en concreto).

### Software malicioso o malware

Los programas maliciosos se conocen como *malware* y los tipos tradicionales más conocidos son los virus, troyanos y gusanos, aunque el malware actual suele ser una mezcla de varios tipos. El malware permite al hacker utilizar un método de explotación para atacar más fácilmente a sus víctimas o llegar a un mayor número de víctimas de forma más rápida.

Cuando se descubre un nuevo método de explotación, los defensores saben que los desarrolladores de malware utilizarán malware automatizado para difundir la explotación más rápidamente en un proceso denominado *weaponization* de la explotación lo que genera un mayor riesgo para el usuario final y la sociedad.

Sin malware, un atacante está obligado a implementar un ataque contra una víctima a la vez; con malware, millones de víctimas pueden ser explotadas en cuestión de minutos.

### Ingeniería social

Una de las estrategias de hackeo más exitosas es la *ingeniería social*. La ingeniería social, ya sea llevada a cabo manualmente por un adversario humano o mediante un método automatizado, es un truco de hackers que consiste en engañar a un usuario final para que haga algo perjudicial para su propio ordenador o seguridad.

Puede ser un correo electrónico que engaña al usuario para que haga clic sobre un vínculo web malicioso o que ejecute un archivo adjunto falso. También puede ser algo o alguien que engaña a un usuario para que revele su información privada de acceso *(phishing)*. 

La ingeniería social ha sido muy frecuente en los ataques perpetrados por hackers. El que fue durante mucho tiempo hacker de sombrero blanco, [Kevin Mitnick](https://muycritico.com.ar/2016/10/kevin-mitnick-biografia-completa-del-hacker-mas-famoso-del-mundo-2/), solía ser uno de los mejores ejemplos de ingenieros sociales maliciosos.

### Problemas con contraseñas

Las contraseñas o sus derivaciones almacenadas internamente pueden ser descifradas o robadas. Durante mucho tiempo, adivinar contraseñas (o la ingeniería social) era uno de los métodos más populares para conseguir el acceso inicial a un sistema informático o una red, y lo sigue siendo. 

Sin embargo, el robo de credenciales y su reutilización (como los ataques *pass-the-hash*) ha entrado por la puerta grande en el campo del hackeo de contraseñas en la última media década. 

Mediante el robo de contraseñas, el atacante normalmente consigue el acceso administrativo a un ordenador o dispositivo y recupera una o más credenciales de inicio de sesión almacenadas en el sistema (memoria o disco duro). 

Las credenciales robadas se utilizan después para acceder a otros sistemas que aceptan los mismos datos de inicio de sesión. Casi todos los grandes ataques corporativos han tenido el robo de credenciales como componentes de explotación común, tanto es así que la técnica del descifrado de contraseñas ya no se utiliza tanto.

### Ataque de intermediario (MitM)

El ataque de intermediario o de *Main-in-the-Middle (MitM)* pone en peligro una conexión de red legítima para obtener acceso a las comunicaciones o participar de ellas maliciosamente. 

La mayoría de los ataques de intermediario ocurren por fallos de red o de protocolos de aplicación, aunque también pueden llevarse a cabo por un error humano. Actualmente, los ataques de intermediario se producen en redes inalámbricas.

### Fugas de información

La fuga de información privada puede ser el resultado de una de las formas de hackeo existentes o bien de una acción humana no intencionada (o intencionada). La mayor parte de las fugas de información ocurren a causa de una ubicación descuidada de la misma (y con poca protección) o porque algún hacker ha descubierto el modo de acceder a datos que eran privados. 

No obstante, los ataques internos, donde un empleado o empresario roba o utiliza de forma intencionada información privada, también es una forma común de hackeo.

### Configuración errónea

También resulta común para usuarios y administradores de ordenadores implementar (a veces sin saberlo) opciones de seguridad muy débiles. Es decir, en un sitio web público se han encontrado que la mayoría de los archivos críticos estaban marcados con permisos del grupo (Todo o Público); y estos permisos son exactamente lo que parecen. Cuando se permite a todo el mundo acceder a todos los archivos que desee, el sitio o los archivos almacenados en él dejarán de ser privados en poco tiempo.

### Ataque de denegación de servicio

Incluso si no hay nadie que haya cometido un error o que haya dejado una pequeña parte de un software sin parchear, todavía es posible hacer caer de Internet casi cualquier sitio web o cualquier ordenador. Aunque el administrador sea perfecto, el ordenador depende de uno o más servicios (ancho de banda), que él no los controla.

Hoy en día, los grandes *ataques de denegación de servicio distribuido (DDoS)* pueden hacer caer o perjudicar de forma importante casi cualquier sitio web u ordenador conectado a Internet.

Estos ataques suelen contener miles de millones de paquetes por segundo, lo que sobrecarga el objetivo (o sus vecinos de origen o destino).

Existen decenas de servicios comerciales (a veces ilegales) que cualquiera puede utilizar tanto para causar un enorme ataque DDoS como para defenderse de él.

### Información privilegiada (socio/asesor/proveedor/terceros)

Incluso si toda la red y sus ordenadores están perfectos (que no lo están), puede ocurrir un fallo en un ordenador conectado de un socio o de un empleado interno. Esta categoría es muy amplia e implica varios de los métodos de hackers.

### Error de usuario

Esta categoría de intrusión también implica varios métodos de hackeo. Por ejemplo, un usuario puede enviar de forma accidental información privada a un usuario no autorizado simplemente introduciendo un carácter mal escrito en una dirección de correo electrónico.

Otro usuario puede olvidarse por error de parchear un servidor en riesgo o configurar un permiso equivocado. Un error común de usuario es cuando alguien responde a un correo electrónico pensando que dicha respuesta es privada o que va dirigida a una breve lista de gente, pero en realidad está contestando a una amplia lista o, incluso a alguien de quien se está hablando mal.

### Acceso físico

El saber popular dice que, si un atacante tiene acceso físico a un activo, este simplemente lo robará todo; y esta percepción se ha demostrado bastante precisa hasta el momento, incluso contra las defensas que están explícitamente destinadas a proteger dicho activo ante cualquier ataque físico.

Por ejemplo, muchos programas de cifrado de discos pueden ser vencidos por el atacante con un microscopio electrónico para obtener las claves secretas de protección identificando por separado los electrones que componen dichas claves. O la RAM puede congelarse con aire comprimido para traducir la clave secreta encriptada en texto sin cifrar debido a un fallo en la manera en que la memoria almacena físicamente la información.

### Escalada de privilegios

Cada hacker utiliza uno de los métodos de intrusión descritos anteriormente para explotar inicialmente un sistema objetivo. La única cuestión tras haber conseguido entrar es con qué tipo de acceso de seguridad se encontrará.

Si están explotando un programa o un servicio informático que se ejecuta en el contexto de seguridad del mismo usuario, solo tendrán por el momento los mismos privilegios y permisos de acceso que el usuario conectado.

O pueden conseguir el *Santo grial* del sistema y obtener el acceso completo al sistema administrativo. Si el atacante solo cuenta con permisos de acceso normales y sin privilegios, entonces, por lo general ejecuta un segundo ataque de escalada de privilegios para intentar obtener un mayor acceso privilegiado.

Los ataques de escalada de privilegios abarcan toda la gama, esencialmente duplicando los mismos enfoques que para la intrusión, pero empiezan por el punto de partida más alto de tener como mínimo algún acceso.

Los ataques de escalada de privilegios son generalmente más fáciles de llevar a cabo que las explotaciones iniciales. Y como dichas explotaciones tienen el éxito siempre garantizado, la escalada de privilegios resulta mucho más fácil.

## Garantía de un acceso futuro más fácil (Backdoor)

Aunque es opcional, una vez que el atacante ha obtenido el acceso inicial, la mayoría de los hackers trabajan implementando un método adicional que asegure que podrán acceder de forma más rápida y sencilla al mismo objetivo o software la próxima vez. Para muchos hackers, esto significa situar una *puerta trasera (backdoor)* conocida por la cual puedan conectarse directamente en ocasiones futuras.

Otras veces, significa descifrar contraseñas o crear nuevas cuentas. El atacante siempre puede utilizar las mismas explotaciones que ya han funcionado con éxito la última vez para conseguir el acceso inicial, pero por lo general quiere otro método que funcione incluso si la víctima soluciona el problema que antes funcionaba.

## Reconocimiento interno

Una vez que la mayoría de los hackers han accedido al sistema, empiezan a ejecutar múltiples comandos o programas para saber más sobre el objetivo y qué es lo que está conectado a él. 

Por lo general, esto significa buscar conexiones de redes en la memoria y en el disco duro, e identificar usuarios, recursos compartidos, servicios y programas. Toda esta información se utiliza para entender mejor el objetivo y sirve como punto de inicio para el siguiente ataque.

## Movimiento

No es habitual que el atacante o el malware se contente con acceder solo a un objetivo. Casi todos los hackers y los programas maliciosos quieren difundir su área de influencia por más y más objetivos. Una vez han conseguido acceder al objetivo inicial, propagar esta influencia dentro de la misma red o entidad es muy sencillo.

Si el atacante se mueve hacia otros objetivos similares con usos parecidos, se denomina *movimiento lateral*; pero si el atacante pasa de dispositivos con un privilegio a privilegios más altos o más bajos, se denomina *movimiento vertical*.

La mayoría de los atacantes se mueven de bajos a altos niveles de privilegios utilizando técnicas de movimiento vertical. Por ejemplo, una metodología común de hacker es que primero el atacante comprometa una única estación de trabajo de un usuario. Utilizará este acceso inicial para buscar y descargar contraseñas de cuentas administrativas locales. Después, si estas credenciales administrativas están compartidas con otras máquinas (que a menudo lo están), entonces se mueve horizontalmente y repite el proceso hasta que captura accesos a cuentas muy privilegiadas.

A veces, esto se produce inmediatamente durante la primera intrusión, porque el usuario o el sistema conectado ya cuenta con privilegios altos.

A continuación, se mueve hasta el servidor de autenticación y obtiene todas las credenciales de conexión del usuario. Este es el modo operandi estándar para la mayoría de los grupos de hackers actualmente, e ir del compromiso inicial a la obtención de una red completa (o *pwning*) puede suponer menos de 1 hora.

## Ejecución de la acción prevista

Una vez que el acceso está garantizado y la propiedad del activo obtenida, los hackers llevan a cabo lo que tienen previsto hacer (a menos que el acceso haya puesto al descubierto un objetivo nuevo). Todos los hackers tienen previsiones.

Un pentester legítimo tiene la obligación por contrato de hacer una o varias cosas. Un hacker malicioso difundirá algún malware, leerá o robará información confidencial, hará modificaciones perjudiciales o causará daños.

La única razón que tiene el hacker para poner en riesgo uno o más sistemas es hacer algo. Hace algún tiempo (2 o 3 décadas atrás), a la mayoría de los hackers simplemente les bastaba demostrar que habían hackeado un sistema. Hoy en día, el hackeo tiene un 99% de motivación criminal y el hacker tiene que hacer algo malicioso a su objetivo (aunque el único daño que haga sea permanecer infiltrado de forma silenciosa esperando una futura acción potencial). El acceso no autorizado sin daños directos también es un daño.

## Borrado de pistas

Algunos hackers intentarán borrar sus pistas. Esto es lo que solían hacer todos los hackers hace unos años, pero actualmente los sistemas informáticos son tan complejos y tienen tantos números que la mayoría de los propietarios de activos no comprueban la existencia de pistas de hacker. No comprueban los inicios de sesión, no comprueban los cortafuegos y no buscan signos de hackeo ilegal a menos que estos no les golpeen en la cara.

Cada año, el [Data Breach Investigations Report de Verizon](http://www.verizonenterprise.com/verizon-insights-lab/dbir/) informa que la mayoría de los atacantes pasan desapercibidos durante meses y años y que un 80% de los ataques se podrían haber detectado si los defensores se hubieran preocupado de mirar.

Gracias a estas estadísticas, la mayoría de los hackers ya no se molestan en borrar sus pistas.

Actualmente es cuando los hackers deben borrar menos sus pistas, puesto que utilizan métodos que nunca serán localizados mediante la detección de acciones de hacker tradicionales. Lo que utiliza el hacker es tan común en el entorno de la víctima que es casi imposible distinguir entre actividades legítimas e ilegítimas.

Por ejemplo, una vez dentro, el hacker normalmente lleva a cabo acciones en el contexto de la seguridad de un usuario legítimo, a menudo accediendo a los mismos servidores y servicios que dicho usuario. Y además utiliza las mismas herramientas (programas de acceso remoto y lenguajes de script) que el administrador.