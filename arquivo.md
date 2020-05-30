---
layout: page
title: Arquivo
---

    <section>
        <table>
            {% for post in site.posts %}
            <tr>
                <td><i class="icon-clock"></i> <time datetime="{{post.date | date: "%d/%m/%Y"}}">{{post.date | date: "%d/%m/%Y"}}</time></td>  
                <td><a href="{{ post.url }}">{{ post.title }}</a></td>
            </tr>
    	{% endfor %}
        </table>
    </section>
