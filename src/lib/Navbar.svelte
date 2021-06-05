<script>
	import { link } from "svelte-spa-router";
</script>

<header class="relative">
	<div class="bg-gray-900 pt-6">
		<nav
			class="relative max-w-xl mx-auto flex items-center justify-center px-4 sm:px-6"
		>
			<div class="flex items-center">
				<a href="/">
					<h2 class="header-text text-white text-3xl font-semibold">
						zinzy.dev
					</h2>
				</a>
				<div class="hidden space-x-8 md:flex md:ml-10">
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
