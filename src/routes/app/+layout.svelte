

<script lang="ts">
	import Header from '$lib/sections/Header.svelte';
	import Nav from '$lib/sections/Nav.svelte';

	let { children } = $props();
</script>

<!-- @component
	The layout for the app with header and navigation bar
-->

<div class="flex flex-col items-center justify-center h-full bg-blue">
	
	<Header />
	<main class="flex-1 overflow-y-auto w-full">
		{@render children()}
	</main>

	<Nav />
</div>
