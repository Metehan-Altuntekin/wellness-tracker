<script lang="ts">
	import Icon from '@iconify/svelte';

	import { page } from '$app/state';

	let navItems = [
		{
			icon: 'solar:sun-linear',
			tooltip: 'Home',
			link: '/app'
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

<nav class="flex bg-base-300 w-full py-3 items-center justify-center gap-3 rounded-t-3xl">
	{#each navItems as { icon, tooltip, link }}
		<a
			href={link}
			class="btn btn-square btn-lg rounded-2xl transition-all duration-200
						{page.url.pathname === link ? 'bg-white text-red-500 shadow-lg' : ''}"
		>
			<Icon {icon} class="w-6 h-6" />
		</a>
	{/each}
</nav>
