---
layout: default

semanas:
  - descripcion:
      Vamos a presentar la materia y charlar un poco sobre diseño con objetos y la necesidad de herramientas para abordar           problemas más voluminosos usando la base de lo viste en Programación con Objetos I.

      Vamos a empezar a Jugar un poco con el ecosistema Java con el siguiente enunciado [figuras]()

      Es casi imposible que hayas llegado a esta materia y no tengas tu cuenta en Github ... pero por si las moscas:
        * crearte una cuenta en [GitHub](https://github.com/);
        
    ejercicios:
      - name: Multipepita
        repo: unahur-obj2/multipepita
        classroom: https://classroom.github.com/a/4pxDNIhk
    
---
# Semana a semana

{% for semana in page.semanas reversed %}

## Semana {{forloop.rindex}}
{{semana.descripcion}}

{% if semana.ejercicios %}
### Ejercicios para trabajar en clase
<table>
    <thead>
        <tr class="header">
            <th>Nombre</th>
            <th>GitHub Classroom</th>
            <th>Repositorio original</th>
        </tr>
    </thead>
    <tbody>
      {% for ej in semana.ejercicios %}
      <tr>
          <td markdown="span">{{ej.name}}</td>
          <td markdown="span">[Clonar el ejercicio]({{ej.classroom}}) <i class="fas fa-book"></i></td>
          <td markdown="span">[Ver repositorio](https://github.com/{{ej.repo}}) <i class="fab fa-github"></i></td>
      </tr>
      {% endfor %}
    </tbody>
</table>
{% endif %}

{% if semana.mumuki %}
### Mumuki

Te recomendamos resolver la guía [{{semana.mumuki.guia}}]({{semana.mumuki.url}}).
{% endif %}

{% endfor %}
