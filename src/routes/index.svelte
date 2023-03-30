<script context="module">
	export async function load({ fetch }) {
		const res = await fetch(
			'https://api.rss2json.com/v1/api.json?rss_url=https%3A%2F%2Fparagchirde.medium.com%2Ffeed'
		);
		const data = await res.json();
		if (res.ok) {
			return {
				props: { blogs: data.items }
			};
		}
	}
	export const prerender = true;
	import Row1 from '../lib/WebSections/Index/Row1.svelte';
	import Row2 from '../lib/WebSections/Index/Row2.svelte';
	import Row3 from '../lib/WebSections/Index/Row3.svelte';
	import Skills from '../lib/WebSections/Index/Skills.svelte';
	import Blogs from '../lib/WebSections/Index/Blogs.svelte';
</script>

<script>
	export let blogs;
</script>

<svelte:head>
	<title>Parag Chirde</title>
	<meta name="title" content="Parag's Portfolio Website" />
	<meta name="description" content="Parag's portfolio website" />

	<!-- Open Graph / Facebook -->
	<meta property="og:type" content="website" />
	<meta property="og:url" content="https://www.paragchirde.com/" />
	<meta property="og:title" content="Parag Chirde" />
	<meta property="og:description" content="Parag's portfolio website" />
	<meta property="og:image" content="" />

	<!-- Twitter -->
	<meta property="twitter:card" content="summary_large_image" />
	<meta property="twitter:url" content="https://www.paragchirde.com/" />
	<meta property="twitter:title" content="Parag Chirde" />
	<meta property="twitter:description" content="Parag's portfolio website" />
	<meta property="twitter:image" content="" />
</svelte:head>

<section class="overflow-hidden 2xl:container">
	<div class="border">
		<!-- Row 1  - The Navbar -->
		<Row1 />
		<!-- Row 2 - The Profile -->
		<Row2 />
		<!-- Row 3 - The forte -->
		<Row3 />
		<!-- Row 4 -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light h-16">
			<div class="col-span-2 border-r" />
			<div class="" />
			<div class="border-r  col-span-2 relative">
				<div class="grid grid-flow-row grid-cols-4 h-full">
					<div class="border-r h-full col-span-2" />
					<div class="border-r h-full " />
					<div class="	h-full " />
				</div>
			</div>
			<div class="border-r pt-0 pr-0 col-span-3 h-full flex flex-col relative" />
			<div class="border-r col-span-2 p-2 " />
			<div class="border-r col-span-2 p-2 " />
		</div>
		<!-- Row Skills -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light h-16">
			<div class="lg:col-span-2 border-r" />
			<div class=" col-span-7 lg:col-span-3 w-full p-4">
				<span class="text-md lg:text-lg font-semibold uppercase"
					>Technical Skills<span class="text-rose-400">.</span>
				</span>
			</div>
			<div class="border-r pt-0 pr-0 col-span-2 h-full " />
			<div class=" hidden lg:block border-r col-span-2 p-2 " />
			<div class="border-r col-span-2 p-2 " />
		</div>
		<!-- Row 5 - Skills Quote -->
		<Skills />
		<!-- Row Blogs -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light h-16">
			<div class="lg:col-span-2 border-r" />
			<div class=" col-span-7 lg:col-span-3 w-full p-4 flex justify-between items-center">
				<p>
					<span class="text-md lg:text-lg font-semibold uppercase"
						>Blogs<span class="text-rose-400">.</span>
					</span>
				</p>
				<div class="flex flex-row space-x-2 justify-end items-center w-full">
					<p>
						<a href="https://paragchirde.medium.com/" target="_blank" rel="noopener noreferrer">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" viewBox="0 0 24 24"
								><path
									fill="currentColor"
									d="M20 3H4a1 1 0 0 0-1 1v16a1 1 0 0 0 1 1h16a1 1 0 0 0 1-1V4a1 1 0 0 0-1-1zm-2.046 4.265l-.966.925a.28.28 0 0 0-.106.271v6.801a.28.28 0 0 0 .106.271l.942.926v.204h-4.741v-.204l.977-.948c.097-.096.097-.125.097-.271V9.742l-2.716 6.896h-.368L8.018 9.742v4.622a.644.644 0 0 0 .176.531l1.271 1.541v.203H5.861v-.203l1.271-1.541a.618.618 0 0 0 .164-.531V9.02a.468.468 0 0 0-.152-.395l-1.13-1.36v-.203H9.52l2.71 5.943l2.382-5.943h3.343v.203z"
								/></svg
							>
						</a>
					</p>
					<p>
						<a href="https://dev.to/chirdeparag" target="_blank" rel="noopener noreferrer">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" viewBox="0 0 24 24"
								><path
									fill="currentColor"
									d="M7.826 10.083a.784.784 0 0 0-.468-.175h-.701v4.198h.701a.786.786 0 0 0 .469-.175c.155-.117.233-.292.233-.525v-2.798c.001-.233-.079-.408-.234-.525zM19.236 3H4.764C3.791 3 3.002 3.787 3 4.76v14.48c.002.973.791 1.76 1.764 1.76h14.473c.973 0 1.762-.787 1.764-1.76V4.76A1.765 1.765 0 0 0 19.236 3zM9.195 13.414c0 .755-.466 1.901-1.942 1.898H5.389V8.665h1.903c1.424 0 1.902 1.144 1.903 1.899v2.85zm4.045-3.562H11.1v1.544h1.309v1.188H11.1v1.543h2.142v1.188h-2.498a.813.813 0 0 1-.833-.792V9.497a.813.813 0 0 1 .792-.832h2.539l-.002 1.187zm4.165 4.632c-.531 1.235-1.481.99-1.906 0l-1.548-5.818h1.309l1.193 4.569l1.188-4.569h1.31l-1.546 5.818z"
								/></svg
							>
						</a>
					</p>
				</div>
			</div>
			<div class="border-r pt-0 pr-0 col-span-2 h-full " />
			<div class=" hidden lg:block border-r col-span-2 p-2 " />
			<div class="border-r col-span-2 p-2 " />
		</div>
		<!-- Row Blogs Data -->
		<Blogs {blogs} />
	</div>
</section>

<style>
</style>
