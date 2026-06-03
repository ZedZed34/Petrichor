<svelte:head>
	<title>Aura Handcrafted | Beautiful Artisan Jewelry</title>
</svelte:head>

<section class="hero">
	<div class="hero-content">
		<h1>Elegance in Every Detail</h1>
		<p>Discover unique, handmade jewelry designed to highlight your natural aura.</p>
		<a href="/shop" class="btn">Shop the Collection</a>
	</div>
</section>

<section class="featured container">
	<h2>Featured Pieces</h2>
	<div class="grid">
		<div class="card">
			<div class="placeholder-img ring">
				<!-- SVG representation of a ring -->
				<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
					<circle cx="50" cy="50" r="30" stroke="var(--color-primary)" stroke-width="6"/>
					<polygon points="50,15 55,25 45,25" fill="var(--color-accent)"/>
				</svg>
			</div>
			<div class="card-info">
				<h3>Rose Quartz Ring</h3>
				<p>$45.00</p>
			</div>
		</div>
		<div class="card">
			<div class="placeholder-img necklace">
				<!-- SVG representation of a necklace -->
				<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M20,30 Q50,90 80,30" stroke="var(--color-primary)" stroke-width="4" fill="none"/>
					<circle cx="50" cy="61" r="8" fill="var(--color-accent)"/>
				</svg>
			</div>
			<div class="card-info">
				<h3>Delicate Gold Chain</h3>
				<p>$65.00</p>
			</div>
		</div>
		<div class="card">
			<div class="placeholder-img earrings">
				<!-- SVG representation of earrings -->
				<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
					<line x1="40" y1="20" x2="40" y2="60" stroke="var(--color-primary)" stroke-width="3"/>
					<line x1="60" y1="20" x2="60" y2="60" stroke="var(--color-primary)" stroke-width="3"/>
					<circle cx="40" cy="65" r="6" fill="var(--color-accent)"/>
					<circle cx="60" cy="65" r="6" fill="var(--color-accent)"/>
				</svg>
			</div>
			<div class="card-info">
				<h3>Drop Pearl Earrings</h3>
				<p>$35.00</p>
			</div>
		</div>
	</div>
</section>

<section class="about-teaser">
	<div class="container teaser-content">
		<h2>The Maker's Story</h2>
		<p>Every piece at Aura is thoughtfully designed and handcrafted in our small studio. We believe in sustainable practices and the beauty of slow fashion. Our materials are ethically sourced, and our designs are meant to be cherished for a lifetime.</p>
		<a href="/about" class="btn btn-secondary">Read More</a>
	</div>
</section>

<style>
	.hero {
		background: linear-gradient(135deg, var(--color-bg) 0%, #EADDDB 100%);
		min-height: 60vh;
		display: flex;
		align-items: center;
		justify-content: center;
		text-align: center;
		padding: 2rem;
	}

	.hero-content h1 {
		font-size: 3.5rem;
		margin-bottom: 1rem;
		color: var(--color-text);
	}

	.hero-content p {
		font-size: 1.2rem;
		max-width: 600px;
		margin: 0 auto 2rem auto;
		color: #5d4a47;
	}

	.featured h2 {
		text-align: center;
		font-size: 2.5rem;
		margin-bottom: 3rem;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
		gap: 2rem;
	}

	.card {
		background: var(--color-white);
		border-radius: 8px;
		overflow: hidden;
		box-shadow: 0 4px 15px rgba(0,0,0,0.05);
		transition: transform 0.3s ease;
	}

	.card:hover {
		transform: translateY(-5px);
	}

	.placeholder-img {
		height: 250px;
		background-color: var(--color-bg);
		display: flex;
		align-items: center;
		justify-content: center;
		border-bottom: 1px solid #eee;
	}
	
	.placeholder-img svg {
		width: 100px;
		height: 100px;
	}

	.card-info {
		padding: 1.5rem;
		text-align: center;
	}

	.card-info h3 {
		font-size: 1.2rem;
		margin-bottom: 0.5rem;
	}

	.about-teaser {
		background-color: var(--color-white);
		text-align: center;
		padding: 6rem 2rem;
	}

	.teaser-content p {
		max-width: 700px;
		margin: 0 auto 2rem auto;
		font-size: 1.1rem;
		line-height: 1.8;
	}
	
	@media (max-width: 768px) {
		.hero-content h1 {
			font-size: 2.5rem;
		}
	}
</style>