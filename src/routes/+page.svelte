<script>
	import Project from '../lib/Project.svelte';

	let projects = [
		{
			title: 'Post Malone',
			url: 'https://www.postmalone.com/',
			description: "A website promoting Posty's new album 12 Carat Toothache.",
			with: 'alright'
		},

		{
			title: 'Counter Situations',
			url: 'https://counter-situations.netlify.app/',
			description: 'A funky web archive with a focus on exploring different realities.',
			with: ''
		},

		{
			title: 'Trippin',
			url: 'https://trippin.world/',
			description:
				'Website for an independent platform that connects travel, culture and creativity.',
			with: 'alright'
		},

		{
			title: 'Noom',
			url: 'https://brand.noom.com/',
			description: 'A brand hub that for the Noom team.',
			with: 'alright'
		},

		{
			title: 'Saint James',
			url: 'https://saintjamesicedtea.com/',
			description: 'A website for a brand new tea company.',
			with: 'alright'
		},

		{
			title: 'Manhattan Hydraulics',
			url: 'https://www.hydraulics.nyc/',
			description: 'Getting a new product design studio off the ground.',
			with: 'sanctuary'
		},

		{
			title: 'Studio Carbon Negative',
			url: 'https://negative.sanctuary.computer/',
			description: `A website to celebrate our studio's commitment to carbon neutrality.`,
			with: 'sanctuary'
		},
		{
			title: 'A. Savage',
			url: 'https://a-savage.com/',
			description: 'A simple website for the portfolio of a New York based artist.',
			with: ''
		},

		{
			title: 'Seaborne',
			url: 'https://www.seaborne.nyc/',
			description: 'Branding and website for a sustainability company.',
			with: 'sanctuary'
		},

		{
			title: 'New Grove',
			url: 'https://newgroveconcepts.com/',
			description: 'A personal portfolio for a talented woodworker in Kingston, New York.',
			with: ''
		},
		{
			title: 'Spillt',
			url: 'https://apps.apple.com/us/app/spillt-social-recipes/id1583973507',
			description: 'Product audit and UI kit for a recipe sharing app.',
			with: 'alright'
		},
		{
			title: 'Car Thing',
			url: 'https://www.theverge.com/2022/7/27/23280357/spotify-stops-manufacturing-car-thing-q2-2022-earnings',
			description: `Branding and art direction for Spotify's first hardware product.`,
			with: 'thisalso'
		},
		{
			title: 'Nike SNKRS Pass',
			url: 'https://www.nike.com/launch/t/inside-snkrs-updates-to-snkrs-pass',
			description: 'Product design for a Nike SNKRS reservation feature.',
			with: 'thisalso'
		},
		{
			title: 'OOO',
			url: 'https://techcrunch.com/2017/02/06/ooo-is-a-camera-toy-that-lets-you-play-with-zoom-make-mini-music-videos/?guccounter=1&guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAADby1LFxfudUBp5a5wb4IM0_5B-rUQcS7BW1SNAUvePK56T6LOF4Vwe5zLKZWF-4306A0m0sRInsnQYvIPRkAoq3NVdRAj_cSCpfEBIKSUawtDnCW7dJ7i55H2c_53JOygWQO591ncPlK0QHv3sJfGL7hKohQyacUbDokRiznM3K',
			description:
				'Branding and product design for an app that makes let you make crazy zoom videos.',
			with: 'thisalso'
		},
		{
			title: 'Sprayscape',
			url: 'https://experiments.withgoogle.com/sprayscape',
			description: `Product design for a Google experiment that let's you create and send 3D collages with your phone.`,
			with: 'thisalso'
		}
	];
</script>

<svelte:head>
	<title>brendon avalos</title>
	<meta name="description" content="A designer based in Los Angeles." />
</svelte:head>

<section>
	<div class="column">
		<div class="title"><a href="/">brendon avalos</a></div>

		<div>
			Hello and welcome to my small corner of the internet. I'm a designer and strategic thinker who
			enjoys collaborating, learning and laughing with other humans (live, laugh, love...if you feel
			me). I'm currently living in Los Angeles and clicking away at <span class="no-icon fictive"
				><a target="blank" href="https://fictivekin.com/">Fictive Kin</a></span
			>. Before that, I had the pleasure of starting a product design studio from the ground up at
			<span class="no-icon sanctuary"
				><a target="blank" href="https://www.sanctuary.computer/">Sanctuary Computer</a></span
			>. Before that, I helped large companies make digital products. I've also made music with my
			friends in
			<a target="blank" href="https://bboys.bandcamp.com/">B Boys</a> and
			<a target="blank" href="https://flexi.bandcamp.com/album/nothing">Flexi</a>, as well as a solo
			record as
			<a target="blank" href="https://giftwrap.bandcamp.com/album/losing-count">Gift Wrap</a>.
		</div>
		<div class="mail title">
			<a href="mailto:avalos.brendon@gmail.com">avalos.brendon@gmail.com</a>
		</div>

		<div class="credits-container">
			<div class="credits-header"><span class="custom-underline">Credits</span></div>

			<div class="credits-description">
				<div class=" credit sanctuary title ">
					with <a target="blank" href="https://www.garden3d.net/">Garden3d</a>
				</div>
				<div class="credit alright title  ">
					with <a target="blank" href="https://alright.studio/">Alright Studios</a>
				</div>
				<div class="credit thisalso title  ">
					with <a
						target="blank"
						href="https://www.bizjournals.com/portland/news/2019/03/21/portland-agency-instrument-expands-to-brooklyn.html"
						>This Also</a
					>
				</div>
			</div>
		</div>
	</div>

	<div class="column">
		<div class="section-header"><span class="custom-underline">Projects</span></div>
		{#each projects as project}
			<Project
				title={project.title}
				url={project.url}
				team={project.with}
				description={project.description}
			/>
		{/each}
	</div>
</section>

<style lang="postcss">
	section {
		@apply flex gap-6 flex-col md:flex-row content-start;
	}

	.custom-underline {
		border-bottom: 1px solid currentColor;
		height: 0px;
	}

	.credits-container {
		@apply pt-1;
	}

	.credits-header {
		@apply pb-4;
	}

	.credit {
		display: block !important;
		line-height: 1.5 !important;
	}

	.title {
		display: inline;
	}

	.column {
		@apply flex flex-col gap-4;
		flex-grow: 1;
		max-width: 20rem;
	}
</style>
