<script lang="ts">
	import Header from "$lib/components/Header.svelte";
    import "$lib/css/app.css"
</script>


<Header />

<main>
    <slot />
</main>

<style>
    main {
        max-width: 1000px;
        margin: auto;
        padding: 50px 20px 0px 20px;
    }
</style>