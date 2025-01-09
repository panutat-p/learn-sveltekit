<script>
  import { counter } from '../lib/counter.svelte'
</script>

<div>
  <button onclick={() => (counter.value += 1)}>
    clicks: {counter.value}
  </button>
  <button onclick={() => (counter.value += 1)}>
    clicks: {counter.value}
  </button>
  <button onclick={() => (counter.value += 1)}>
    clicks: {counter.value}
  </button>
</div>

<style>
  div {
    margin: 20px;
    padding: 2px;
  }
  button {
    background-color: rgb(0, 251, 255);
    color: rgb(31, 31, 31);
    border: none;
    border-radius: 30px;
    padding: 10px 20px;
    font-size: 1.5em;
    cursor: pointer;
  }
</style>
