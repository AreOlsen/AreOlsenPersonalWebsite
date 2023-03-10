<script>
	let subject = "";
	let content = "";
	$: emailUrl = `mailto:are_olsen@hotmail.no?subject=${subject}&body=${content}`;
</script>

<main class="flex flex-row gap-8">
	<div class="flex flex-col gap-4">
		<h1 class="font-bold text-2xl">Let's chat!</h1>
		<h2 class="font-bold text-3xl">Tell me about your ideas.</h2>
		<h3 class="font-bold text-xl">Let's build something revolutionary together.</h3>
		<div class="">
			<ul class="flex flex-col gap-3">
				<li>
					<span class="font-bold">email:</span>
					<a href="mailto:are_olsen@hotmail.no?subject=Dear Mr. Olsen." class="link link-hover"
						>are_olsen@hotmail.no</a
					>
				</li>
				<li>
					<span class="font-bold">discord:</span>
					<a href="https://discord.gg/9snq8SfpZ9" class="link link-hover">That guy#6103</a>
				</li>
			</ul>
		</div>
	</div>
	<div class="rounded-lg shadow-2xl gap-2 p-8 flex flex-col bg-accent">
		<h2 class="text-3xl font-bold">Send me an email!</h2>
		<label for="Subject">Subject of matter:</label>
		<input
			class="input input-bordered input-secondary"
			type="text"
			name="Subject"
			id="Subject"
			bind:value={subject}
		/>
		<label for="Email">Contents of Email:</label>
		<textarea
			class="textarea textarea-bordered textarea-secondary"
			style="width:400px; height:300px;
                	max-height: 550px;
                	min-height:200px;"
			type="text"
			name="Email"
			id="Email"
			bind:value={content}
		/>
		<a href={emailUrl} class="btn btn-secondary">Send Email!</a>
	</div>
</main>
