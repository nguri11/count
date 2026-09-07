<script lang="ts">
	let count = $state(0);

	function increment() {
		count += 1;
	}

	function decrement() {
		count -= 1;
	}
</script>

<div class="number-label">{count}</div>
<div class="button-container">
	<button onclick={increment}>+</button>
	<button onclick={decrement}>-</button>
</div>

<style>
	.number-label {
		font-size: 64px;
		text-align: center;
		margin-top: 120px;
	}
	.button-container {
		text-align: center;
	}
	.button-container button {
		width: 100px;
		height: 100px;
		font-size: 64px;
		background-color: white;
		border-radius: 50%;
	}
</style>
