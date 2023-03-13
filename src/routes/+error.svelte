<script>
	import { page } from "$app/stores";
</script>

<main class="flex-col gap-4">
	<h1 class="text-5xl font-bold">{$page.status}</h1>
	<h2 class="text-3xl italic">Error code: {$page.error.message}</h2>
	<a class="btn btn-accent normal-case text-xl" href="/">Go To Main Page</a>
</main>
