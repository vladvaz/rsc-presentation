<script lang="ts">
	import { Presentation, Markdown } from '@components'
	import Slide from '@lib/components/slide.svelte'

	const categories = [
		'TDD',
		'Soft Skills',
		'Fun',
		'JavaScript',
		'Web',
		'.NET',
		'Architecture',
		'Microservices',
		'People',
		'Concurrency',
		'Languages',
		'Tools',
		'Security',
		'Functional Programming',
		'Design',
		'Docker',
		'Testing',
		'DevOps',
		'AI',
		'Ethics',
		'Machine Learning',
		'Agile',
		'UX',
		'Cloud',
		'UI',
		'IoT',
		'Microsoft',
		'Work skills',
		'Big Data',
		'Continuous Delivery',
		'Observability',
		'CI/CD',
		'Serverless',
		'Embedded',
	]
</script>

<Presentation>
	<Slide
		class="h-full"
		image="./slides/alfandega.jpeg"
		data-background-opacity="0.4"
	>
		<div class="h-full flex items-center justify-center flex-col">
			<h1>NDC Porto</h1>
			<h3>16-20 October 2023</h3>
			<h3>Alfândega Porto Congress Centre</h3>
		</div>
	</Slide>

	<Slide
		class="h-full "
		image="./slides/alfandega.jpeg"
		data-background-opacity="0.1"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<h2 class="fragment fade-up">Agenda</h2>
			<ul>
				<li class="fragment fade-left">3 days with talks</li>
				<li class="fragment fade-left">2 days with workshops</li>
				<li class="fragment fade-left">84 speakers</li>
			</ul>
			<div
				class="fragment flex flex-wrap justify-center gap-4 text-xs w-3/4 mt-8"
			>
				{#each categories as category}
					<span
						class="fade-up relative z-10 rounded-full bg-gray-50 px-3 py-1.5 font-medium text-gray-600 hover:bg-gray-100"
						>{category}</span
					>
				{/each}
			</div>
		</div>
	</Slide>

	<Slide
		class="h-full"
		image="./slides/background.jpg"
		data-background-opacity="0.1"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<h2 class="fragment fade-up">React server components</h2>
			<h3 class="fragment fade-up">Single Page Applications - SPA's</h3>
			<ul>
				<li class="fragment fade-left">
					A traditional single-page application (SPA) in React ships an empty
					div element with a large bundle of JavaScript
				</li>
				<li class="fragment fade-left">
					The client is then responsible for making data fetches to a database,
					computing the UI, and making the resulting HTML interactive
				</li>
				<li class="fragment fade-left">
					This process is known as client-side rendering (CSR)
				</li>
			</ul>
		</div>
	</Slide>

	<Slide
		class="h-full"
		image="./slides/background.jpg"
		data-background-opacity="0.1"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<h2>React server components</h2>
			<h3 class="fragment fade-up">Issues With SPA's</h3>
			<ul>
				<li class="fragment fade-left">Heavy lifting done by the client</li>
				<li class="fragment fade-left">Need javascript</li>
				<li class="fragment fade-left">Can turn website navigation slow</li>
				<li class="fragment fade-left">Poor performance on SEO</li>
				<li class="fragment fade-left">Security issues</li>
				<li class="fragment fade-left">
					Accuracy and usefulness of website traffic metrics
				</li>
			</ul>
		</div>
	</Slide>

	<Slide
		class="h-full"
		image="./slides/background.jpg"
		data-background-opacity="0.1"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<h2>React server components</h2>
			<h3 class="fragment fade-up">SSG and SSR</h3>
			<ul>
				<li class="fragment fade-left">Static Site Generation (SSG)</li>
				<li class="fragment fade-left">Occurs at build time</li>
				<li class="fragment fade-left">Server-Side Rendering (SSR)</li>
				<li class="fragment fade-left">Routes are rendered at request time</li>
				<li class="fragment fade-left">
					Both fetch the content from the server and generate the resulting HTML
				</li>
			</ul>
		</div>
	</Slide>

	<Slide
		class="h-full"
		image="./slides/background.jpg"
		data-background-opacity="0.1"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<h2>React server components</h2>
			<h3 class="fragment fade-up">An hybrid approach</h3>
			<ul>
				<li class="fragment fade-left">
					Represent the latest advancement in pre-rendering content on the web
				</li>
				<li class="fragment fade-left">
					Components can be created both on server and on the client
				</li>
				<li class="fragment fade-left">
					Server rendering can now happen at the component level
				</li>
				<li class="fragment fade-left">
					Server Components also seamlessly interweave with Client Components
				</li>
				<li class="fragment fade-left">
					Smaller client-side JavaScript bundles
				</li>
			</ul>
		</div>
	</Slide>

	<Slide
		class="h-full"
		image="./slides/background.jpg"
		data-background-opacity="0.1"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<h2>React server components</h2>
			<h3 class="fragment fade-up">Frameworks that currently support RSC</h3>
			<div class="mt-16">
				<h3 class="fragment fade-left">Next.js</h3>
				<h3 class="fragment fade-left">Hydrogen</h3>
				<h3 class="fragment fade-left">Remix</h3>
			</div>
		</div>
	</Slide>

	<Slide
		class="h-full"
		image="./slides/demo.png"
		data-background-opacity="0.5"
		data-auto-animate
	>
		<div class="flex flex-col items-center">
			<div class="mt-48 bg-gray-500/[0.8] p-8 rounded-lg">
				<!-- svelte-ignore a11y-missing-content -->
				<h2 class="fragment fade-up">Demo</h2>
				<a
					href="https://nextjs-dashboard-seven-fawn-35.vercel.app/"
					class="fragment fade-up"
					>https://nextjs-dashboard-seven-fawn-35.vercel.app/</a
				>
			</div>
		</div>
	</Slide>
</Presentation>
