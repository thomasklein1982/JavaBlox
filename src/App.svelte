<script>
	import { Button, Checkbox,Icon,Textfield } from 'svelte-mui';
	import lzstring from 'lz-string';
	import localforage from 'localforage';
	let hallo='Test';

	function click(){
		alert('ahlohh');
		hallo='blubba';
		
	}
</script>

<main>
	
	<h1>Meine erst App mit Svelte</h1>
	<p>Dies ist ein {hallo} <Button color="primary" outlined on:click={click}>Ändern!</Button></p>
	<Textfield label="Gib was ein!" bind:value={hallo}></Textfield>
	<Button color="accent" outlined on:click={click}>
		<!-- left icon -->
		<Icon path="M2.01 21L23 12 2.01 3 2 10l15 2-15 2z" style="margin: 0 0px 0 8px;" />
    Add
</Button>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 250px;
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