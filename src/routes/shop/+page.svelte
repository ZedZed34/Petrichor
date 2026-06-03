<script>
	import sample1 from '$lib/assets/Sample1.jpg';
	import sample2 from '$lib/assets/Sample2.jpg';
	import sample3 from '$lib/assets/Sample3.jpg';
	import sample4 from '$lib/assets/Sample4.jpg';
	import sample5 from '$lib/assets/Sample5.png';
	import sample6 from '$lib/assets/Sample6.png';
</script>

<svelte:head>
	<title>Shop | Petrichor</title>
</svelte:head>

<section class="container page-header">
	<h1>Our Collection</h1>
	<p>Explore our carefully curated selection of handcrafted pieces. Each item is unique and made to order.</p>
</section>

<section class="container">
	<div class="grid">
		<!-- Item 1 -->
		<div class="card">
			<div class="card-img-container">
				<img src={sample1} alt="Rose Quartz Ring" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Rose Quartz Ring</h3>
				<p>$45.00</p>
			</div>
		</div>

		<!-- Item 2 -->
		<div class="card">
			<div class="card-img-container">
				<img src={sample2} alt="Delicate Gold Chain" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Delicate Gold Chain</h3>
				<p>$65.00</p>
			</div>
		</div>

		<!-- Item 3 -->
		<div class="card">
			<div class="card-img-container">
				<img src={sample3} alt="Drop Pearl Earrings" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Drop Pearl Earrings</h3>
				<p>$35.00</p>
			</div>
		</div>

		<!-- Item 4 -->
		<div class="card">
			<div class="card-img-container">
				<img src={sample4} alt="Geometric Studs" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Geometric Studs</h3>
				<p>$28.00</p>
			</div>
		</div>

		<!-- Item 5 -->
		<div class="card">
			<div class="card-img-container">
				<img src={sample5} alt="Triangle Pendant" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Triangle Pendant</h3>
				<p>$50.00</p>
			</div>
		</div>

		<!-- Item 6 -->
		<div class="card">
			<div class="card-img-container">
				<img src={sample6} alt="Halo Bracelet" class="card-img" />
			</div>
			<div class="card-info">
				<h3>Halo Bracelet</h3>
				<p>$85.00</p>
			</div>
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

	.page-header p {
		font-size: 1.1rem;
		color: #5d4a47;
		max-width: 600px;
		margin: 0 auto;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
		gap: 2.5rem;
		padding-bottom: 4rem;
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
		height: 280px;
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
		font-size: 1.3rem;
		margin-bottom: 0.5rem;
	}

	.card-info p {
		font-weight: 700;
		color: var(--color-accent);
		margin-bottom: 0;
	}
</style>