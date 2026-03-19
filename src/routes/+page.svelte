<script>
  import Counter from "$lib/components/Counter.svelte";
  import Hello from "$lib/components/Hello.svelte";
  import Todo from "$lib/components/Todo.svelte";
  import Toggle from "$lib/components/Toggle.svelte";
</script>

<h1>Delroy's Home!</h1>
<p>Welcome, Human</p>

<main>
  <Hello name="Sir" />
  <Counter />

  <br />
  <br />
  <Todo />

  <br />
  <br />
  <Toggle name="Test" />
</main>

<style>
  * {
    font-family:
      system-ui,
      -apple-system,
      BlinkMacSystemFont,
      "Segoe UI",
      Roboto,
      Oxygen,
      Ubuntu,
      Cantarell,
      "Open Sans",
      "Helvetica Neue",
      sans-serif;
  }
</style>
