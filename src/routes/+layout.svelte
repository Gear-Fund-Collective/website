<script lang="ts">
	import Heading from '$lib/components/Heading.svelte';
	import NavBar from '$lib/components/NavBar/NavBar.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import '../app.css';

	let { children } = $props();
</script>

<div class="container mx-auto max-w-[666px] p-8">
	<Heading />
	<NavBar />
	{@render children()}
	<Footer />
</div>
