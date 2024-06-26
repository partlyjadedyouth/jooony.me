<script>
	/**
	 * [/about/+page.svelte]
	 * This component renders the About page, displaying personal information, contact details,
	 * education background, work experience, awards, and proficiency in languages and tools.
	 */

	import email from '$lib/images/email.svg';
	import browser from '$lib/images/browser.png';
	import LinkContainer from '$lib/components/LinkContainer.svelte';
</script>

<svelte:head>
	<title>about</title>
	<meta name="description" content="Joonyoung's Blog" />
</svelte:head>

<section class="pt-20">
	<!-- Name -->
	<div class="flex">
		<h1 class="font-biryani text-2xl font-semibold mr-2">Joonyoung Park</h1>
		<LinkContainer type="pdf" url="/pdfs/cv.pdf" />
	</div>
	<!-- Email -->
	<div class="flex items-center">
		<a href="mailto:jooony@snu.ac.kr" target="_blank" rel="noopener noreferrer">
			<img alt="email" src={email} class="w-5 mr-1 pt-1" />
		</a>
		<a href="mailto:jooony@snu.ac.kr" target="_blank" rel="noopener noreferrer">
			<p class="font-ibm hover:font-medium hover:underline">jooony@snu.ac.kr</p>
		</a>
	</div>
	<!-- Website -->
	<div class="flex items-center">
		<a href="https://joonyoung.dev" target="_blank" rel="noopener noreferrer">
			<img
				alt="Browser icons created by kmg design - Flaticon"
				src={browser}
				class="w-5 mr-1 pt-1"
			/>
		</a>
		<a href="https://joonyoung.dev" target="_blank" rel="noopener noreferrer">
			<p class="font-ibm hover:font-medium hover:underline">joonyoung.dev</p>
		</a>
	</div>
</section>

<!-- EDUCATION -->
<section class="mt-10 font-ibm">
	<h1 class="text-2xl font-medium">EDUCATION</h1>

	<div class="mt-2">
		<b class="font-medium">Seoul National University</b>, Seoul, Republic of Korea
	</div>
	<div class="font-light">
		B.S., Electrical and Computer Engineering<br />
		B.A., Information Science
	</div>
	<div class="font-extralight">Mar 2017 - Feb 2025 (Expected) *</div>
	<div class="font-extralight">
		* includes a 2-year mandatory military service in Republic of Korea
	</div>
</section>

<!-- EXPERIENCE -->
<section class="mt-10 font-ibm">
	<h1 class="text-2xl font-medium">RESEARCH & WORK EXPERIENCE</h1>

	<div class="mt-2">
		<a href="http://hcid.snu.ac.kr/" target="_blank" rel="noopener noreferrer">
			<b class="font-medium hover:underline">HCI+d Lab,</b>
		</a> Seoul National University
	</div>
	<div class="font-light">Undergraduate Research Intern</div>
	<div class="font-extralight">Jan 2024 - Present</div>

	<div class="mt-3">
		<b class="font-medium">Samsung Electro-Mechanics</b>, Suwon, Republic of Korea
	</div>
	<div class="font-light">Undergraduate Intern</div>
	<div class="font-extralight">Jul 2019 - Aug 2019</div>
</section>

<!-- AWARDS & HONORS -->
<section class="mt-10 font-ibm">
	<h1 class="text-2xl font-medium">AWARDS & HONORS</h1>

	<div class="mt-2">
		<b class="font-medium">10% Merit-Based Scholarship</b>, Seoul National University
	</div>
	<div class="font-extralight">Feb 2017</div>
</section>

<!-- PROFICIENCY -->
<section class="mt-10 font-ibm">
	<h1 class="text-2xl font-medium">KEY STRENGTHS</h1>

	<h2 class="mt-3 text-lg font-medium">Programming</h2>
	<div class="mt-1 font-light">
		<b>Languages:</b> Python, C/C++, JavaScript/TypeScript, HTML & CSS, Dart, C#
	</div>
	<div class="font-light">
		<b>Tools & Frameworks:</b> Node.js, React/Next.js, Svelte/SvelteKit, p5.js, Flutter, TailwindCSS,
		NumPy, Pandas, Unity
	</div>
	<div class="font-light">
		<b>Others:</b> Git, LaTeX, Figma
	</div>

	<h2 class="mt-2 text-lg font-medium">Multilingual Skills</h2>
	<div class="mt-1 font-light">
		<b>Korean:</b> native language
	</div>
	<div class="font-light">
		<b>English:</b> TEPS 455 (near-native level of communicative competence)
	</div>
</section>

<section class="pb-20"></section>
