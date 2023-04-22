<!-- src/lib/components/Sidebar.svelte -->
<script>
  import {goto} from '$app/navigation';

  function navigateToHomePage() {
    goto('/');
  }
</script>

<aside class="...">
  <button on:click={navigateToHomePage} class="...">
    Go to Home
  </button>
  <!-- Add more navigation items if needed -->
</aside>

<style>
  /* Add styles for the sidebar */
</style>
