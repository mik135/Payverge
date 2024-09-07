<script>
    import Countdown from "$lib/Countdown.svelte";
    import Loading from "$lib/Loading.svelte";
    let data = $state("notGotten")

   setTimeout(() => {
    data = "gotten"
   }, 4000)
  
</script>

{#if data != "gotten"}
    <Loading />
{:else}
    <Countdown />
{/if}








