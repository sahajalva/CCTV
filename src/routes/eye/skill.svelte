<script>
	import CardKnowMore from '../../components/Card_know_more.svelte';
	import Card_know_more from '../../components/Card_know_more.svelte';
	import { skills } from '../../data/data';
</script>

<section
	class="bg-gray-100 min-h-screen"
	style="background-image: url('assets/bg.png'); background-size: contain;"
>
	<article class="prose-base lg:prose-xl max-w-7xl mx-auto p-4 text-justify text-gray-900">
		<h2 class="text-orange-700">Skill Development Programmes</h2>
		<p>
			The country is witnessing huge number of video surveillance installations coming up and there
			is a great need for trained manpower in this field.
		</p>
		<div class=" flex flex-nowrap space-x-2">
			{#each skills as s }
			<Card_know_more
			Title={s.Title}
			Description={s.Description}
			Link={s.Link}
			know_more_link={s.know_more_link}
			/>
			{/each}
			
			
		</div>
		<p>CCTV system integrators are not able to train them and put them on the field.</p>
		<p>
			Hence this activity will be taken up by the center by way of conducting skill development
			programmes providing hands on training in the domain of CCTV surveillance. Essentially,the
			programme comprises of two modules which are briefly explained below.
		</p>

		<img
			src="/assets/photos/Skill Development/sd10.jpeg"
			alt=""
			class="w-[50%] h-auto rounded-md mx-auto"
		/>
		<p class="text-center font-bold ">
			Session 1 of Skill development programme: CCTV installation and maintainence
		</p>
		<img
			src="/assets/photos/Skill Development/sd9.jpeg"
			alt=""
			class="w-[50%] h-[50%] rounded-md mx-auto"
		/>
		<p class="text-center font-bold ">
			Session 2 of Skill development programme: CCTV installation and maintainence
		</p>
	</article>
</section>
