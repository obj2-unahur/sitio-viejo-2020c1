---
layout: default

semanas:
  - descripcion: |
      Vamos a presentar la materia y charlar un poco sobre diseño con objetos y la necesidad de herramientas para abordar           problemas más voluminosos usando la base de lo viste en Programación con Objetos I.
      
      Por favor completa ese formulario con tu nombre , mail y usuario de github [Información de contacto](https://forms.gle/WKYmpsr3HQSJwD197)

      Es casi imposible que hayas llegado a esta materia y no tengas tu cuenta en Github ... pero por si las moscas:
        * crearte una cuenta en [GitHub](https://github.com/)
        
      Hoy vamos a empezar a jugar con Java y buscar entre todos, que cosas tiene de parecidas a Wollok y en que cosas se      diferencia.
        
    ejercicios:
      - name: figuras
        repo: obj2-unahur/figuras
        classroom: https://classroom.github.com/a/Ku1IcSgB
        
 - descripcion: |
      Fue una semana corta, solo tuvimos una clase de 2 horas, continuamos con dudas sobre el ejercicio figuras.
        
    ejercicios:
      - name: figuras
        repo: obj2-unahur/figuras
        classroom: https://classroom.github.com/a/Ku1IcSgB
        
 - descripcion: |
      Presentamos la solución al ejercicio figuras.
      Vamos a ver temas nuevos con el lenguaje Java:
      * Interfaces
      * Introducción a colecciones en Java
      * Métodos equals / hashcode / toString
      * Introducción a Excepciones en Java
        
    ejercicios:
      - name: tp1-rocola
        repo: obj2-unahur/rocola
        classroom: https://classroom.github.com/a/_vqgzCtU        
        
        
    
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

{% endfor %}
