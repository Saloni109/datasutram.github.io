---
layout: page
title: Projects
category: project
comments: true
---


# Projects

<table>
    <tr>
        <th>Name</th>
        <th>Points</th>
        <th>Completed</th>
    </tr>
    {% for post in site.categories[page.category] %}
        <tr>
            <td> <a href="{{ post.url | absolute_url }}">{{ post.title }}</a> </td>
            <td>  {{ post.points}} </td>
            <td>  {{post.status}}  </td>
        </tr>
    {% endfor %}
</table>
