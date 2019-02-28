# My Lab

Here's how you can add a check:

{% check %}
{{ exists }}
{% endcheck %}

{% next %}

Here's another (different) check:

{% check "Does your code compile?" %}
    {{ if compiles.passed }}
        Yes! Nicely done.
    {% else %}
        {{ compiles }}
    {% endif %}
{% endcheck %}
