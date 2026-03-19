<script>
  let count = $state(0);
  const increment = () => (count += 1);
  const decrement = () => (count -= 1);

  const reset = () => (count = 0);
</script>

<button class="action-btn" onclick={decrement}>Minus</button>
<span class="value">{count}</span>
<button class="action-btn" onclick={increment}>Plus</button>
<button class="action-btn" onclick={reset}>reset</button>

<style>
  .action-btn {
    background-color: rgb(49, 119, 163);
    color: aliceblue;
    border-radius: 12px;
    padding: 12px;
  }

  .action-btn:hover {
    transition-duration: 300ms;
    background-color: rgb(20, 68, 98);
    cursor: pointer;
  }

  .value {
    color: rgb(94, 66, 29);
    font-size: x-large;
  }
</style>
