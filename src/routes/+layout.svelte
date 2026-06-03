<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<header>
	<div class="header-container">
		<a href="/" class="logo">Aura Handcrafted</a>
		<nav>
			<a href="/">Home</a>
			<a href="/shop">Shop</a>
			<a href="/about">About</a>
			<a href="/contact">Contact</a>
		</nav>
	</div>
</header>

<main>
	{@render children()}
</main>

<footer>
	<p>&copy; {new Date().getFullYear()} Aura Handcrafted Jewelry. All rights reserved.</p>
</footer>

<style>
	header {
		background-color: var(--color-bg);
		border-bottom: 1px solid var(--color-primary);
		padding: 1.5rem 0;
		position: sticky;
		top: 0;
		z-index: 100;
	}

	.header-container {
		max-width: 1200px;
		margin: 0 auto;
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 0 2rem;
	}

	.logo {
		font-family: var(--font-heading);
		font-size: 1.8rem;
		font-weight: 600;
		color: var(--color-text);
		text-decoration: none;
		letter-spacing: 0.05em;
	}

	nav {
		display: flex;
		gap: 2rem;
	}

	nav a {
		text-decoration: none;
		color: var(--color-text);
		font-weight: 500;
		font-size: 1.05rem;
		transition: color 0.3s ease;
	}

	nav a:hover {
		color: var(--color-accent);
	}

	main {
		min-height: calc(100vh - 80px - 100px); /* Approx calc for header and footer */
	}

	footer {
		background-color: var(--color-primary);
		color: var(--color-bg);
		text-align: center;
		padding: 2rem;
		margin-top: 4rem;
	}
	
	footer p {
		margin: 0;
		opacity: 0.9;
	}
	
	@media (max-width: 768px) {
		.header-container {
			flex-direction: column;
			gap: 1rem;
		}
	}
</style>