<script lang="ts">
	let { count = 0 }: { count: number } = $props();
</script>

<input type="number" bind:value={count} disabled />

<style>
	input {
		border: 1px solid white;
	}
</style>
