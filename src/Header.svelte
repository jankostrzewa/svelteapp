<script>
  import Button from "./Button.svelte";

  export let props;
</script>

<style>
  header {
    margin: 0;
    padding: 0;
    height: 100%;
    background-color: #eee;
    display: grid;
    grid-auto-flow: column;
  }
</style>

<header>
  {#each props as item}
    <Button label={item.label} url={item.url} />
  {/each}
</header>
