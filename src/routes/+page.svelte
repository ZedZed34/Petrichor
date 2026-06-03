<script>
	import sample1 from '$lib/assets/Sample1.jpg';
	import sample2 from '$lib/assets/Sample2.jpg';
	import sample3 from '$lib/assets/Sample3.jpg';
</script>

<svelte:head>
	<title>Petrichor | Beautiful Artisan Jewelry</title>
</svelte:head>

<section class="hero">
	<div class="hero-content">
		<h1>Elegance in Every Detail</h1>
		<p>Discover unique, handmade jewelry designed to highlight your natural style.</p>
		<a href="/shop" class="btn">Shop the Collection</a>
	</div>
</section>

<section class="featured container">
	<h2>Featured Pieces</h2>
	<div class="grid">
		<div class="card">
			<div class="card-img-container">
				<img src={sample1} alt="Rose Quartz Ring" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Rose Quartz Ring</h3>
				<p>$45.00</p>
			</div>
		</div>
		<div class="card">
			<div class="card-img-container">
				<img src={sample2} alt="Delicate Gold Chain" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Delicate Gold Chain</h3>
				<p>$65.00</p>
			</div>
		</div>
		<div class="card">
			<div class="card-img-container">
				<img src={sample3} alt="Drop Pearl Earrings" class="card-img" />
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
		<p>Every piece at Petrichor is thoughtfully designed and handcrafted in our small studio. We believe in sustainable practices and the beauty of slow fashion. Our materials are ethically sourced, and our designs are meant to be cherished for a lifetime.</p>
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

	.card-img-container {
		height: 250px;
		width: 100%;
		overflow: hidden;
		border-bottom: 1px solid #eee;
	}
	
	.card-img {
		width: 100%;
		height: 100%;
		object-fit: cover;
		transition: transform 0.5s ease;
	}

	.card:hover .card-img {
		transform: scale(1.05);
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