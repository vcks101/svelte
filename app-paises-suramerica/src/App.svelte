<script>
  import Paises from "./lib/paises.svelte";
  const lista=["colombia", "venezuela", "ecuador", "peru", "brasil", "argentina", "chile", "uruguay", "paraguay"]
</script>
<div class="main">
  {#each lista as pais}
    <div>
      <Paises {pais}/> 
    </div>
  {:else}
    No existen elementos 
  {/each}
</div>
<svelte:head>
  <title>Paises de suramerica</title>
</svelte:head>
<style>
  .main{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 10px;
    grid-auto-rows: minmax(100px, auto);
  }
</style>