# ¡Bienvenido a mi Blog de Física!

Soy [Tu Nombre], experto en [tu especialidad]. En este blog comparto:

- Cálculos interesantes que no son papers
- Análisis de sistemas físicos complejos
- Ejemplos prácticos de teoría
- Herramientas computacionales

## Posts Recientes

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
