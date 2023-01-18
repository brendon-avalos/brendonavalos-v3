<script>
	import '../styles/app.css';
</script>

<main>
	<slot />
</main>

<style lang="postcss">
	:global(:root) {
		--font-body: 'IBM Plex Serif', serif;
		--color-bg-1: #ffffff;
		--color-text: rgba(0, 0, 0, 1);
	}

	:global(body) {
		min-height: 100vh;
		margin: 0;
		background-attachment: fixed;
		background-color: var(--color-bg-1);
		background-size: 100vw 100vh;
		font-family: var(--font-body);
		color: var(--color-text);
		font-size: 14px;
		line-height: 1.4;
	}
	.app {
		@apply flex justify-start flex-col;
		min-height: 100vh;
	}

	main {
		@apply flex flex-nowrap content-start;
		flex: 1;
		padding: 1rem;
		width: 100%;
		box-sizing: border-box;
	}
</style>
