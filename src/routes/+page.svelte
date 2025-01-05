<script lang="ts">
  import Paragraph from '../components/Paragraph.svelte'
  import Button from '../components/Button.svelte'

  let name = 'John'
  let imgUrl =
    'https://images.unsplash.com/photo-1735598417949-d22e9f8092ea?q=80&w=2187&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D'
</script>

<h1>Welcome to SvelteKit</h1>
<h2>Hello {name.toUpperCase()}</h2>
<p>
  Visit <a href="https://svelte.dev/docs/kit" target="_blank">svelte.dev</a> to read the documentation
</p>
<p>
  Visit <a href="https://svelte.dev/tutorial/svelte/styling" target="_blank">svelte.dev</a> to read about
  styling
</p>
<p>
  Visit <a href="https://svelte.dev/tutorial/svelte/nested-components" target="_blank">svelte.dev</a
  > to read about nested components
</p>
<Paragraph />
<Button />
<img src={imgUrl} alt="Milky Way Switzerland" />

<style>
  p {
    color: rgb(16, 60, 170);
    font-family: 'Comic Sans MS', cursive;
    font-size: 2em;
  }
  img {
    width: auto;
    height: 500px;
  }
</style>
