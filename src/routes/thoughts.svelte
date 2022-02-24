<script context="module">
	export const prerender = true;
</script>

<script>

</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<section class="overflow-hidden 2xl:container">
	<div class="border ">
		<!-- Row 1 -->
		<div class="grid grid-flow-row grid-cols-12 lg:grid-cols-12 border-collapse font-thin">
			<div class=" lg:col-span-2 border-r p-4 bgLines"></div>
			<div class="hidden lg:block border-r p-4">Hello, World!</div>
			<div class="border-r p-4 col-span-6 lg:col-span-4 uppercase flex flex-row text-xs lg:text-base font-medium">
				This is my site, <img
					src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif"
					class="w-5" alt="svelte"
				/>
			</div>
			<div class="hidden lg:block">
				<div class=" border-r p-4 flex flex-row space-x-2">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="h-6 w-6"
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h8m-8 6h16"
						/>
					</svg>
					<p>Menu</p>
				</div>
			</div>
			<div
				class="col-span-4 lg:col-span-2 border-r flex flex-row space-x-1 text-xs lg:text-base justify-center items-center bg-yellow-50 text-yellow-500 uppercase font-medium"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="h-3 lg:h-6 w-3 lg:w-6"
					fill="none"
					viewBox="0 0 24 24"
					stroke="currentColor"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M7 20l4-16m2 16l4-16M6 9h14M4 15h14"
					/>
				</svg>
				<p>Thoughts Page</p>
			</div>
			<div class=" border-r p-4 bgLines" />
		</div>
		<!-- Row 2 -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-thin  auto-rows-max">
			<div class="lg:col-span-2 border-r ">
				<img class="w-full h-full" src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645588282/My-Website/magicpattern-svg-chart-1645588275336_uiv5bd.png" alt="">
			</div>
			<div class="col-span-2 lg:col-span-1 p-4 flex flex-col space-y-12 items-center justify-center text-center bg-rose-400">
				<div class=" font-bold uppercase transform -rotate-90">
					<span class="bg-clip-text text-lg lg:text-4xl text-transparent bg-gradient-to-r from-amber-50 to-rose-50 flex flex-row">
						 Design
					</span>
				</div>
			</div>
			<div class="border-r col-span-8 h-48 lg:h-full lg:col-span-3 relative overflow-hidden flex items-center">
				<div class="absolute text-2xl lg:text-3xl top-0 left-0 ml-2 mt-2 font-bold text-rose-200/40 z-40 flex flex-col -space-y-4">
					<p>Let's</p>
					<p>add</p>
					<p>some</p>
					<p>NOISE.</p>
				</div>
				<div class="lg:text-xl absolute bottom-0 right-0 mr-2 mb-2 text-rose-50 z-40">I use TailwindCSS <br> to design</div>
				<img class="absolute w-full top-0 z-10" src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645555952/My-Website/magicpattern-grain-1645555941869_vytibh.png" alt="">
			</div>
			<div class="border-t lg:border-t-0 border-r pt-0 pr-0 col-span-6 lg:col-span-2 h-full flex flex-col relative polkaDots">
				<div class="bg-amber-50/90 p-2 rounded-tr-full h-full">
					<img src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645553220/My-Website/488-bicycle-outline_ug9tew.gif" class="w-32" alt="bicycle" />
					<p class="text-sm lg:text-base text-amber-600">Desiging is like riding a bicycle, you'll need to get a grip for smooth experience.</p>
				</div>
			</div>
			<div class="border-t lg:border-t-0 lg:border-r col-span-6 lg:col-span-2 p-2 ">
				<div class="w-full h-full border-t border-r border-dashed border-amber-400 p-2">
					<div class="bg-amber-50 text-amber-600 w-full h-full flex flex-col p-4 text-sm">
						<p class="uppercase">I design</p>
						<div class="flex flex-row space-x-2 mt-4 items-center">
							<div class="h-2 w-2 bg-rose-300 rounded-full"></div> <p>Websites</p>
						</div>
						<div class="flex flex-row space-x-2 mt-1 items-center">
							<div class="h-2 w-2 bg-rose-300 rounded-full"></div> <p>Web Applications</p>
						</div>
						<div class="flex flex-row space-x-2 mt-1 items-center">
							<div class="h-2 w-2 bg-rose-300 rounded-full"></div> <p>SaaS Dashboards</p>
						</div>
						<div class="mt-3">...and deliver beautiful experiences.</div>
					</div>
				</div>
			</div>
			<div></div>
		</div>

	</div>
</section>

<style>
</style>
