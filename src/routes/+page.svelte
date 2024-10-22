<script lang="ts">
	import CountInput from '$lib/components/CountInput.svelte';

	let count: number = $state(0);

	function increaseCount() {
		count = count + 1;
	}

	function decreaseCount() {
		count = count - 1;
	}
</script>

<div class="">
	<CountInput {count} />

	<button onclick={() => increaseCount()}>Count</button>
	<button onclick={() => decreaseCount()}>Count down</button>
</div>

<style>
</style>
