<script lang="ts">
  import Paragraph from '../components/Paragraph.svelte'
  import Button from '../components/Button.svelte'
  import List from '../components/List.svelte'
  import Speed from '../components/Speed.svelte'
  import Fruit from '../components/Fruit.svelte'

  const apple = {
    name: '🍎 Apple',
    image:
      'https://images.unsplash.com/photo-1619546813926-a78fa6372cd2?fm=jpg&q=60&w=3000&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTZ8fHJlZCUyMGFwcGxlc3xlbnwwfHwwfHx8MA%3D%3D',
    color: 'red',
    price: 50.25
  }
</script>

<h1>Welcome to SvelteKit</h1>
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
<Paragraph title="🤖 Robot" />
<Button />
<List />
<Speed />
<Fruit {...apple} />

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
