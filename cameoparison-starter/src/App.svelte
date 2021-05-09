<script>
    import Welcome from "./screens/Welcome.svelte";
    let state = "welcome"; // "welcome" or "playing"
</script>

<main>
    {#if state === "welcome"}
        <Welcome />
    {:else}
        <p>game screen goes here</p>
    {/if}
</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 800px;
        margin: 0 auto;
    }
</style>
