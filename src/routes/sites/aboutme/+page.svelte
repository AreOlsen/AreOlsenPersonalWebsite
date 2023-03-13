<script>
	let computerBooks = [
		{
			title: "Code 1 (Kode 1)",
			authors: ["Solheim, E.", "Vågeskar, E.", "Olav L., G.", "Bae, B., P.", "Rostamzadeh, H."],
			releaseYear: 2021,
			pageCount: 369,
			topics: [
				"HTML",
				"CSS",
				"Javascript",
				"Svelte & Sveltekit",
				"Social Networks",
				"Universal Design",
				"Computers, Datatypes & Networking",
				"Lists & Datastructures",
				"Algorithms",
				"Cybersecurity & Computer law",
			],
			read: true,
		},
	];
	let mathBooks = [
		{
			title: "Patterns - Mathematics R1 (Mønster Matematikk R1)",
			authors: ["Kalvø, T.", "Christian L. O., J.", "Skrindo, K.", "Johannes W., Ø."],
			releaseYear: 2021,
			pageCount: 405,
			topics: ["Exponents & Logarithms", "Functions", "Derivation", "Function Analysis", "Vectors"],
			read: true,
		},
		{
			title: "Mathematics In Practice (Matematikk I Praksis)",
			authors: ["Gulliksen, T.", "Hashemi M., A.", "Hole, A."],
			releaseYear: 2022,
			pageCount: 473,
			topics: [
				"General Mathematics",
				"Functions",
				"Periodic Phenomena",
				"Continuity & Limits",
				"Exponential functions, Logarithms & Models",
				"Derivation",
				"Integrals",
				"Complex Numbers",
				"Differential Equations",
				"Linear Algebra",
				"Differential Equation Systems",
				"Multivariable Calculus",
			],
			read: false,
		},
	];

	let allBooks = [
		{
			setTitle: "Computer Science",
			books: computerBooks,
		},
		{
			setTitle: "Mathematics",
			books: mathBooks,
		},
	];
</script>

<main class="flex flex-col gap-4">
	<h1 class="text-5xl font-bold">About Me.</h1>
	<div class="grid-cols-3 grid grid-rows-1 gap-6">
		<div class="col-start-1 col-end-3 flex flex-col gap-2">
			<h1 class="font-bold text-4xl">Well, who am I?</h1>
			<p>
				Greetings, my name is <i>Are Olsen</i>, and I am an 18-year-old from Western Norway with a deep passion
				for logical academic fields such as physics, mathematics, biology, and computer science. I find these
				subjects to be particularly interesting because they allow me to explore the fundamental principles that
				govern the world we live in. I believe that understanding these principles is essential to solving many
				of the world's most pressing problems. In my studies of computer science, I have developed a proficiency
				in multiple programming languages, including Python, C#, HTML & CSS & Javascript & Svelte, and C++. This
				proficiency has allowed me to create various programs and projects, from simple algorithms to complex
				systems. One example of a project I have created is this website, which I made using Sveltekit,
				TailwindCSS & daisyUI. I enjoy the challenge of designing systems and finding elegant solutions to
				complex problems. I am particularly fascinated by the field of artificial intelligence and the potential
				it has to revolutionize the way we interact with technology. Beyond computer science, I am also
				interested in exploring related fields, such as machine learning and data science. These fields have the
				potential to unlock new insights and solutions to some of society's most significant challenges. I am
				eager to continue learning and expanding my knowledge in these areas. In addition to my studies, I enjoy
				reading books and articles on topics related to logical fields, as well as participating in online
				forums and communities. I find that engaging with other learners and experts in these fields allows me
				to deepen my understanding and gain new perspectives. If I continue with in the pace and with the grades
				I am maintaining now, I am estimated to have an equivalent exiting status of that a of
				<i>summa cum laude</i>. When I am not immersed in my studies or reading, I enjoy spending time outdoors,
				hiking and exploring the natural beauty of Western Norway. I find that this helps me maintain a healthy
				balance between my academic pursuits and personal life.
			</p>
		</div>
		<div class="mockup-code flex flex-col gap-2 text-info-content">
			<pre data-prefix="$"><code>Hey, I am Are!</code></pre>
			<pre data-prefix=">"><code>I am 18 and from Western Norway.</code></pre>
			<pre data-prefix=">"><code>I love programming and my academics!</code></pre>
			<pre data-prefix=">"><code>Interested in compsci, physics, mathematics...</code></pre>
			<pre data-prefix=">"><code>Experienced developer in:</code></pre>
			<pre data-prefix=">"><code>C#, Python, C++, Svelte & More.</code></pre>
			<pre data-prefix=">"><code>I love to spend my time creating projects & studying.</code></pre>
		</div>
	</div>

	<div class="divider" />
	<div class="flex flex-col gap-4">
		<div class="flex flex-col gap-2">
			<h2 class="text-4xl font-bold">My studies and study books:</h2>
			<div class="flex flex-row gap-4 pr-6">
				<p>
					As a dedicated student, I am constantly seeking opportunities to learn and grow. I believe that
					reading is one of the most effective ways to broaden one's perspective and increase knowledge.
					That's why I make reading a priority in my daily routine. Whether it's a few pages before bed or a
					chapter during my lunch break, I try to make time for reading every day. Despite not being a fan of
					reading in my younger years, I've grown to appreciate the immense benefits that come with it.
					Reading has not only expanded my vocabulary and improved my comprehension skills, but it has also
					helped me to develop a deeper understanding of complex topics. I find myself drawn to mathematical
					and logical books, as they provide a structured and logical approach to problem-solving that aligns
					with my academic interests. That being said, I'm also an avid fan of historical fiction books. I
					love immersing myself in different eras and cultures and getting a glimpse of what life was like in
					the past. I appreciate authors who put in the effort to research and present accurate historical
					details in their work. Incorporating reading into my daily study schedule has been a game-changer
					for me. By setting aside dedicated time for reading, I'm able to focus more deeply and absorb
					information more effectively. I've found that this has helped me to retain information better and
					has led to a more profound understanding of the topics I'm studying. Because of my strong
					understanding of complex mathematical, physics, biology and computer science topics, I've become a
					go-to resource for my peers and teachers alike. I'm always willing to help others with their studies
					and offer my insights and perspective to help them better understand difficult concepts. Whether
					it's a fellow student, for example an IB student, who's struggling in a particular class or a
					teacher who's looking for a fresh perspective, I'm always happy to lend a hand. My passion for
					learning has led me to become a well-rounded student who excels in both academic and social
					settings.
				</p>
				<img src="/highMarks.svg" alt="I get high grades." width="150px" />
			</div>
		</div>
		<div class="divider" />
		<div class="flex flex-col gap-7">
			<h3 class="font-bold text-3xl">Study Books I Use For Self Studying.</h3>
			<div class="flex flex-row gap-3">
				{#each allBooks as bookSet, z}
					<div>
						<h4 class="text-3xl font-bold">{bookSet.setTitle}</h4>
						<ul class="flex flex-col gap-2">
							{#each bookSet.books as book, i}
								<div class="divider" />
								<li>
									<article class="flex flex-col gap-1">
										<h5 class="font-bold text-xl">
											{book.title} ({book.releaseYear} - {book.pageCount}p)
										</h5>
										<h6 class="font-bold">{book.authors.join(" - ")}</h6>
										{#if book.read}<span class="italic text-success">Studied.</span>{:else}<span
												class="text-warning">To Be Studied.</span
											>{/if}
										<div>
											<h6 class="font-bold">Topics</h6>
											<span class="italic">{book.topics.join(" - ")}</span>
										</div>
									</article>
								</li>
							{/each}
						</ul>
					</div>
					<div class="divider divider-horizontal" />
				{/each}
			</div>
		</div>
	</div>
</main>
