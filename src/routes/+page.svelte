<script>
	import ThemeSwitch from '$lib/theme-switch.svelte';
	('$lib/theme-switch.svelte');
</script>

<div class="bg">
	<h1 class="static">Welcome to SvelteKit</h1>
	<h1 class="themed">Welcome to SvelteKit</h1>
	<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

	<p class="guideline">
		color scale guideline is <a
			href="https://www.radix-ui.com/colors/docs/palette-composition/understanding-the-scale"
			>here</a
		>
	</p>

	<ThemeSwitch></ThemeSwitch>
</div>

<style>
	.themed {
		color: var(--blue-11);
		margin: 0;
	}

	.static {
		color: #0d74ce;
	}

	h1 {
		margin: 0;
	}

	.guideline {
		color: var(--gray-12);
	}
</style>
