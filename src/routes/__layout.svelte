<script>
	import '../app.css';
	// import Sidenav from '../components/sidenav2.svelte';
	import Nav from '../components/nav.svelte';
	import Footer from '../components/Footer.svelte'
</script>


<!-- <div class="flex">
	<div class="w-72"><Sidenav /></div>

	<main class="flex-col">
		<div class="max-w-6xl"> -->
<Nav />
<div class="py-16"></div>
<slot />
<Footer />

<!-- </div>
	</main>
</div> -->
