<script>
  let count = 0;
  const increment = () => (count += 1);
  const decrement = () => (count -= 1);

  const reset = () => (count = 0);
</script>

<div class="counter">
  <button class="action-btn" onclick={increment}>Plus</button>
  <span class="value">{count}</span>
  <button class="action-btn" onclick={decrement}>Minus</button>
</div>

<style>
  .action-btn {
    background-color: rgb(49, 119, 163);
    color: aliceblue;
    border-radius: 12px;
    padding: 12px;
  }
  :hover {
    cursor: pointer;
  }

  .value {
    color: rgb(94, 66, 29);
    font-size: x-large;
  }
</style>
