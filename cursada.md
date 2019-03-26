---
layout: default

semanas:
  - descripcion: |
      Vamos a trabajar con un ejercicio de diagnóstico, cuyo enunciado podés encontrar [acá]().

      Además vas a tener que cumplir algunos pasos administrativos:
        * completar la encuesta de inicio de curso, [acá](https://goo.gl/forms/OKvLH5ivKYyx0fBi1);
        * crearte una cuenta en [GitHub](https://github.com/);
        * registrarte en Mumuki: [acá si cursás a la tarde](https://mumuki.io/wollok-obj1/join/6NvUVA) y [acá si cursás a la noche](https://mumuki.io/wollok-obj1/join/Bj85hg).
        **Ojo:** podés entrar con tu cuenta de Google, de GitHub o crearte una nueva dentro de Mumuki con mail y contraseña. Lo importante es que entres _siempre de la misma forma_, caso contrario no podremos registrar correctamente tu progreso
    ejercicios:
      - name: Multipepita
        repo: wollok/multipepita
        classroom: https://classroom.github.com/a/4pxDNIhk
    mumuki:
      guia: Personas y barrios - qué anda, qué no, cuánto da
      url: https://mumuki.io/wollok-obj1/lessons/482-objetos-y-mensajes-personas-y-barrios-que-anda-que-no-cuanto-da
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
