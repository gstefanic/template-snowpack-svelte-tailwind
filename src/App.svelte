<script>
  import { onMount } from 'svelte';
  let count = 0;
  onMount(() => {
    const interval = setInterval(() => count++, 1000);
    return () => {
      clearInterval(interval);
    };
  });
</script>

<style>
  
</style>

<div class="bg-gray-100">
  Hello World, {count}
</div>
