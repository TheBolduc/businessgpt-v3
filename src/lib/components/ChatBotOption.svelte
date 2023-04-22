<!-- src/lib/components/ChatBotOption.svelte -->
<script>
  export let name = "";
  export let onSelect = () => {};
</script>

<button on:click={onSelect} class="...">
  {name}
</button>

<style>
  /* Add styles for the ChatBotOption button */
</style>
