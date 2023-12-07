---
layout: default
---

<header>
{% if site.theme_config.show_navbar == true %}
  {% include horizontal_list.html collection=site.data.home.navbar_entries %}
{% endif %}

  <h1>Build Your Forensics Workstation 🔬⚒️</h1>
  {% if site.theme_config.show_description == true %}
    <p>{{ site.description }}</p>
  {% endif %}
</header>


{% if site.theme_config.show_third_category == true %}
  <h2>{{ site.theme_config.home.title_third_category }}</h2>
  {% include card_list.html collection=site.data.home.third_category %}
{% endif %}


{% if site.theme_config.show_footer == true %}
  <footer>
    <div style="border: 2px solid red;"></div>
    {% include horizontal_list.html collection=site.data.home.footer_entries %}
  </footer>
{% endif %}
