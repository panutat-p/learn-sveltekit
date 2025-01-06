<script lang="ts">
  let numbers = $state([1, 2])
  let total = $derived(numbers.reduce((t, n) => t + n, 0))

  function addNumber() {
    numbers.push(numbers.length + 1)
  }
</script>

<div>
  <button onclick={addNumber}> Add a number </button>

  <ul>
    {#each numbers as number}
      <li>{number}</li>
    {/each}
  </ul>
  <p>Total: {total}</p>
</div>

<style>
  div {
    margin: 20px;
    padding: 2px;
  }
  p {
    color: rgb(27, 50, 180);
    font-family: 'Comic Sans MS', cursive;
    font-size: 1.5em;
  }
  button {
    background-color: rgb(27, 50, 180);
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 1.5em;
    cursor: pointer;
  }
</style>
