<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<!-- @component
	Render a phone container on the devices that are bigger than phone screens  
	The reason for this is because we are designing the app for mobile only.
-->

<div class="sm:mockup-phone sm:shadow-2xl font-display">
	<div class="sm:mockup-phone-camera"></div>
	<div class="sm:mockup-phone-display min-h-full flex flex-col ">
		<div class="hidden sm:block w-full h-12 bg-base-300"></div>
		<div class="w-full sm:flex-1 max-sm:h-screen bg-base-200">
			{@render children()}
		</div>
	</div>
</div>

<!-- TODO - FONT değiştir  -->
