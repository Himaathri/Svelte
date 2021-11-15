<script>
	let name="excuseme";
	let Hello="Hi ";
	let sufix="Everyone";
	const clicked = () => {
		Hello='Bye ';
		};
	const handleInput = (e) =>{
		sufix=e.target.value;
	}
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>This is my first program.</p>
	<p class="p1">{Hello}{sufix}</p>
	<button on:click={clicked}>Click to change</button><br>
	<input type="text" on:input={handleInput} value ={sufix}>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #e41717;
		text-transform: none;
		font-size: 4em;
		font-weight: 100;
	}

	 .p1{
		color: #9917e4;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>