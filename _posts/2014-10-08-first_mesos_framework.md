---
layout: post
title: Cómo desarrollar tu primer aplicación distribuida con Mesos 
---
Como desarrolladores muchos nos hemos encontrado en algún momento dado
con la necesidad de construir una applicación distribuida ya sea para
aprovechar la potencia de procesamiento de un cluster, 
o bien porque necesitamos trabajar
con sistemas que se encuentran repartidos en distintos servidores en
un cluster.

*¿Qué es Mesos?*

Mesos es un gestor que permite ejecutar de manera sencilla
applicaciones distribuidas. Mesos es útil porque proporciona mecanismos
para tratar toda una serie de problemas que se presentan de forma habitual
en el desarrollo de la mayoría de aplicaciones distribuidas.

*Problemas al construir SISDIS* de reinventar la rueda:

- En cuanto hay varias aplicaciones que se ejecutan en el cluster se
  plantea el problema de cómo se pueden *repartir los recursos*.
- Cada vez hay que definir un sistema de *tolerancia a fallos* en
  caso de que un nodo del cluster tenga un problema (*failover*).
- Cada vez es necesario definir una manera apropriada de ejecutar
  tareas de forma remota en una máquina específica (*ejecución remota*).
- El Planificador no puede ser un cuello de botella.
- Cómo implementar el intercambio de mensajes entre distintas instancias
  de la aplicación.


Mesos facilita las tareas de gestión de los
recursos del cluster, de recuperación autómatica ante el fallo de uno
de los nodos o de intercambio de mensajes entre las distintas instancias
de una aplicación que se ejecutan en cada nodo.


Utilizaremos el ejemplo de una aplicación distribuida (de tratamiento
de datos en paralelo) para introducir los conceptos básicos de Mesos
*ejemplo*

*Cómo hacer esto con Mesos*

Para 
funcionalidades las aplicaciones sólo necesitan implementar dos
interfaces definidas en la API de Mesos conocidas como ejecutor y
planificador (o scheduler)

*¿Como funciona Mesos?*

Mecanismo de ofertas


*Ejemplo: mi primer framework*


![_config.yml]({{ site.baseurl }}/images/config.png)


[Viadeo Profile](http://www.viadeo.com/profile/002lz309wldwqir)
[LinkedIn Profile](https://www.linkedin.com/pub/i%C3%B1igo-mediavilla/3a/700/276)


