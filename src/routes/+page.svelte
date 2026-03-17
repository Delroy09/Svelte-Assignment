<script>
  import Counter from "$lib/components/Counter.svelte";
  import Hello from "$lib/components/Hello.svelte";
  import Todo from "$lib/components/Todo.svelte";
</script>

<h1>Delroy's Home!</h1>
<p>Welcome, Human</p>

<main>
  <Hello name="Sir" />
  <Counter />
  <Todo />
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
