<script lang="ts">
  let { name, image, color, price } = $props()
</script>

<div>
  <h1>{name}</h1>
  <img src={image} alt={name} />
  <p>color: {color}</p>
  <p>price: {price}</p>
</div>

<style>
  div {
    margin: 20px;
    padding: 2px;
  }
  h1 {
    color: rgb(255, 4, 4);
    font-family: 'Comic Sans MS', cursive;
    font-size: 2em;
  }
  img {
    width: auto;
    height: 300px;
    border-radius: 100px;
    border: 2px solid rgb(30, 36, 34);
  }
  p {
    color: rgb(255, 4, 4);
    font-family: 'Comic Sans MS', cursive;
    font-size: 1.5em;
  }
</style>
