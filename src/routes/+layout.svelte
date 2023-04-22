<!-- src/routes/+layout.svelte -->
<script>
	import '../app.css';
	import Sidebar from '$lib/components/Sidebar.svelte';
	import { goto } from '$app/navigation';
</script>

<header>
  <nav class="flex justify-between items-center">
    <a href="/">
      <blockquote class="imgur-embed-pub" lang="en" data-id="a/XEapHJE" data-context="false"><a href="//imgur.com/a/XEapHJE"></a></blockquote><script async src="//s.imgur.com/min/embed.js" charset="utf-8"></script>
    </a>
    <button class="btn" on:click={() => goto('/')}>Go Home</button>
  </nav>
</header>

<div class="flex flex-col items-center max-w-2xl mx-auto">
	<Sidebar />
	<main class="w-full">
		<slot />
	</main>
</div>

<style>
	/* Add styles for the layout container */
</style>
