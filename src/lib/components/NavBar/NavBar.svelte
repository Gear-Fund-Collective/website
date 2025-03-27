<script>
	import Link from '../Link.svelte';

	const links = [
		{ name: 'About', href: '/' },
		{ name: 'Request', href: '/request' },
		{ name: 'Donate', href: '/donate' },
		{ name: 'Gear Library', href: '/library' },
		{ name: 'Instagram', href: 'https://www.instagram.com/thegearfundcollective' }
	];
</script>

<nav class="mt-4 mb-8 flex justify-center">
	<ul class="grid list-none grid-cols-3 justify-items-center gap-4 md:grid-cols-5">
		{#each links as link}
			<li>
				<Link href={link.href}>{link.name}</Link>
			</li>
		{/each}
	</ul>
</nav>
