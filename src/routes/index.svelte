<script context="module">
	export const prerender = true;
	import Row1 from '../lib/WebSections/Index/Row1.svelte'
	import Row2 from '../lib/WebSections/Index/Row2.svelte'
	import Row3 from '../lib/WebSections/Index/Row3.svelte'
	import Skills from '../lib/WebSections/Index/Skills.svelte'
</script>

<script>
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
		<Row1></Row1>
		<!-- Row 2 - The Profile -->
		<Row2></Row2>
		<!-- Row 3 - The forte -->
		<Row3></Row3>
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
			<div
				class=" col-span-7 lg:col-span-3 w-full p-4"
			>
				<span class="text-md lg:text-lg font-semibold uppercase">Technical Skills<span class="text-rose-400">.</span> </span>
			</div>
			<div class="border-r pt-0 pr-0 col-span-2 h-full " />
			<div class=" hidden lg:block border-r col-span-2 p-2 " />
			<div class="border-r col-span-2 p-2 " />
		</div>
		<!-- Row 5 - Skills Quote -->
		<Skills></Skills>
		<!-- Row 6 -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light h-32">
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
		<!--  -->
	</div>
</section>

<style>
</style>
