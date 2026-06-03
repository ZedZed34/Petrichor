<script>
	import sample4 from '$lib/assets/Sample4.jpg';
</script>

<svelte:head>
	<title>About | Petrichor</title>
</svelte:head>

<section class="container page-header">
	<h1>About the Maker</h1>
</section>

<section class="container about-content">
	<div class="about-grid">
		<div class="about-image">
			<img src={sample4} alt="About Petrichor" class="about-img" />
		</div>
		<div class="about-text">
			<h2>Crafting with Intention</h2>
			<p>
				Petrichor was born out of a passion for creating wearable
				art that empowers and inspires. Every piece of jewelry is
				meticulously hand-forged, polished, and finished in our cozy
				studio.
			</p>

			<p>
				We source our materials ethically, ensuring that our metals and
				stones have minimal impact on the earth. The "rose tan"
				aesthetic reflects our commitment to natural, earthy warmth and
				timeless elegance.
			</p>

			<p>
				Our goal is to create heirloom-quality pieces that you can wear
				every day. Thank you for supporting independent artisans and
				slow fashion.
			</p>

			<a href="/shop" class="btn">View Collection</a>
		</div>
	</div>
</section>

<style>
	.page-header {
		text-align: center;
		padding: 4rem 2rem 2rem 2rem;
	}

	.page-header h1 {
		font-size: 3rem;
		margin-bottom: 1rem;
	}

	.about-content {
		padding-bottom: 6rem;
	}

	.about-grid {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 4rem;
		align-items: center;
	}

	.about-image {
		width: 100%;
		border-radius: 10px;
		overflow: hidden;
		box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
	}

	.about-img {
		width: 100%;
		height: 100%;
		object-fit: cover;
		display: block;
	}

	.about-text h2 {
		font-size: 2rem;
		margin-bottom: 1.5rem;
		color: var(--color-accent);
	}

	.about-text p {
		font-size: 1.1rem;
		margin-bottom: 1.5rem;
		color: #5d4a47;
		line-height: 1.8;
	}

	.btn {
		margin-top: 1rem;
	}

	@media (max-width: 768px) {
		.about-grid {
			grid-template-columns: 1fr;
			gap: 2rem;
		}
	}
</style>
