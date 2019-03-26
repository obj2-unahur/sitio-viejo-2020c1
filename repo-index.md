---
layout: default

ejercicios:
  - name: Multipepita
    github: wollok/multipepita
    classroom: https://classroom.github.com/a/983lTmoo
  - name: Empanadas Giménez
    github: wollok/polimorfismoEmpanadasGimenez
    classroom: https://classroom.github.com/a/aO_2yfqS
  - name: Viajes en auto
    github: wollok/viajesEnAuto
    classroom: https://classroom.github.com/a/vYA0wLuw
  - name: Remiseria
    github: obj1-unahur/remiseria
    classroom: https://classroom.github.com/a/yhIG0GAi  
  - name: Spa
    github: wollok/spa
    classroom: https://classroom.github.com/a/Ai0icdEv
  - name: Juego con personajes y elementos
    github: wollok/juegoPersonajesElementos
    classroom: https://classroom.github.com/a/PZm1ETWq
  - name: Casa de Pepe y Julián
    github: obj1-unahur/casaDePepeYJulian
    classroom: https://classroom.github.com/a/waLnAp4R
  - name: Camión de transporte
    github: obj1-unahur/coleccionesCamionTransporte
    classroom: https://classroom.github.com/a/5p9d1U1y
  - name: Multipepita Recargada
    github: obj1-unahur-2018s2/multipepita-recargada
    classroom: https://classroom.github.com/a/lj_K-8cZ
  - name: Infraestructura ferroviaria
    github: obj1-unahur-2018s2/infraFerroviaria.git
    classroom: https://classroom.github.com/a/AV4jl0sg
  - name: Naves Espaciales
    github: wollok/naves-espaciales
    classroom: https://classroom.github.com/a/luD_7cg1
  - name: Obreros
    github: obj1-unahur/obreros
    classroom: https://classroom.github.com/a/dMPWviNb
  - name: Obreros (revisado)
    github: obj1-unahur/obreros-emergencia
    classroom: https://classroom.github.com/a/FuvfCiBL
  - name: Vendedores
    github: wollok/vendedores
    classroom: https://classroom.github.com/a/GOmaxpHu
  - name: Sueldo de Pepe (en Java)
    github: obj1-unahur/sueldo-pepe-java
    classroom: https://classroom.github.com/a/IcfQ0S9D
  - name: Ciudades
    github: obj1-unahur/ciudades
    classroom: https://classroom.github.com/a/huz89_kN
ejercicios-game:
  - name: Juego interactivo con Pepita - completo
    github: obj1-unahur/pepitaGame
    classroom: https://classroom.github.com/a/RA2D1K4z
  - name: Juego interactivo con Pepita (versión parcial)
    github: wollok/pepitaGame
    classroom: https://classroom.github.com/a/7jFBW_sF
ejercicios-extra:
  - name: Cumbre de software
    github: obj1-unahur/cumbre-software
    classroom: https://classroom.github.com/a/-A-FcNEZ
entregas:
  - name: Cosas que le gustan a distintas personas
    github: wollok/objetosGustos
    classroom: https://classroom.github.com/a/iQjzZW_g
  - name: Sueldo de Pepe
    github: wollok/polimorfismoSueldoDePepe
    classroom: https://classroom.github.com/a/Wntnv_vc    
  - name: Golosinas
    github: wollok/golosinas
    classroom: https://classroom.github.com/a/iOeEyp6H
  - name: Flota de rodados
    github: wollok/flotasDeRodados
    classroom: https://classroom.github.com/a/o7Yjdyae
  - name: Plagas
    github: obj1-unahur/plagas_enunciado
    classroom: https://classroom.github.com/a/DLVXji3G  
  - name: Oktubre Fest
    github: obj1-unahur/oktubre-fest
    classroom: https://classroom.github.com/a/XI94FuWy  

---
# Final 20/12/2018:
  [Classroom](https://classroom.github.com/a/K7AHavSw)

# Ejercicios para trabajar en clase

{% for ejercicio in page.ejercicios %}
  * {{ejercicio.name}} ([GitHub](https://github.com/{{ejercicio.github}}){% if ejercicio.classroom %} / [Classroom]({{ejercicio.classroom}}){% endif %})
{% endfor %}

<br>

Hay muchos más ejercicios para mirar en el [sitio GitHub de Wollok](https://github.com/wollok)

<br>

# Ejercicios para practicar

{% for ejercicio in page.ejercicios-extra %}
  * {{ejercicio.name}} ([GitHub](https://github.com/{{ejercicio.github}}){% if ejercicio.classroom %} / [Classroom]({{ejercicio.classroom}}){% endif %})
{% endfor %}

<br>

# Entregas

Ejercicios como los anteriores, pero que hemos elegido como mini trabajos prácticos. Consultá la fecha de entrega con tu docente amigo.

{% for ejercicio in page.entregas %}
  * {{ejercicio.name}} ([GitHub](https://github.com/{{ejercicio.github}}){% if ejercicio.classroom %} / [Classroom]({{ejercicio.classroom}}){% endif %})
{% endfor %}

# Wollok Game

En Wollok existe una herramienta visual para mostrar objetos, llamada Wollok Game. Eventualmente con ella se podrían hacer pequeños juegos, de ahí su nombre.

Si quieren investigar sobre esto les recomendamos que empiecen con [este ejemplo de Pepita](https://github.com/wollok/pepitaGame/tree/demoFirstClass). En el README del repositorio explica cómo hacerlo andar.

Otros ejercicios:
{% for ejercicio in page.ejercicios-game %}
  * {{ejercicio.name}} ([GitHub](https://github.com/{{ejercicio.github}}){% if ejercicio.classroom %} / [Classroom]({{ejercicio.classroom}}){% endif %})
{% endfor %}
