<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<!-- @component
	Render a phone container on the devices that are bigger than phone screens  
	The reason for this is because we are designing the app for mobile only.
-->

<div class="sm:mockup-phone sm:shadow-2xl">
	<div class="sm:mockup-phone-camera"></div>
	<div class="sm:mockup-phone-display">
		<div class="w-full h-12 bg-base-300"></div>
		<div class="w-full h-full bg-base-200">
			{@render children()}
		</div>
	</div>
</div>
