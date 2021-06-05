<script>
	export let src;
	export let tags = [];
</script>

<div class="max-w-sm rounded overflow-hidden shadow-lg bg-gray-700 mx-auto">
	<img class="w-full h-56" {src} alt="Sunset in the mountains" />
	<div class="px-6 pt-4">
		{#each tags as item}
			<span class="tag">{item}</span>
		{/each}
	</div>
	<div class="px-6 pb-6">
		<div class="text-white font-semibold text-2xl mb-2">
			<slot name="title">
				<span>Default Title</span>
			</slot>
		</div>
		<div class="text-gray-400 text-base font-medium">
			<slot name="desc">
				<span>Default Desc</span>
			</slot>
		</div>
	</div>
</div>

<style scoped>
	.tag {
		@apply inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-medium text-gray-700 mr-2 mb-2;
	}
</style>
