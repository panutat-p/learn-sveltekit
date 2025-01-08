<script lang="ts">
  let { title } = $props()

  let s = `this string contains some <strong>HTML!!!</strong>`
</script>

<h1>{title}</h1>
<p>This is a paragraph.</p>
<p>{@html s}</p>

<style>
  h1 {
    color: rgb(19, 180, 116);
    font-family: 'Comic Sans MS', cursive;
    font-size: 2em;
  }
  p {
    color: rgb(19, 180, 116);
    font-family: 'Comic Sans MS', cursive;
    font-size: 1.5em;
  }
</style>
