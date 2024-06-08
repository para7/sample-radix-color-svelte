<script lang="ts">
	const onClick = () => {
		if (document.documentElement.classList.contains('dark')) {
			document.documentElement.classList.remove('dark');
			localStorage.setItem('theme', 'light');
		} else {
			document.documentElement.classList.add('dark');
			localStorage.setItem('theme', 'dark');
		}
	};
</script>

<button class="button" onclick={onClick}> change theme! </button>

<style>
	button {
		background-color: var(--blue-9);
		color: var(--gray-12);
		padding: 0.5em;
		font-size: 1.2rem;
	}

	.dark > button {
		background-color: var(--red-9);
		color: var(--gray-12);
	}
</style>
