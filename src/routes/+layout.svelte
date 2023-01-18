<script>
	import '../styles/app.css';
</script>

<slot />



<style>
	.app {
		
		@apply flex justify-start flex-col ;
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
		min-width:min-content;
		max-width: 24rem;
		
	}

	

		



	
</style>
