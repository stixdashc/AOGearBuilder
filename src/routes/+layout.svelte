<script>
	import Header from '../lib/components/Header.svelte';
	import './styles.css';
	import '../app.css';
	import Analytics from '$lib/utils/Analytics.svelte';
</script>

<div class="app bg-zinc-800">
	<Analytics />
	<Header />

	<main>
		<slot />
	</main>
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
</style>
