<script>
	import Card from '../../components/Card.svelte';
	import { projects } from '../../data/data';
</script>

<section
	class="bg-gray-100 min-h-screen"
	style="background-image: url('assets/bg.png'); background-size: contain;"
>
	<article class="prose-base lg:prose-xl max-w-7xl mx-auto p-4 text-justify text-gray-900">
		<h2 class="text-orange-700">Projects</h2>
		<p class="">Projects will be one of the most important activities of the Center.</p>
		<p>
			Experts from the Center and Industry will come out with challenging problem statements which
			will be assigned to the students of RVCE.
		</p>
		<p>Each project will have a team of students, one Faculty guide and a project mentor.</p>
		<p>
			As on now,about 6 projects have been assigned to different teams and they have already started
			the literature survey.
		</p>
		<p>
			There will be frequent interaction sessions with students, project guide and the mentor to
			assess the progress of the project work.
		</p>
		<p>
			Projects are related to developing A<strong
				>I and ML based algorithms to analyse and extract content</strong
			>
			in an intelligent manner from live video surveillance camera feeds.
		</p>
		{#each projects as i}
			<div class="py-3">
				<Card Title={i.Title} Description={i.Description} Link={i.Link} />
			</div>
		{/each}
	</article>
</section>
<!-- <iframe src="assets/projects/wildanimal.pdf"  title="Animals" class="w-[50%] h-[75%]"></iframe> -->
