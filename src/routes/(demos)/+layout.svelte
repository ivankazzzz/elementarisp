<script lang="ts">
  import { name } from '$root/package.json'
  import { DemoNav } from '$site'
</script>

<h1>
  <img src="favicon.svg" alt={name} height="50" width="50" />&ensp;Examples
</h1>

<DemoNav />

<main>
  <slot />
</main>

<style>
  h1 {
    text-align: center;
    display: flex;
    place-content: center;
    place-items: center;
  }
  main :global(h2) {
    text-align: center;
  }
</style>
