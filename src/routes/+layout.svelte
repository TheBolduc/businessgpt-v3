<!-- src/routes/+layout.svelte -->
<script>
	import '../app.css';
	import Sidebar from '$lib/components/Sidebar.svelte';
</script>

<div class="flex flex-col items-center max-w-2xl mx-auto">
	<Sidebar />
	<main class="w-full">
		<slot />
	</main>
</div>

<style>
	/* Add styles for the layout container */
</style>
