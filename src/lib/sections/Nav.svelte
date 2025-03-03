<script lang="ts">
	import Icon from '@iconify/svelte';

	import { page } from '$app/stores';
	export let title = 'Default Title';
	export let href = '/app/today';

	let navItems = [
		{
			icon: 'solar:sun-linear',
			tooltip: 'Home',
			link: '/app/today'
		},
		{
			icon: 'charm:chart-line',
			tooltip: 'Analysis',
			link: '/app/analysis'
		},
		{
			icon: 'mdi:folder-open-outline',
			tooltip: 'Database',
			link: '/app/database'
		},
		{
			icon: 'mdi:menu',
			tooltip: 'Menu',
			link: '/app/menu'
		}
	];
</script>

<!-- TODO (Burak) proper styling of this nav bar as a fixed nav at the bottom of the screen -->

<nav class="flex bg-base-300 w-full py-3 items-center justify-center gap-3 rounded-t-3xl">
	{#each navItems as { icon, tooltip, link }}
		<a
			href={link}
			class="btn rounded-2xl transition-all duration-200
		{$page.url.pathname.includes(link) ? 'bg-white text-red-500 shadow-lg' : ''}"
		>
			<Icon {icon} />
		</a>
	{/each}
</nav>
