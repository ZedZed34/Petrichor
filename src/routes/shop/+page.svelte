<svelte:head>
	<title>Shop | Aura Handcrafted</title>
</svelte:head>

<section class="container page-header">
	<h1>Our Collection</h1>
	<p>Explore our carefully curated selection of handcrafted pieces. Each item is unique and made to order.</p>
</section>

<section class="container">
	<div class="grid">
		<!-- Item 1 -->
		<div class="card">
			<div class="placeholder-img">
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

		<!-- Item 2 -->
		<div class="card">
			<div class="placeholder-img">
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

		<!-- Item 3 -->
		<div class="card">
			<div class="placeholder-img">
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

		<!-- Item 4 -->
		<div class="card">
			<div class="placeholder-img">
				<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
					<rect x="35" y="35" width="30" height="30" rx="5" stroke="var(--color-primary)" stroke-width="4" fill="none"/>
					<circle cx="50" cy="50" r="5" fill="var(--color-accent)"/>
				</svg>
			</div>
			<div class="card-info">
				<h3>Geometric Studs</h3>
				<p>$28.00</p>
			</div>
		</div>

		<!-- Item 5 -->
		<div class="card">
			<div class="placeholder-img">
				<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M30,30 L70,30 L50,70 Z" stroke="var(--color-primary)" stroke-width="4" fill="none"/>
				</svg>
			</div>
			<div class="card-info">
				<h3>Triangle Pendant</h3>
				<p>$50.00</p>
			</div>
		</div>

		<!-- Item 6 -->
		<div class="card">
			<div class="placeholder-img">
				<svg viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
					<ellipse cx="50" cy="50" rx="40" ry="25" stroke="var(--color-primary)" stroke-width="4" fill="none"/>
					<circle cx="50" cy="50" r="10" fill="var(--color-accent)"/>
				</svg>
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

	.placeholder-img {
		height: 280px;
		background-color: var(--color-bg);
		display: flex;
		align-items: center;
		justify-content: center;
		border-bottom: 1px solid #eee;
	}
	
	.placeholder-img svg {
		width: 120px;
		height: 120px;
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