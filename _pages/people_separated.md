This is just a place holder with some useful code:

<!-- When there are a large number, do this -->

{% assign faculty = people| where: "role", "faculty" %}
{% assign postdoc = people | where: "role", "postdoc" %}
{% assign phd = people | where: "role", "phd" %}
{% assign masters = people | where: "role", "masters" %}
{% assign ra = people | where: "role", "ra" %}
{% assign alumnifaculty = people | where: "role", "alum-faculty" %}

{% include people-list.html arr=faculty title="Faculty" %}
{% include people-list.html arr=phd title="PhD" %}
{% include people-list.html arr=masters title="Masters" %}
