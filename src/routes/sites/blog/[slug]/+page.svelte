<!-- src/routes/[slug]/+page.svelte -->
<script>
  export let data;
</script>

<main>
  <article class="w-9/12">
    <h1 class="font-bold text-4xl">{ data.title }</h1>
    <p class="italic text-2xl">Published: {data.date} by Are Olsen.</p> 
    <svelte:component this={data.content} />
  </article>
</main>
