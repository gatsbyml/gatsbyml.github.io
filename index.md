---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults

title: Home
layout: home
---

## Time & Location
Usually on Monday 1:30pm-3pm at the [Gatsby Unit,
UCL](http://www.gatsby.ucl.ac.uk/) 3th floor seminar room. Please subscribe to
[our mailing
list](https://groups.google.com/forum/#!forum/gatsby-ml-reading-group) to
receive announcements of upcoming talks. To enter the building, see
[here](about/).

## Events

<style>
    td {
        margin: 0;
        padding: 5px;
    
    }

    tr:nth-child(even) {
        background-color: #f2f2f2;
    }
</style>


<p style="font-size: 0.8em; color: black;">
Updated: {{ site.time | date: "%d-%b-%y" }}  <br>
</p>

<table>
    <tr>
        <th style="width: 15%;">Date</th>
        <th>Presenter</th>
        <th style="width: 40%;">Topic</th>
        <th>Reading</th>
        <th>Supplement</th>
    </tr>

    {% for talk in site.data.events %}
    <tr>
        <td>{{ talk.date | date_to_string }}</td>
        <td>{{ talk.presenter | markdownify }}</td>
        <td>{{ talk.topic | markdownify }}</td>
        <td>{{ talk.reading | markdownify }}</td>
        <td>{{ talk.supplement | markdownify }}</td>
    </tr>
    {% endfor %}
</table>

<!--{{ talk.date }}: <a href="{{ talk.slides }}">{{ talk.title }}</a>-->
<!--{% if talk.at %}-->
<!--at {{ talk.at | markdownify }}-->
<!--{% endif %}-->

