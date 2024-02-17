<script lang="ts">
	import { onMount } from "svelte";

	export let data: {
		text: string;
		increment: number;
		interval: number;
		css: string;
		icon: string;
	};

    let count:number = 0;

    onMount(()=>{
        window.setInterval(()=>count+=data.increment,data.interval)
    })
</script>


<div class="counter" style={data.css}>
    <div class="left">
        <span class="material-symbols-outlined">
            {data.icon}
        </span>
    </div>
    <div class="right">
        <div class="count">{count.toLocaleString('en-US', {maximumFractionDigits:0})}</div>
        <div class="text">{data.text}</div>
    </div>
</div>

<style>
    .counter {
        display: grid;
        grid-template-columns: 0.1fr 1fr;
        align-items: center;
        gap: 10px;
        padding: 20px;
    }
    .count {
        font-family: var(--monospace-font-family);
        font-size: 20px;
    }
</style>