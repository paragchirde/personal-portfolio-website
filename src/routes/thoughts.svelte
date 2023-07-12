<script context="module">
	export const prerender = true;
	const thoughts = [
		{
			id:1,
			data: 'A hammer that breaks the glass, also forges a steel.'
		},
		{
			id:2,
			data: 'Your real resume is just a catalog of all your sufferings.'
		},
			
	]
</script>

<script>
</script>

<svelte:head>
	<title>Parag Chirde - Thoughts</title>
</svelte:head>

<section class="overflow-hidden 2xl:container pt-14 font-light">
	<div class="border-b ">
		<!-- Row 1 -->
		<div class="grid grid-flow-row grid-cols-12 border-t border-collapse  auto-rows-max">
			<div class="lg:col-span-2 border-r ">
				<img
					class="w-full h-full"
					src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645588282/My-Website/magicpattern-svg-chart-1645588275336_uiv5bd.png"
					alt=""
				/>
			</div>
			<!--  -->
			<div
				class="col-span-2 lg:col-span-8 p-4 "
			>
				<div class="grid grid-flow-row grid-cols-4 gap-4">
					{#each thoughts as thought }	
						<div class="	w-full border-b border-l p-4">
							<span
								class=" text-xs lg:text-base flex flex-row"
							>
								{thought.data}
							</span>
						</div>
					{/each}
				</div>
			</div>
			<!--  -->
			<div class="lg:col-span-2 border-r ">
				<img
					class="w-full h-full"
					src="https://res.cloudinary.com/dqn0fj8ae/image/upload/v1645588282/My-Website/magicpattern-svg-chart-1645588275336_uiv5bd.png"
					alt=""
				/>
			</div>
		</div>
	</div>
</section>

<style>
</style>
