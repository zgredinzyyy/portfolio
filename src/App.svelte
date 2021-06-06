<script>
	import Router from "svelte-spa-router";
	import Home from "./Home.svelte";
	import Projects from "./Projects.svelte";
</script>

<Router
	routes={{
		"/": Home,
		"/projects": Projects,
	}}
/>
