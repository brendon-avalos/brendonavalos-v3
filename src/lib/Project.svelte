<script lang="ts">
	export let title: string;
	export let url: string;
	export let team: string; // can't call something 'with' in JS
	export let description: string;
</script>

<div class="project">
	<div class="{team} title">
		<a target="blank" href={url}>{title}</a>
	</div>
	<div class="project-description">
		{description}
	</div>
</div>

<style lang="postcss">
	.project-description {
		display: inline;
	}

	.project-description:before {
		content: '\2E3A';
		@apply pr-1;
	}

	.underline {
		border-bottom: 1px solid currentColor;
	}

	.section-header {
	}

	.credits-container {
		@apply pt-6;
	}

	.credits-description {
	}

	.credits-header {
		@apply pb-4;
	}

	.credit {
		display: block !important;
		line-height: 1.5 !important;
	}

	.project {
	}

	.title {
		line-height: 100%;
		display: inline;
	}

	.column {
		@apply flex flex-col gap-4;
		flex-grow: 1;
		max-width: 24rem;
	}
</style>
