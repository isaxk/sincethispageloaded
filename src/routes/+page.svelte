<script lang="ts">
	import Counter from "$lib/components/Counter.svelte";

	import { counters } from "$lib/counters";
</script>

<h1>Since this page was loaded...</h1>

<div class="counters">
	{#each counters as data}
		<Counter {data} />
	{/each}
</div>

<style>
	.counters {
		display: grid;
		grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
	}
</style>
