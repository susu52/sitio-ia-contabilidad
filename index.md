---
layout: default
title: Inicio
---

<!-- Hero Section -->
<section class="hero text-center">
    <div class="container">
        <h1 class="display-5 fw-bold mb-4">Explorando IA en Contabilidad</h1>
        <p class="lead mb-4">Un espacio para aprender y compartir sobre inteligencia artificial aplicada a la contabilidad</p>
        <a href="/blog" class="btn btn-light btn-lg">Ver Artículos</a>
    </div>
</section>

<!-- Sobre Mí Section -->
<section id="sobre-mi" class="section">
    <div class="container">
        <div class="row align-items-center">
            <div class="col-md-8">
                <h2 class="mb-4">Sobre Mí</h2>
                <p class="lead">Soy <strong>Guillermo Correa</strong>, contador público con varios años de experiencia.</p>
                <p>Actualmente estoy explorando cómo la inteligencia artificial puede transformar nuestra profesión, haciendo procesos más eficientes y permitiéndonos enfocarnos en lo que realmente importa: el análisis estratégico y la asesoría a nuestros clientes.</p>
                <p>En este espacio comparto <strong>mi proceso de aprendizaje</strong>, descubrimientos y reflexiones sobre esta fascinante intersección entre tecnología y contabilidad.</p>
            </div>
            <div class="col-md-4 text-center">
                <div class="bg-light p-4 rounded shadow">
                    <h5 class="mb-3">Mi Enfoque</h5>
                    <ul class="list-unstyled text-start">
                        <li class="mb-2">✅ Contabilidad tradicional</li>
                        <li class="mb-2">✅ Asesoría tributaria</li>
                        <li class="mb-2">🚀 IA aplicada a procesos</li>
                        <li class="mb-2">📊 Análisis de datos</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Blog Preview Section -->
<section class="section section-alt">
    <div class="container">
        <h2 class="text-center mb-5">Últimos Artículos</h2>
        
        <div class="row">
            {% for post in site.posts limit:3 %}
            <div class="col-md-4">
                <div class="card">
                    <img src="{{ post.image | default: '/assets/images/ai_accounting_3.png' }}" class="card-img-top" alt="{{ post.title }}">
                    <div class="card-body">
                        <span class="badge bg-primary mb-2">{{ post.categories[0] }}</span>
                        <h5 class="card-title">{{ post.title }}</h5>
                        <p class="card-text">{{ post.excerpt | strip_html | truncate: 120 }}</p>
                        <div class="d-flex justify-content-between align-items-center">
                            <small class="text-muted">{{ post.date | date: "%b %Y" }}</small>
                            <a href="{{ site.baseurl }}{{ post.url }}" class="btn btn-sm btn-outline-primary">Leer más</a>
                        </div>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
        
        <div class="text-center mt-4">
            <a href="/blog" class="btn btn-primary">Ver Todos los Artículos</a>
        </div>
    </div>
</section>

<!-- Servicios Section -->
<section id="servicios" class="section">
    <div class="container">
        <h2 class="text-center mb-5">Servicios Profesionales</h2>
        
        <div class="row">
            <div class="col-md-6 mb-4">
                <div class="card h-100">
                    <div class="card-body text-center">
                        <div class="mb-3">
                            <span style="font-size: 2rem;">📊</span>
                        </div>
                        <h5 class="card-title">Contabilidad Tradicional</h5>
                        <p class="card-text">Servicios contables completos para empresas y personas naturales, con los más altos estándares profesionales.</p>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 mb-4">
                <div class="card h-100">
                    <div class="card-body text-center">
                        <div class="mb-3">
                            <span style="font-size: 2rem;">💼</span>
                        </div>
                        <h5 class="card-title">Asesoría Tributaria</h5>
                        <p class="card-text">Optimización fiscal y cumplimiento normativo para maximizar beneficios dentro del marco legal.</p>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 mb-4">
                <div class="card h-100">
                    <div class="card-body text-center">
                        <div class="mb-3">
                            <span style="font-size: 2rem;">🤖</span>
                        </div>
                        <h5 class="card-title">Implementación de IA</h5>
                        <p class="card-text">Asesoría en la incorporación de herramientas de inteligencia artificial en procesos contables.</p>
                    </div>
                </div>
            </div>
            
            <div class="col-md-6 mb-4">
                <div class="card h-100">
                    <div class="card-body text-center">
                        <div class="mb-3">
                            <span style="font-size: 2rem;">📈</span>
                        </div>
                        <h5 class="card-title">Análisis de Datos</h5>
                        <p class="card-text">Transformación de datos financieros en insights accionables para la toma de decisiones.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Contacto Section -->
<section id="contacto" class="section section-alt">
    <div class="container">
        <h2 class="text-center mb-5">Contacto</h2>
        
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card">
                    <div class="card-body">
                        <div class="row text-center">
                            <div class="col-md-6 mb-3">
                                <h5>📧 Email</h5>
                                <p class="text-muted">guicolo52@gmail.com</p>
                            </div>
                            <div class="col-md-6 mb-3">
                                <h5>📍 Ubicación</h5>
                                <p class="text-muted">Colombia</p>
                            </div>
                        </div>
                        <div class="text-center mt-4">
                            <p class="text-muted">¿Interesado en conversar sobre contabilidad e IA? ¡No dudes en contactarme!</p>
                            <a href="mailto:guicolo52@gmail.com" class="btn btn-primary">Enviar Email</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
