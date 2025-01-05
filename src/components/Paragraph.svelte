<script>
  let s = `this string contains some <strong>HTML!!!</strong>`
</script>

<p>This is a paragraph.</p>
<p>{@html s}</p>

<style>
  p {
    color: rgb(19, 180, 116);
    font-family: 'Comic Sans MS', cursive;
    font-size: 1.5em;
  }
</style>
