<script>
	import './styles.css';
	import { base } from '$app/paths';
</script>

<div class="app bg-gray-300">
	<header>
		<div class="flex-col">
			<a href="{base}/">home</a>
			<a href="{base}/contact">contact</a>
			<a href="{base}/about">about</a>
		</div>
	</header>
	<main>
		<slot />
	</main>

	<footer>
		<p>Radau Test</p>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 12px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
