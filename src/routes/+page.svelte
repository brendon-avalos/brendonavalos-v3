
<svelte:head>
	<title>Brendon Avalos</title>
	<meta name="description" content="A designer based in Los Angeles." />
</svelte:head>

<section>
	<div class="column">
		<div class="title"><a href="/">brendon avalos</a></div>
		
		<div>
			I'm a digital designer based in Los Angeles. I'm currently a designer at <a target="blank" href="https://fictivekin.com/">Fictive Kin</a>. Before that, I had the pleasure of starting a product design studio from the ground up at <a target="blank" href="https://www.sanctuary.computer/">Sanctuary Computer</a>. And even before that, I helped large companies make digital products.
		</div>
		<div class="mail title">
			<a href="mailto:avalos.brendon@gmail.com">avalos.brendon@gmail.com</a>
			</div>

			<div class="credits-container">
				<div class="credits-header"> <span class="underline">Credits</span></div>
			
				<div class="credits-description">
					<div class=" credit sanctuary title "><a target="blank" href="https://www.garden3d.net/">with garden3d</a></div>
					<div class="credit alright title  "><a target="blank" href="https://www.alright.studios/">with alright studios</a></div>
					<div class="credit thisalso title  "><a target="blank" href="https://www.bizjournals.com/portland/news/2019/03/21/portland-agency-instrument-expands-to-brooklyn.html">with this also</a></div>
					</div>
					</div>

					

			
	</div>

	

<div class ="column">
	<div class="section-header"> <span class="underline">Projects</span></div>

	<div class="project">
		<div class="sanctuary title"><a target="blank" href="https://www.hydraulics.nyc/">Manhattan Hydraulics</a></div>
		<div class="project-description">Getting a new product design studio off the ground.</div>
		</div>


		<div class="project">
			<div class="alright title"><a target="blank" href="https://trippin.world/">Trippin</a></div>
			<div class="project-description">Website for an independent platform that connects travel, culture and creativity.</div>
			</div>

	<div class="project">
	<div class="sanctuary title"><a target="blank" href="https://negative.sanctuary.computer/">Studio Carbon Negative</a></div>
	<div class="project-description">A website to celebrate our studio's commitement to carbon neutrality.</div>
	</div>

	<div class="project">
		<div class="title"><a target="blank" href="https://a-savage.com/">A. Savage</a></div>
		<div class="project-description">A simple website for the portfolio of a New York based artist.</div>
		</div>

	<div class="project">
		<div class="title"><a target="blank" href="https://counter-situations.netlify.app/">Counter Situations</a></div>
		<div class="project-description">A funky web archive with a focus on recontextualizing our current way of living.</div>
	</div>

	<div class="project">
		<div class="sanctuary title"><a target="blank" href="https://www.seaborne.nyc/">Seaborne</a></div>
		<div class="project-description">Branding and website for a sustainability company.</div>
	</div>

	

	<div class="project">
		<div class="alright title"><a target="blank" href="https://apps.apple.com/us/app/spillt-social-recipes/id1583973507">Spillt</a></div>
		<div class="project-description">Product audit and UI kit for a recipe sharing app.</div>
	</div>

	<div class="project">
		<div class="thisalso title"><a target="blank" href="https://www.theverge.com/2022/7/27/23280357/spotify-stops-manufacturing-car-thing-q2-2022-earnings">Car Thing</a></div>
		<div class="project-description">Branding and art direction for Spotify's first hardware product.</div>
		</div>

	<div class="project">
		<div class="thisalso title"><a target="blank" href="https://www.nike.com/launch/t/inside-snkrs-updates-to-snkrs-pass">Nike SNKRS Pass</a></div>
		<div class="project-description">Product design for a Nike SNKRS reservation feature.</div>
	</div>

	<div class="project">
		<div class="thisalso title"><a target="blank" href="https://techcrunch.com/2017/02/06/ooo-is-a-camera-toy-that-lets-you-play-with-zoom-make-mini-music-videos/?guccounter=1&guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAADby1LFxfudUBp5a5wb4IM0_5B-rUQcS7BW1SNAUvePK56T6LOF4Vwe5zLKZWF-4306A0m0sRInsnQYvIPRkAoq3NVdRAj_cSCpfEBIKSUawtDnCW7dJ7i55H2c_53JOygWQO591ncPlK0QHv3sJfGL7hKohQyacUbDokRiznM3K">OOO</a></div>
		<div class="project-description">Branding and product design for an app that makes let you make crazy zoom videos.</div>
	</div>

	<div class="project">
		<div class="thisalso title"><a target="blank" href="https://experiments.withgoogle.com/sprayscape">Sprayscape</a></div>
		<div class="project-description">Product design for a Google experiment that let's you create and send 3D collages with your phone.</div>
	</div>

	

		
</div>


	

	


</section>

<style lang = "postcss">


	section {
	@apply flex gap-6 flex-col md:flex-row content-start;
	}
	
	.project-description{
		display: inline;
	}

	.project-description:before{
		content: '\2E3A';
		@apply pr-1;
	}
	
	.underline {
  border-bottom: 1px solid currentColor;
}

	.section-header {
	
	}

	.credits-container{
		@apply pt-6;
	}

	.credits-description{
	}

	.credits-header{
		@apply pb-4;
	}

	.credit {
		display: block !important;
		line-height: 1.5 !important;
	}

	.project{
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

	.title :before {
	@apply pr-1; /* Add a little space between text and arrow */
	content: '\273A'; 
	}

	.alright :before {

	content: '\273B'; /* Unicode hex for &raquo; */}

	.sanctuary :before {

	content: '\271E'; /* Unicode hex for &raquo; */}

	.thisalso :before {
	content: '\2750'; /* Unicode hex for &raquo; */}

	.mail :before {
	content: '\27AA'; /* Unicode hex for &raquo; */}




</style>
