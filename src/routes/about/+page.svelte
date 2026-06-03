<svelte:head>
	<title>About | Aura Handcrafted</title>
</svelte:head>

<section class="container page-header">
	<h1>About the Maker</h1>
</section>

<section class="container about-content">
	<div class="about-grid">
		<div class="about-image">
			<svg
				viewBox="0 0 400 500"
				fill="none"
				xmlns="http://www.w3.org/2000/svg"
			>
				<rect width="400" height="500" fill="#EADDDB" rx="10" />
				<circle
					cx="200"
					cy="250"
					r="100"
					stroke="var(--color-primary)"
					stroke-width="4"
				/>
				<path
					d="M150,300 Q200,350 250,300"
					stroke="var(--color-accent)"
					stroke-width="4"
					fill="none"
				/>
			</svg>
		</div>
		<div class="about-text">
			<h2>Crafting with Intention</h2>
			<p>
				Aura Handcrafted was born out of a passion for creating wearable
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
sdfsadfasdf

<!-- dfsfsadfsdaf -->

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

	.about-image svg {
		width: 100%;
		height: auto;
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
ddasdfasdfasdf