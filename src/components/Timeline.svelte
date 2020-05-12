<script>
  import Card from "./Card.svelte";
  import Loading from "./Loading.svelte";

  export let posts = [];
</script>

<style>
  .Timeline {
    padding: 4em 0 0 0;
  }
</style>

<div class="Timeline">
  <div class="container">
    {#each posts as post}
      <Card {...post} />
    {:else}
      <Loading />
    {/each}
  </div>
</div>
