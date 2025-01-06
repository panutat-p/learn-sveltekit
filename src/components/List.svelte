<script lang="ts">
  let numbers = $state([1, 2, 3, 4])

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
</div>

<style>
  div {
    margin: 20px;
    padding: 2px;
  }
  button {
    background-color: rgb(38, 28, 184);
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 1.5em;
    cursor: pointer;
  }
</style>
