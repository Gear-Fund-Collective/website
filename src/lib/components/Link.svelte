<script>
	export let href = '';
	export let target = '';
	export let rel = '';
	export let title = '';
	export let className = '';
	export let id = '';
	export let style = '';
	export let ariaLabel = '';
</script>

<a
	{href}
	{target}
	{rel}
	{title}
	class={`${className} underline underline-offset-2 transition-all hover:underline-offset-4`}
	{id}
	{style}
	aria-label={ariaLabel}
>
	<slot />
</a>
