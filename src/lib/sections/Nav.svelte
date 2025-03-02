<script lang="ts">
	import Icon from '@iconify/svelte';
</script>

<!-- TODO (Burak) proper styling of this nav bar as a fixed nav at the bottom of the screen -->

<nav class="flex bg-red-500 w-full py-3 items-center justify-center gap-3 rounded-t-3xl">
	<button class="btn">
		<Icon icon="solar:sun-linear" />
	</button>
	<button class="btn">
		<Icon icon="charm:chart-line" />
	</button>
	<button class="btn">
		<Icon icon="mdi:folder-open-outline" />
	</button>
	<button class="btn">
		<Icon icon="mdi:menu" />
	</button>
</nav>
