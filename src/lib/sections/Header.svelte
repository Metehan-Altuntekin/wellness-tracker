<script>
	import Icon from '@iconify/svelte';
</script>

<header class="flex w-full px-3 justify-between items-center py-2 rounded-b-3xl bg-base-300">
	<button class="btn btn-square btn-lg rounded-2xl">
		<Icon icon="line-md:chevron-left" class="w-6 h-6" />
	</button>

	<div class="text-xl font-black">Today</div>

	<button class="btn btn-square btn-lg rounded-2xl">
		<Icon icon="line-md:chevron-right" class="w-6 h-6" />
	</button>
</header>
