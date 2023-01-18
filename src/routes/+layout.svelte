<script>
	import '../styles/app.css';
</script>

<slot />

<style lang="postcss">
	:global(:root) {
		--font-body: 'IBM Plex Serif', serif;
		--color-bg-1: #ffffff;
		--color-theme-1: #9092a9;
		--color-theme-2: #4075a6;
		--color-text: rgba(0, 0, 0, 1);
		--column-width: 42rem;
		--column-margin-top: 4rem;
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

	.column {
		@apply flex flex-col gap-4;
		flex-grow: 0;
		min-width: min-content;
		max-width: 24rem;
	}
</style>
