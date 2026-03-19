<script>
  let { name = "Student" } = $props();

  let show = $state(true);

  function toggleMessage() {
    show = !show;
  }
</script>

<div class="card">
  <h2>Message Toggle Demo</h2>

  {#if show}
    <p>Hello, <strong>{name}</strong> 👋</p>
  {:else}
    <p>Hope you're having a great day 🌟</p>
  {/if}

  <button onclick={toggleMessage}> Change Message </button>
</div>

<style>
  .card {
    border: 1px solid #ccc;
    padding: 1.5rem;
    border-radius: 8px;
    background-color: #fff3cd;
    max-width: 20rem;
    text-align: center;
  }

  h2 {
    margin-top: 0;
    color: #856404;
  }

  button {
    margin-top: 1rem;
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 5px;
    background-color: #ffc107;
    cursor: pointer;
  }

  button:hover {
    background-color: #e0a800;
  }
</style>
