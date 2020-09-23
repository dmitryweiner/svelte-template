<script>
  let initialCount = 42;

  function apply() {
      initialCountChange(initialCount);
  }

  export let initialCountChange;
</script>

<h3>Enter initial count:</h3>
<input bind:value={initialCount} type="number" />
<button on:click={apply}>Apply</button>

<style>
 h3 {
   color: darkgray;
 }
</style>
