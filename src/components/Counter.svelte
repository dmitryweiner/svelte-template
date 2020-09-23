<script>
  let initialCount;
  $: count = initialCount;
  $: double = count * 2;

  function increment() {
    count += 1;
  }

  function decrement() {
    count -= 1;
  }

  export { initialCount };
</script>

<h3>Counter: {count}</h3>
<h3>Double: {double}</h3>
<button on:click={increment}>+</button>
<button on:click={decrement}>-</button>

<style>
 h3 {
   color: gray;
 }
</style>
