<script>
  let count = $state(0);

  function increment() {
    count += 1;
  }
</script>

<div>
  <button onclick={increment}>
    Clicked {count}
  </button>
</div>

<style>
  div {
    margin: 20px;
    padding: 2px;
  }
  button {
    background-color: rgb(19, 180, 116);
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 1.5em;
    cursor: pointer;
  }
</style>
