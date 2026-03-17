<script>
  /** @typedef {{ id: number, text: string }} Todo */

  /** @type {string} */
  let newTodo = $state("");
  /** @type {Todo[]} */
  let todos = $state([]);

  function add() {
    const text = newTodo.trim();
    if (!text) return;
    todos = [...todos, { id: Date.now(), text }];
    newTodo = "";
  }

  /**
   * @param {number} id
   */
  function remove(id) {
    todos = todos.filter((t) => t.id !== id);
  }

  /**
   * @param {{ key: string; }} e
   */
  function onKey(e) {
    if (e.key === "Enter") add();
  }
</script>

<form
  onsubmit={(e) => {
    e.preventDefault();
    add();
  }}
>
  <input placeholder="Add todo..." bind:value={newTodo} onkeydown={onKey} />
  <button type="submit">Add</button>
</form>

{#if todos.length === 0}
  <p>No todos yet.</p>
{:else}
  <ul>
    {#each todos as todo (todo.id)}
      <li>
        {todo.text}
        <button onclick={() => remove(todo.id)}>✕</button>
      </li>
    {/each}
  </ul>
{/if}
