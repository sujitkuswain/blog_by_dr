<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
	import Navbar from '$lib/Navbar.svelte';
	import Footer from '$lib/Footer.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="flex min-h-screen flex-col">
	<Navbar />

	<main class="max-w-7xl flex-1 justify-start px-16 py-8">
		{@render children?.()}
	</main>

	<Footer />
</div>
