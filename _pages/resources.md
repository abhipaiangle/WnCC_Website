---
layout: page
title: Resources
permalink: /resources/
---
<!-- blog -->

{% for item in site.data.settings.resources-items %}
<section class="section bg-light">
<div class="container">
        <div class="col-12 text-center">
            <h2 class="section-title">{{ item.title }}</h2>
            <p>{{ item.fdis }}</p>
        </div>

<!-- Programming_101 -->

<div class="row">
            <!-- {% for label in site.data.settings.{{ item.name }} %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %} -->
            {{ if forloop.index = 1 }}
            {% for label in site.data.settings.wiki %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}
            {{ endif }}
            
            {{ if forloop.index = 2 }}
            {% for label in site.data.settings.ciq %}
            <div class="col-lg-4 col-sm-6 mb-4">
                <article class="card shadow">
                    <img class="rounded card-img-top" src="{{ site.baseurl }}/assets/images/resources/{{ label.image }}"
                        alt="{{ label.title }}">
                    <div class="card-body">
                        <h4 class="card-title"><a class="text-dark"
                                href="{{ label.link }}" target="_blank">{{ label.title }}</a></h4>
                        <p class="cars-text">{{ label.discription }}
                        </p>
                        <a href="{{ label.link }}" class="btn btn-xs btn-primary" target="_blank">Read More</a>
                    </div>
                </article>
            </div>
            {% endfor %}
            {{ endif }}


</div>
<p>{{ item.ldis }}</p>
<div style="display: flex; align-item: center; justify-content: center;">
<a href="{{ item.btn-link }}" class="btn btn-xs btn-primary" target="_blank">{{ item.btn-title }}</a>
</div>
</div>
</section>

{% endfor %}


<!-- /blog -->

<!-- clients -->
<section class="section bg-light">
  <div class="container">
    <div class="row">
      <div class="col-12 text-center">
        <h2 class="section-title">My Clients</h2>
      </div>
    </div>
    {% include client-slider.html %}
  </div>
</section>
<!-- /clients -->
