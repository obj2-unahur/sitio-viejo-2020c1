---
layout: default
guias:
  - name: objetos
  - name: objetos
  - name: objetos
  - name: colecciones
  - name: clases
  - name: herencia
  - name: herencia
  - name: adicionales-1er-parcial
  - name: integradores
  - name: extras
---

# Guías de ejercicios en PDF

Ejercicios en formato "tradicional", que (aún) no tienen un proyecto en GitHub listo para clonar y empezar a trabajar.

{% for guia in page.guias %}
  [Guía {{forloop.index}} - {{guia.name}}](../guias_pdf/guia{{forloop.index}}-{{guia.name}}.pdf)
{% endfor %}
