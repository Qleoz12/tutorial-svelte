<script>
	let count = 0
	function increment() {
		count += 1
	}
</script>

<svelte:options customElement="svelte-counter"  />
<button on:click={increment}>
	Clicks: {count}
</button>

<style>
	button {
		font-family: inherit;
		font-size: inherit;
		padding: 1em 2em;
		color: #ff3e00;
		background-color: rgb(255 62 0 / 0.1);
		border-radius: 2em;
		border: 2px solid rgb(255 62 0 / 0);
		outline: none;
		width: 200px;
		font-variant-numeric: tabular-nums;
		cursor: pointer;
	}

	button:focus {
		border: 2px solid #ff3e00;
	}

	button:active {
		background-color: rgb(255 62 0 / 0.2);
	}
</style>