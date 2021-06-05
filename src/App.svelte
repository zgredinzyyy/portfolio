<script>
	import Router from "svelte-spa-router";
	import Navbar from "./lib/Navbar.svelte";
	import Home from "./Home.svelte";
	import Projects from "./Projects.svelte";
	import Footer from "./lib/Footer.svelte";
</script>

<div class="flex flex-col h-screen">
	<Navbar />
	<Router
		routes={{
			"/": Home,
			"/projects": Projects,
		}}
	/>
	<Footer />
</div>
