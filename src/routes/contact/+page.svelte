<svelte:head>
	<title>Contact | Aura Handcrafted</title>
</svelte:head>

<section class="container page-header">
	<h1>Get in Touch</h1>
	<p>Have a question about a piece, or want to inquire about custom orders? We'd love to hear from you.</p>
</section>

<section class="container contact-section">
	<div class="contact-wrapper">
		<div class="contact-info">
			<h2>Our Studio</h2>
			<p><strong>Email:</strong> hello@aurahandcrafted.com</p>
			<p><strong>Hours:</strong> Mon - Fri, 9am - 5pm</p>
			<div class="socials">
				<p>Follow our journey on social media:</p>
				<a href="https://instagram.com" target="_blank" rel="noopener noreferrer">Instagram</a> | <a href="https://pinterest.com" target="_blank" rel="noopener noreferrer">Pinterest</a>
			</div>
		</div>

		<form class="contact-form">
			<div class="form-group">
				<label for="name">Name</label>
				<input type="text" id="name" name="name" required placeholder="Jane Doe">
			</div>
			
			<div class="form-group">
				<label for="email">Email</label>
				<input type="email" id="email" name="email" required placeholder="jane@example.com">
			</div>
			
			<div class="form-group">
				<label for="message">Message</label>
				<textarea id="message" name="message" rows="5" required placeholder="How can we help you?"></textarea>
			</div>
			
			<button type="button" class="btn">Send Message</button>
		</form>
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

	.contact-section {
		padding-bottom: 6rem;
	}

	.contact-wrapper {
		display: grid;
		grid-template-columns: 1fr 1.5fr;
		gap: 4rem;
		background: var(--color-white);
		padding: 3rem;
		border-radius: 12px;
		box-shadow: 0 10px 40px rgba(0,0,0,0.05);
	}

	.contact-info h2 {
		font-size: 2rem;
		margin-bottom: 1.5rem;
		color: var(--color-accent);
	}

	.contact-info p {
		margin-bottom: 1rem;
		color: #5d4a47;
	}

	.socials {
		margin-top: 2rem;
		padding-top: 2rem;
		border-top: 1px solid #EADDDB;
	}

	.socials a {
		font-weight: bold;
	}

	.contact-form {
		display: flex;
		flex-direction: column;
		gap: 1.5rem;
	}

	.form-group {
		display: flex;
		flex-direction: column;
		gap: 0.5rem;
	}

	label {
		font-weight: 600;
		color: var(--color-text);
		font-size: 0.95rem;
	}

	input, textarea {
		width: 100%;
		padding: 1rem;
		border: 1px solid #EADDDB;
		border-radius: 6px;
		background-color: var(--color-bg);
		font-family: var(--font-body);
		font-size: 1rem;
		color: var(--color-text);
		transition: border-color 0.3s ease;
	}

	input:focus, textarea:focus {
		outline: none;
		border-color: var(--color-accent);
	}

	.btn {
		align-self: flex-start;
		margin-top: 1rem;
	}

	@media (max-width: 768px) {
		.contact-wrapper {
			grid-template-columns: 1fr;
			padding: 2rem;
			gap: 3rem;
		}
	}
</style>