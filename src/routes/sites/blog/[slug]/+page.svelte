<script>
	export let data;
</script>

<main>
	<article class="w-9/12 flex flex-col justify-center items-center gap-3">
		<h1 class="font-bold text-5xl">{data.title}</h1>
		<p class="italic text-2xl">Published on "{data.date}" by Are Olsen.</p>
		<div class="divider" />
		<div class="prose">
			<svelte:component this={data.content} />
		</div>
	</article>
</main>
