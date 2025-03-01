<script>
	import Icon from '@iconify/svelte';
</script>

<!-- TODO (Burak) proper styling of this header as a fixed nav at the top of the screen -->

<header class="flex">
	<button class="btn">
		<Icon icon="line-md:chevron-left" />
	</button>

	<div class="text-lg font-bold">Today</div>

	<button class="btn">
		<Icon icon="line-md:chevron-right" />
	</button>
</header>
