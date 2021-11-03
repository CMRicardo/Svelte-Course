<script>
	export let initialCounter = 0
	let counter = initialCounter

	const handleClick = () => {
		counter += 1
	}
</script>

<main>
	<h1>Times {counter}!!!</h1>
	
	<button on:click={handleClick}>Increment</button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: crimson;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>