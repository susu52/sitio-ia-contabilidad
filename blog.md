---
layout: default
title: Blog
permalink: /blog/
---

<section class="section">
    <div class="container">
        <h1 class="text-center mb-5">Blog - IA en Contabilidad</h1>
        
        <div class="row">
            {% for post in site.posts %}
            <div class="col-md-6 mb-4">
                <div class="card">
                    <img src="{{ post.image | default: '/assets/images/ai_accounting_5.jpg'}}" class="card-img-top" alt="{{ post.title }}">
                    <div class="card-body">
                        <span class="badge bg-primary mb-2">{{ post.categories[0] }}</span>
                        <h5 class="card-title">{{ post.title }}</h5>
                        <p class="card-text">{{ post.excerpt | strip_html | truncate: 150 }}</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small class="text-muted">{{ post.date | date: "%B %d, %Y" }}</small>
                            <a href="{{ post.url }}" class="btn btn-sm btn-outline-primary">Leer más</a>
                        </div>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</section>
