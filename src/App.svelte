<script>
	let hallo='Test';

	function click(){
		alert('ahllo');
		hallo='bla';
	}
</script>

<main>
	<h1>Meine erste App mit Svelte</h1>
	<p>Dies ist ein {hallo} <button on:click={click}>Ändern!</button></p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
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