---
layout: eventLayout
title: Events
project: Git/GitHub Workshop
    
permalink: /events/event/git-github-workshop/
---

<h2 class="display1 m-3 p-3 text-center">{{page.project}}</h2>

{% for project in site.data.settings.events-items %}
{% if project.title == page.project %}
<div>
    <img src="{{ site.baseurl }}/{{ project.image }}"  width = "300" height="300" alt="{{ project.title }}" class="border rounded img-soc">
</div>

<div>
    <p class="display3" style = "font-size:20px;" >
        <br>
        Producing 2D images of a 3D world is inherently a lossy process, i.e. the entire geometric richness of 3D gets projected onto a single flat 2D image. We aim to create an API in Python which primarily reconstructs 3D volumes from 2D X-Ray Images.
<br><br>
We see this project as the first step towards a diagnostic tool in conditions where either no CT equipment or the education to interpret x-ray imagery is available, such as for mobile x-ray devices, lay users, or medical diagnostics in developing countries. The project is primarily divided into 2 parts:
<br><br>
    Implementation of various CNN architectures for 3D reconstruction from 2D images(3 people would be working on this part)
<br><br>
    Development of API(back-end framework for the above task).1 mentee would be working on this part.
<br><br>
Part 1 has some hard pre-requisites while anyone who has an interest in python or has done some basic programming in python or java-script can apply for part 2.
<br><br>
Pre-requisites for part 1: Must be familiar with any one of the following deep learning frameworks: Pytorch/Tensorflow/Theano/Keras. A basic idea of neural networks and machine learning is required. Previous experience in image processing is desired although is not a hard pre-requisite.
<br><br>
Interested people in this part should go through the following <a href='https://arxiv.org/pdf/1710.04867.pdf'>paper</a> while applying.
<br><br>
Note: If you are new to deep learning, it is recommended that you should go through the first 5 chapters of the <a href='https://www.goodreads.com/book/show/33986067-deep-learning-with-python'>book</a> before applying.
    </p>
</div>
<div>
    <h4 class="display3" style="margin:40px 0px 40px 0px;">Tentative Timeline :</h4>
    <table class="table table-striped">
    <thead>
        <tr>
        <th>Week</th>
        <th>Work</th>
        </tr>
    </thead>
    <tbody>
    <tr>
      <td style='width: 120px'>Week 1 and 2</td>
      <td>Reading of related material and learning relevant applications of the framework that would be used(mostly Keras and PyTorch)</td>
    </tr>
    <tr>
      <td>Week 3</td>
      <td>Testing and implementing Simple CNN architectures</td>
    </tr>
    <tr>
      <td>Week 4 and 5</td>
      <td>Working on Designing and implementation of 3D reconstruction from multiple images along with data pre-processing</td>
    </tr>
    <tr>
      <td>Week 6 and 7</td>
      <td>Programming and testing of various models for 3D reconstruction from single 2D image</td>
    </tr>
    <tr>
      <td>Week 8</td>
      <td>Further improvements on the models that have been created above.</td>
    </tr>
    </tbody>
    </table>
</div>
{% endif %}
{% endfor %}
