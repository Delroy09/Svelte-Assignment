<script>
  let items = $state(["Apple", "Banana", "Mango"]);

  function reverseList() {
    items = [...items].reverse();
  }
</script>

<h3>Fruit List</h3>

<button onclick={reverseList}>Reverse List</button>

<ul>
  {#each items as item}
    <li>{item}</li>
  {/each}
</ul>

<style>
  h3 {
    text-align: center;
    margin-bottom: 0.6rem;
    color: #333;
  }

  button {
    border: 1px solid #4caf50;
    background: #4caf50;
    color: white;
    padding: 0.45rem 0.8rem;
    border-radius: 999px;
    cursor: pointer;
    display: block;
    margin: 0.5rem auto 1rem;
  }

  button:hover {
    opacity: 0.9;
  }

  ul {
    list-style: none;
    padding: 0;
    margin: 0 auto;
    max-width: 300px;
  }

  li {
    padding: 0.5rem 0.7rem;
    border: 1px solid #ccc;
    border-radius: 8px;
    margin-bottom: 0.35rem;
    background: #fff;
  }
</style>
