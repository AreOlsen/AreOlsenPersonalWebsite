<script>
	let date_1 = new Date("03/08/2023");

	const days = (date_1) => {
		let date_2 = new Date();
		let difference = date_2.getTime() - date_1.getTime();
		let TotalDays = Math.ceil(difference / (1000 * 3600 * 24));
		return TotalDays;
	};

	let duoStreak = days(date_1) + 552;
	setInterval(() => {
		duoStreak = days(date_1) + 552;
	}, 1000 * 60 * 60);
</script>

<main class="flex flex-col gap-10">
	<h1 class="font-bold text-5xl">Achievements.</h1>
	<div class="flex flex-row gap-2">
		<div class="flex flex-col gap-4">
			<h1 class="font-bold text-3xl">Personal Achievements</h1>
			<div class="divider" />
			<article class="flex flex-row gap-2">
				<div>
					<h2 class="font-bold text-2xl">Spanish Learning with Duolingo.</h2>
					<p>
						When I first started learning Spanish I have to admit that I hated every bit of it, I didn't
						despite it, but it wasn't the language I favoured. As a result my first grades in the language
						class was not on par with my own standards for grades and studying. At first I started studying
						other languages instead of Spanish, I became familiar in the languages of Russian, Portuegese,
						Romanian, German and Arabic. Which was an experience I am glad I took even though it was just a
						temporary escape from Spanish. Nevertheless, I realised that if I was going to improve in
						spanish I just had to bite the bullet and take a shot at it. Quickly it came to my attention
						that Spanish is one of the most beatuiful languages, as it relies so much on feeling, intuition
						and allows for the personal voice to be shine through the sentence structure. I started using
						Duolingo as my primary learning tool, where I do exactly 10 whole lessons or more a day taking
						about 40-50 minutes, and I have now used it daily for a long long time. I also read spanish
						books and watch spanish entertainment. If I were to speak with a Spanish native we would be able
						to have full on discussions and debates with each other where both of our viewpoints get
						communicated exactly as meant.
					</p>
				</div>
				<div class="stat flex flex-col justify-center items-center">
					<div class="stat-title">DUOLINGO STREAK.</div>
					<div class="stat-value">{duoStreak} days</div>
				</div>
			</article>
		</div>
		<div class="divider lg:divider-horizontal" />
		<div class="flex flex-col gap-4">
			<h1 class="font-bold text-3xl">Olympiads & Others.</h1>
			<div class="divider" />
			<article class="flex flex-row gap-2">
				<div>
					<h2 class="font-bold text-2xl">International Language Olympiad (2022).</h2>
					<p>
						The International Language Olympiad (ILC) is an international competition which focuses on the
						understanding of a particular language, if it is a self-studied foreign language, such as
						Spanish in my case, or your mother's tounge it doesn't really matter as there are many
						categories. I participated and scored the highest at my entire school, leading our team, I
						scored a total of 50 points of the maximum 60. After the competition finished I was informed
						that if it was an individual competition I would have gone to compete on national level as my
						skill was on par with the highest in the entire country. Unfortunately this was a team-based
						competition and our team lacked only a total of 0.2 points to go further. Nevertheless, even
						though I was not able to go to further I was still pleased with my score.
					</p>
				</div>
				<div class="stat flex flex-col justify-center items-center">
					<div class="stat-title">ILC SCORE.</div>
					<div class="stat-value">50/60 total</div>
				</div>
			</article>
			<article class="flex flex-row gap-2">
				<div>
					<h2 class="font-bold text-2xl">Norwegian Informatics Olympiad (2022).</h2>
					<p>
						The Norwegian Informatics Olympiad (NIO) is a national-level competition challenging a persons
						algorithmic thinking and logical thinking. I competed in the year 2022 and will be competing
						once more this year, and the years to come as well. I have always been fascinated by algorithms
						and computers so partaking in this was an obvious experience needed to be felt. Unfortunately,
						when I was partaking I was quite sick and was therefore not nearly at the same level of logical
						thinking which I usually am. Therefore, my score was not the best I could have achieved if I was
						in my best condition. I scored a total 26 points of the required 27 to partake further. Even
						though I got one point less than the required, I am still glad I partaked this year, as you may
						have thought my lack of just one point made me, to put it lightly, furious. I am therefore of
						course practicing and putting myself in the best state mentally and with the best experience I
						can have for the next year. I <i>will</i> get to the national-level.
					</p>
				</div>
				<div class="stat flex flex-col justify-center items-center">
					<div class="stat-title">NIO SCORE.</div>
					<div class="stat-value">26/27 required</div>
				</div>
			</article>
			<article class="flex flex-row gap-2">
				<div>
					<h2 class="font-bold text-2xl">The Abels Competition (2022).</h2>
					<p>
						The Abels Competition is a challening mathematical competition that challenges one's
						mathematical understanding of probabilty-theory, possibility-theory, and just general
						mathematical knowledge. As the NIO was closely timed with the Abels, you may have understood
						that I was also sick on this competition as well. Even though I was sick and not in my best form
						during the competition I still feel that to remain honest to myself and to the readers of this
						page. I have to inform you that I could have performed better, and that being sick was not my
						biggest setback. My biggest setback was in fact my mathematical knowledge. The competition
						included theories, and mathematical fields that I have never encountered before, and have had a
						real use for. Hence I was not fully prepared for the competition. I received a total of 40
						points, where 60 points was the requirement for further participation. One correct question
						equaled 5 points, I was therefore only 4 questions correct away from further participation. The
						competition is known for being incredibly challenging and the need of hard mathematical rigour
						is to be found. Therefore, even though I didn't meet the requirement I was still awarded a
						diploma for having great results. Which actually was signed by the Norwegian Minister of
						Education "Tonje Brenna". Just like with the NIO, I <i>will</i> get to the national-level next year.
						The first time was a fluke, the next time I will reign and get further than I had ever gotten in
						my mathematical understanding.
					</p>
				</div>
				<div class="stat flex flex-col justify-center items-center">
					<div class="stat-title">ABELS SCORE.</div>
					<div class="stat-value">40/60 required</div>
				</div>
			</article>
			<article class="flex flex-row gap-2">
				<div>
					<h2 class="font-bold text-2xl">Others.</h2>
					<p>
						I have also competed in smaller competitions, such as the Norwegian English Literature
						Competition, where one has to write a good fantasy-like text. However, these competitions never
						were so important and I can with my whole heart say that they would not be interesting to any
						reader as well.
					</p>
				</div>
			</article>
		</div>
	</div>
</main>
