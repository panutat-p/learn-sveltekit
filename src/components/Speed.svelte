<script>
  let n = $state(0)
  let interval = $state(1000)

  $effect(() => {
    const id = setInterval(() => {
      n += 1
    }, interval)

    return () => {
      clearInterval(id)
    }
  })
</script>

<div>
  <button onclick={() => (interval /= 2)}>speed up</button>
  <button onclick={() => (interval *= 2)}>slow down</button>

  <p>elapsed: {n}</p>
</div>

<style>
  div {
    margin: 20px;
    padding: 2px;
  }
  button {
    background-color: rgb(216, 98, 19);
    color: white;
    border: none;
    padding: 10px 20px;
    font-size: 1.5em;
    cursor: pointer;
  }
  p {
    color: rgb(216, 98, 19);
    font-family: 'Comic Sans MS', cursive;
    font-size: 1.5em;
  }
</style>
