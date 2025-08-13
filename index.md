---
layout: default
---

# НАИМЕНОВАНИЕ ОРГАНИЗАЦИИ  
## ИНСТРУКЦИЯ ПОЛЬЗОВАТЕЛЯ  
### программа «Калькулятор» в Windows  
На 16 листах  
2025

---

## Содержание

{% for item in site.navigation %}
  {% if item.children %}
    ### {{ item.title }}
    <ul>
    {% for child in item.children %}
      <li><a href="{{ child.url }}">{{ child.title }}</a></li>
    {% endfor %}
    </ul>
  {% else %}
    - [{{ item.title }}]({{ item.url }})
  {% endif %}
{% endfor %}
