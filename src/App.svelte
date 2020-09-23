<script>
  import Counter from './components/Counter.svelte';
  import Input from './components/Input.svelte';
  let initialCount = 42;
  function initialCountChange(newValue) {
      initialCount = newValue;
  }
</script>

<main>
  <Input initialCountChange={initialCountChange}/>
  <Counter initialCount={initialCount} />
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
