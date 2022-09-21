<script context="module">
	export const prerender = true;
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
	<div class="border ">
		<!-- Row 1 -->
		<div class="grid grid-flow-row grid-cols-12 lg:grid-cols-12 border-collapse font-light">
			<div class=" lg:col-span-2 border-r p-4 bgLines" />
			<div class="hidden lg:block border-r p-4">Hello, World!</div>
			<div
				class="border-r p-4 col-span-6 lg:col-span-4 uppercase flex flex-row text-xs lg:text-base font-medium"
			>
				<img
					src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif"
					class="w-5 h-5 object-cover"
					alt="svelte"
				/> I am Parag.
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
					<!-- <p>Menu</p> -->
				</div>
			</div>
			<div
				class="col-span-4 lg:col-span-2 border-r flex flex-row space-x-1 text-xs lg:text-base justify-center items-center bg-yellow-50 text-yellow-500 uppercase font-medium"
			>
				<p>#Thoughts</p>
			</div>
			<div class=" border-r p-4 bgLines" />
		</div>
		<!-- Row 2 -->
		<div
			class="grid grid-flow-row auto-rows-max grid-cols-12 lg:grid-cols-12 border-t border-collapse font-light"
		>
			<div class="lg:col-span-2 border-r p-4" />
			<div class="border-r p-4 col-span-5 lg:col-span-4 flex flex-col">
				<p class="lg:text-2xl tracking-wider">This webpage</p>
				<p>is meat to show</p>
				<div class="flex flex-row items-center">
					cool <p class="lg:text-5xl">Design</p>
					work
				</div>
			</div>
			<div class="border-r col-span-5 lg:col-span-2 h-full p-4">
				<div class="flex flex-col h-full justify-center items-center">
					<div
						class=" bg-rose-400 shadow-xl rounded w-full flex flex-col p-2 h-full justify-center items-center"
					>
						<div
							class=" rounded bg-yellow-50 p-3 flex flex-col justify-center items-center text-rose-50"
						>
							<p>
								<svg
									xmlns="http://www.w3.org/2000/svg"
									fill="none"
									viewBox="0 0 24 24"
									stroke-width="1.5"
									stroke="currentColor"
									class="w-6 h-6 "
								>
									<path
										stroke-linecap="round"
										stroke-linejoin="round"
										d="M8.25 21v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21m0 0h4.5V3.545M12.75 21h7.5V10.75M2.25 21h1.5m18 0h-18M2.25 9l4.5-1.636M18.75 3l-1.5.545m0 6.205l3 1m1.5.5l-1.5-.5M6.75 7.364V3h-3v18m3-13.636l10.5-3.819"
									/>
								</svg>
							</p>
							<p class="text-center text-sm lg:text-base font-semibold">
								Website is under Development
							</p>
						</div>
					</div>
				</div>
			</div>
			<div
				class="hidden lg:block border-r col-span-1 p-4 text-amber-800 border-l-4 border-amber-100 bg-amber-50"
			>
				Adversity bring opportunity
			</div>
			<div
				class="hidden lg:block col-span-1 p-4 text-amber-800 border-r-4 border-rose-100 bg-rose-50"
			>
				Uncertanity brings creativity
			</div>
			<div class=" border-r p-4 lg:col-span-2" />
		</div>
		<!-- Row 3 -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light  auto-rows-max">
			<div class="lg:col-span-2 border-r ">
				<img
					class="w-full h-full"
					src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645588282/My-Website/magicpattern-svg-chart-1645588275336_uiv5bd.png"
					alt=""
				/>
			</div>
			<div
				class="col-span-2 lg:col-span-1 p-4 flex flex-col space-y-12 items-center justify-center text-center bg-rose-400"
			>
				<div class=" font-bold uppercase transform -rotate-90">
					<span class="text-white text-lg lg:text-4xl text-transparent flex flex-row">
						#Design
					</span>
				</div>
			</div>
			<div
				class="border-r col-span-8 h-48 lg:h-full lg:col-span-3 relative overflow-hidden flex items-center"
			>
				<div
					class="absolute text-2xl lg:text-3xl top-0 left-0 ml-2 mt-2 font-bold text-rose-200/40 z-40 flex flex-col -space-y-4"
				>
					<p>Let's</p>
					<p>add</p>
					<p>some</p>
					<p>NOISE.</p>
				</div>
				<div class="lg:text-xl absolute bottom-0 right-0 mr-2 mb-2 text-rose-50 z-40">
					I use TailwindCSS <br /> to design
				</div>
				<img
					class="absolute w-full top-0 z-10"
					src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645555952/My-Website/magicpattern-grain-1645555941869_vytibh.png"
					alt=""
				/>
			</div>
			<div
				class="border-t lg:border-t-0 border-r pt-0 pr-0 col-span-6 lg:col-span-2 h-full flex flex-col relative polkaDots"
			>
				<div class="bg-amber-50/90 p-2 rounded-tr-full h-full">
					<img
						src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645553220/My-Website/488-bicycle-outline_ug9tew.gif"
						class="w-32 h-32 object-cover"
						alt="bicycle"
					/>
					<p class="text-sm lg:text-base text-amber-600">
						Desiging is like riding a bicycle, you'll need to get a grip for smooth experience.
					</p>
				</div>
			</div>
			<div class="border-t lg:border-t-0 lg:border-r col-span-6 lg:col-span-2 p-2 ">
				<div class="w-full h-full border-t border-r border-dashed border-amber-400 p-2">
					<div class="bg-amber-50 text-amber-600 w-full h-full flex flex-col p-4 text-sm">
						<p class="uppercase">I design</p>
						<div class="flex flex-row space-x-2 mt-4 items-center">
							<div class="h-2 w-2 bg-rose-300 rounded-full" />
							<p>Websites</p>
						</div>
						<div class="flex flex-row space-x-2 mt-1 items-center">
							<div class="h-2 w-2 bg-rose-300 rounded-full" />
							<p>Web Applications</p>
						</div>
						<div class="flex flex-row space-x-2 mt-1 items-center">
							<div class="h-2 w-2 bg-rose-300 rounded-full" />
							<p>SaaS Dashboards</p>
						</div>
						<div class="mt-3">...and deliver beautiful experiences.</div>
					</div>
				</div>
			</div>
			<div />
		</div>
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
		<!-- Row 5 -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light auto-rows-max">
			<div class="lg:col-span-2 border-r" />
			<div
				class="border-l-4 col-span-8 lg:col-span-4 p-4 lg:p-8 bg-red-50 w-full border-rose-400 flex flex-col justify-center items-start text-xs lg:text-lg font-medium text-gray-800 relative"
			>
				<p class="font-bold uppercase tracking-wide px-4">
					Have a <span class="text-rose-400">design</span> idea?
				</p>
				<p class="font-light px-4">So do you have a wonderful design idea in your mind?</p>
				<div
					class="h-12 bg-rose-500 w-full absolute bottom-0 -mb-10 lg:-mb-8 right-0 -mr-4 flex justify-center items-center p-3 text-xs lg:text-sm font-light text-white z-40"
				>
					It'll take 2 seconds to hit the contact button! <span>
						<button class="ml-2 bg-amber-300 text-rose-700 px-2 py-1 text-xxs lg:text-xs rounded"
							>Click Here</button
						>
					</span>
				</div>
			</div>
			<div class="border-r col-span-3 lg:col-span-2 relative">
				<div class="grid grid-flow-row lg:grid-cols-4 h-full relative">
					<div
						class="border-r h-full col-span-full lg:col-span-2 flex justify-center items-center relative"
					>
						<img
							class="absolute h-full w-full object-cover"
							src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645636937/My-Website/1827-growing-plant-outline_rpvzs2.gif"
							alt="plant"
						/>
					</div>
					<div class="hidden lg:block border-r h-full " />
					<div class="hidden lg:block	h-full " />
				</div>
			</div>
			<div class=" hidden lg:block border-r pt-0 pr-0 col-span-2 h-full" />
			<div class="hidden lg:block border-r col-span-2 p-2 " />
		</div>
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
		<!-- Row 7 - Development -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light h-16">
			<div class="lg:col-span-2 border-r" />
			<div
				class="bg-indigo-500 col-span-7 lg:col-span-3 w-full flex justify-center items-center text-white"
			>
				<span class="text-lg lg:text-3xl font-semibold uppercase"> #Development </span>
			</div>
			<!-- <div class="border-r  col-span-2 relative">
				<div class="grid grid-flow-row grid-cols-4 h-full">
					<div class="border-r h-full col-span-2"></div>
					<div class="border-r h-full "></div>
					<div class="	h-full "></div>
				</div>
			</div> -->
			<div class="border-r pt-0 pr-0 col-span-2 h-full " />
			<div class=" hidden lg:block border-r col-span-2 p-2 " />
			<div class="border-r col-span-2 p-2 " />
		</div>
		<!--  -->
	</div>
</section>

<style>
</style>
