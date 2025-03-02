<script>
	import Icon from '@iconify/svelte';
</script>

<!-- TODO (Burak) proper styling of this header as a fixed nav at the top of the screen -->

<header class="flex w-full px-3 justify-between items-center py-2 rounded-b-3xl bg-base-300">
	<button class="btn rounded-2xl">
		<Icon icon="line-md:chevron-left" />
	</button>

	<div class="text-xl font-bold">Today</div>

	<button class="btn rounded-2xl">
		<Icon icon="line-md:chevron-right" />
	</button>
</header>
