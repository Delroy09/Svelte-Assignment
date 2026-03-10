<script>
  let { name = "Student" } = $props();
</script>

<div class="card">
  <h2>Svelte Framework Demo</h2>
  <p>Hello, <strong>{name}</strong>! This is a simple reusable component.</p>
</div>

<style>
  .card {
    border: 1px solid #ccc;
    padding: 1.5rem;
    border-radius: 8px;
    background-color: #f8f9fa;
    margin-bottom: 1rem;
  }
  h2 {
    margin-top: 0;
    color: #ff3e00;
  }
</style>
