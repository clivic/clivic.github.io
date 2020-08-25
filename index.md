---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{%- comment -%} # Clarence Hann's portfolio
> There are more projects being added. {%- endcomment -%}

# Projects:
<ul>
  {% for post in site.posts %}
    {%- if post.type == "normal" -%}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

# Projects during MS in Game Design:
<ul>
  {% for post in site.posts %}
    {% if post.type == "student" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

# About:
### Clarence is a passionate engineer devoted to learning new things from new people, in order to make interesting things. Asking search engines questions and making friends with talents are among his biggest hobbies.