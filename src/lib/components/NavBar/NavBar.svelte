<script>
	import Link from '../Link.svelte';

	const links = [
		{ name: 'Request', href: '/request' },
		{ name: 'Donate', href: '/donate' },
		{ name: 'Gear Library', href: '/library' }
	];
</script>

<nav class="mt-4 mb-8 flex justify-center">
	<ul class="flex list-none flex-row gap-4">
		{#each links as link}
			<li>
				<Link href={link.href}>{link.name}</Link>
			</li>
		{/each}
	</ul>
</nav>
