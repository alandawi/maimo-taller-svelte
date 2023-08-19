<script>
    import Header from "$lib/components/Header.svelte";
    import Counter from "$lib/components/Counter.svelte";
    import Hero from "$lib/components/Hero.svelte";
    import Blocks from "$lib/components/Blocks.svelte";
    import "$lib/css/style.css";

    let imgSource = "https://picsum.photos/200/300";
    let isActive = false;
</script>

<Header />

{#if isActive}
     <Counter />
{/if}

<Hero image={imgSource} />

<Blocks />

<style>
    /* h2 {
        background: red !important;
    } */
</style>