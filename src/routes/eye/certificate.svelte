<script>
	import Card from '../../components/Card.svelte';
	import { certificates } from '../../data/data'
</script>

<section
	class="bg-gray-100 min-h-screen"
	style="background-image: url('assets/bg.png'); background-size: contain;"
>
	<article class="prose-base lg:prose-xl max-w-7xl mx-auto p-4 text-justify text-gray-900">
		<h2 class="text-orange-700">Certification Courses</h2>
		<p>
			The center had organized a 5 day certification course on "An overview of Video Surveillance
			systems" from 30th August to 3rd Sept 2021.
		</p>
		<div class=" flex flex-nowrap space-x-2">
			{#each certificates as c}
				<Card 
				Title={c.Title}
				Description = {c.Description}
				Link = {c.Link}
				/>
			{/each}
		</div>
		<!-- <p>The program schedule is given below.</p> -->
		<!-- <a href="http://ccctvr.org/tentative_schedule_5day_course.pdf" class="text-blue-800 no-underline hover:underline">
			<h4>Tentative schedule of the 5 days course.</h4>
		</a> -->
	</article>
</section>
