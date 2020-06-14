---
layout: page
title: Seasons of Code 2020
permalink: /soc/
---

<!-- about-soc -->
<section class="section">
  <div class="container">
    <div class="row">
      <div class="col-lg-10 mx-auto text-center">
        <h3> What is Seasons of Code? </h3>
        <br>
        <p class="font-secondary paragraph-lg text-dark">{{ site.data.settings.about-soc-what-is-soc }}</p>
        <br>
        <br>
        <h4>  Why should you participate? </h4>
        <p class="font-secondary paragraph-lg text-dark">{{ site.data.settings.about-soc-why-participate }}</p>
      </div>
    </div>
  </div>
</section>
<!-- /about-soc -->

<!-- join the force (from old website) -->
<section id="one" class="wrapper style2">
  <header class="major_soc">
    <h2>Join The Force</h2>
    <p>Do. Or do not. There is no try.</p>
  </header>
  <div class="container_soc">
    <div class="row">
      <div class="row_soc">
        <section class="special_soc box1_soc">
          <img class="icon major_soc" src="/svg/light-siber-one.svg" />
          <h3>Padawan</h3>
          <p>The Force is strong with you. <br> Train yourself to let go of everything you fear to lose. <br> The Force will be with you always.<br> Ready are you?</p><br />
          <a target="_blank" href="https://forms.gle/6hSaLUSB8Gfeogw7A" class="button big special">Become a Padawan</a>
        </section>
      </div>
      <div class="row_soc">
        <section class="special_soc box2_soc">
          <img class="icon major_soc" src="/svg/light-siber.svg" />
          <h3>Master</h3>
          <p>I can feel you code. <br> It gives you focus. It makes you stronger. <br> Your focus determines your reality. <br> Use the force <br> and someday you will be the most powerful Jedi ever.</p>
          <a target="_blank" href="https://goo.gl/forms/1WXW4oSDwlCHD4313" class="button big special">Become a Master</a>
        </section>
      </div>
    </div>
  </div>
</section>
<!-- /join the force (from old website) --  >


<!-- soc -->
<section class="section">
  <div class="container">
    <div class="row mb-5">
      <div class="col-12">
        <div class="btn-group btn-group-toggle justify-content-center d-flex" data-toggle="buttons">
          <label class="btn btn-sm btn-primary active">
            <input type="radio" name="shuffle-filter" value="all" checked="checked" />All
          </label>
          {% for label in site.data.settings.soc-label %}
          <label class="btn btn-sm btn-primary">
            <input type="radio" name="shuffle-filter" value="{{ label.type }}" />{{ label.title }}
          </label>
          {% endfor %}
        </div>
      </div>
    </div>
    <div class="row shuffle-wrapper">
      {% for item in site.data.settings.soc-items %}
      <div class="col-lg-4 col-6 mb-4 shuffle-item" data-groups="[{% for soc in item.soc-type %}{% if forloop.first == true %}{% else %},{% endif %}&quot;{{ soc.type }}&quot;{% endfor %}]">
        <div class="position-relative rounded hover-wrapper">
          <img src="{{ site.baseurl }}/{{ item.image }}" alt="{{ item.title }}" class="img-fluid rounded w-100 d-block">
          <div class="hover-overlay">
            <div class="hover-content">
              <a class="btn btn-light btn-sm" href="{{ item.url }}">view project</a>
            </div>
          </div>
        </div>
         <a href="{{ item.url }}">{{ item.title }}</a>
      </div>
      {% endfor %}
    </div>
  </div>
</section>
<!-- /soc -->

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