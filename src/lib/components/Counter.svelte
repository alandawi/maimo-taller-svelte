<script>
	let count = 0;

    $: doble = count * 2;

	function handleClick() {
		count += 1;
	}
</script>

<button on:click={handleClick}>
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
</button>

<h2>{doble}</h2>