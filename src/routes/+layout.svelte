<!-- src/routes/+layout.svelte -->
<script>
  import '../app.css';
  import Sidebar from '$lib/components/Sidebar.svelte';
  import { goto } from '$app/navigation';
</script>

<header>
  <nav class="flex justify-between items-center">
    <a href="/">
      <img class="h-16" src="https://i.imgur.com/BTYJrKC.png" alt="BusinessGPT logo" />
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
