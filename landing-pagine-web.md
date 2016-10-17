---
layout: landing
title: Web Design
description: Sviluppo per te Squeeze e Landing Pages.
image: assets/images/pic07.jpg
nav-menu: yes
---

<!-- Banner -->
<!-- Note: The "styleN" class below should match that of the header element. -->
<section id="banner" class="style1">
	<div class="inner">
		<span class="image">
			<img src="{{ site.baseurl }}/{{ page.image }}" alt="" />
		</span>
		<header class="major">
			<h1>FAI APPREZZARE E CONOSCERE IL TUO BUSINESS</h1>
		</header>
		<div class="content">
			<p>{{ page.description }}</p>
		</div>
	</div>
</section>

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h2>LANDING PER TUTTI I GUSTI</h2>
		</header>
		<p>Creiamo pagine web professionali per promuovere il tuo business, te stesso, i tuoi prodotti oppure catturare contatti di business o lavoro.</p>
	</div>
</section>

<!-- Two -->
<section id="two" class="spotlights">
	<section>
		<a href="generic.html" class="image">
			<img src="assets/images/pic08.jpg" alt="" data-position="center center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Create con cura</h3>
				</header>
				<p>Tutte i nostri progetti sono sviluppati con i migliori strumenti disponibili sul mercato, i quali garantiscono un prodotto corretto, robusto, versatile e durevole nel tempo.</p>
				<ul class="actions">
					<li><a href="generic.html" class="button">Dimmi di più</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="assets/images/pic09.jpg" alt="" data-position="top center" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Responsive Design</h3>
				</header>
				<p>Ogni nostro prodotto è sviluppato con un layout fluido che si adatta al tipo di display in cui è visualizzato, una delle principali caratteristiche che distingue un moderno website da uno obsoleto.</p>
				<ul class="actions">
					<li><a href="generic.html" class="button">Dimmi di più</a></li>
				</ul>
			</div>
		</div>
	</section>
	<section>
		<a href="generic.html" class="image">
			<img src="assets/images/pic10.jpg" alt="" data-position="25% 25%" />
		</a>
		<div class="content">
			<div class="inner">
				<header class="major">
					<h3>Contatti e sicurezza</h3>
				</header>
				<p>Utilizziamo e consigliamo i migliori strumenti sul mercato per il tuo web marketign e email marketing implementando nei nostri prodotti i migliori servizi offerti da web. Implementiamo e ci affidiamo a servizi e strutture sicure.</p>
				<ul class="actions">
					<li><a href="generic.html" class="button">Dimmi di più</a></li>
				</ul>
			</div>
		</div>
	</section>
</section>

<!-- Three -->
<section id="three">
	<div class="inner">
		<header class="major">
			<h2>Esempi</h2>
		</header>
		<p>Alcuni esempi che possono essere applicati al tuo business o a tutto ciò che vorresti comunicare su web.</p>
		<ul class="actions">
			<li><a href="generic.html" class="button next">Avanti</a></li>
		</ul>
	</div>
</section>

<section id="one" class="tiles">
	{% for post in site.posts limit:site.tiles-count %}
	{% if site.tiles-source == 'posts' %}
        <article>
                <span class="image">
                        <img src="{{ post.image }}" alt="" />
                </span>
                <header class="major">
                        <h3><a href="{{ site.baseurl }}{{ post.url }}" class="link">{{ post.title }}</a></h3>
                        <p>{{ post.description }}</p>
                </header>
        </article>
	{% endif %}
	{% endfor %}
	{% for page in site.pages limit:site.tiles-count %}
	{% if site.tiles-source == 'pages' %}
        <article>
                <span class="image">
                        <img src="{{ page.image }}" alt="" />
                </span>
                <header class="major">
                        <h3><a href="{{ site.baseurl }}{{ page.url }}" class="link">{{ page.title }}</a></h3>
                        <p>{{ page.description }}</p>
                </header>
        </article>
	{% endif %}
	{% endfor %}


</section>


</div>
