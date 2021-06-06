<script>
	import { link } from "svelte-spa-router";
</script>

<header class="relative">
	<div class="bg-gray-900 pt-6">
		<nav class="relative max-w-xl mx-auto flex justify-center">
			<div class="flex items-center flex-col md:flex-row">
				<a href="/">
					<h2 class="header-text text-white text-3xl font-semibold">
						zinzy.dev
					</h2>
				</a>
				<div class="mt-3 md:mt-0 space-x-8 md:flex md:ml-10">
					<a href="/" class="text">🏠 Home</a>
					<a href="/projects" class="text" use:link>🌠 Projects</a>
				</div>
			</div>
		</nav>
	</div>
</header>

<style>
	.text {
		@apply text-base font-medium text-white hover:text-gray-300;
	}
</style>
