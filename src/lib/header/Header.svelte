<script>
	import * as animateScroll from 'svelte-scrollto';
	import { fade } from 'svelte/transition';
	let visible = true;
	animateScroll.setGlobalOptions({
		offset: -100
	});
	let isOpen = false;
	let showItems = false;
	let scrollPx = null;
	function openNav() {
		isOpen = true;
		showItems = true;
		document.getElementById('mainNav').style.background = '#fff';
	}
	function closeNav() {
		showItems = false;
		isOpen = false;
		document.getElementById('mainNav').style.background = '';
	}
</script>

<svelte:window bind:scrollY={scrollPx} />

<header class="w-full">
	{#if scrollPx > 150}
		<nav transition:fade
			class="fixed top-0 w-full shadow-lg mb-6 z-10"
			id="mainNav"
			style="transition-duration: 0.5s;z-index:9999999;"
		>
			<div class="navBg h-16" />
			<div class="bg-transparent top-0 absolute w-full z-40">
				<div class="flex items-center justify-between h-16 px-4 py-5">
					<div>
						<a href="/" v-scroll-to="'#home'" class="flex flex-row items-center">
							<div class="w-12 md:w-16 2xl:w-20">
								<img
									alt="ortigan-logo"
									src="https://res.cloudinary.com/binarycode/image/upload/v1597915831/Ortigan%20Official/ortigan_nav_bar_logo_left_kkv2u4.svg"
								/>
							</div>
						</a>
					</div>
					<div class="hidden md:block">
						<div class="flex items-center font-light 2xl:text-2xl 3xl:text-2xl">
							<a href="#/" class="" on:click={() => animateScroll.scrollTo({ element: 'home' })}
								><p class=" mr-4">Home</p></a
							>
							<a href="#/" on:click={() => animateScroll.scrollTo({ element: '#aboutus' })}
								><p class=" mr-4">About</p></a
							>
							<a href="#/" on:click={() => animateScroll.scrollTo({ element: '#services' })}
								><p class=" mr-4">Services</p></a
							>
							<a href="#/" on:click={() => animateScroll.scrollTo({ element: '#work' })}
								><p class=" mr-4">Work</p></a
							>
							<a href="#/" on:click={() => animateScroll.scrollTo({ element: '#clients' })}
								><p class=" mr-4">Clients</p></a
							>
							<a href="#/" on:click={() => animateScroll.scrollTo({ element: '#team' })}
								><p class=" mr-4">Team</p></a
							>
							<!-- <DailyBytesButton/> -->
						</div>
					</div>
					<div class="flex justify-center">
						<div class="w-20 2xl:w-32 text-center" v-scroll-to="'#home'">
							<img
								alt="ortigan-text"
								src="https://res.cloudinary.com/binarycode/image/upload/v1597915831/Ortigan%20Official/ortigan_nav_bar_logo_right_yn9mb4.svg"
							/>
						</div>
					</div>
					<div class="md:hidden">
						<button
							type="button"
							name="nav-button"
							class="block text-gray-500 hover: focus: focus:outline-none"
						>
							{#if !isOpen}
								<svg on:click={openNav} class="h-6 w-6 fill-current" viewBox="0 0 24 24">
									<path
										fill="#1c1d1f"
										fill-rule="evenodd"
										d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
									/>
								</svg>
							{/if}
							{#if isOpen}
								<svg
									on:click={closeNav}
									class="h-6 w-6 fill-current"
									viewBox="0 0 24 24"
									v-if="isOpen"
								>
									<path
										fill="#1c1d1f"
										fill-rule="evenodd"
										d="M18.278 16.864a1 1 0 0 1-1.414 1.414l-4.829-4.828-4.828 4.828a1 1 0 0 1-1.414-1.414l4.828-4.829-4.828-4.828a1 1 0 0 1 1.414-1.414l4.829 4.828 4.828-4.828a1 1 0 1 1 1.414 1.414l-4.828 4.829 4.828 4.828z"
									/>
								</svg>
							{/if}
						</button>
					</div>
				</div>
				<div
					class={isOpen == true
						? 'block navBg flex justify-center h-screen'
						: 'hidden navBg flex justify-center h-screen'}
				>
					<transition name="fade">
						<div class="flex flex-col justify-center" v-show="showItems" on:click={closeNav}>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: 'home' })}
								v-scroll-to="'#home'"
								class="px-2 py-1 text-darkPrimary font-semibold text-center  rounded navItem"
								>Home</a
							>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: '#aboutus' })}
								class="mt-1 block px-2 py-1 text-darkPrimary text-center font-semibold  rounded navItem"
								>About</a
							>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: '#services' })}
								class="mt-1 block px-2 py-1 text-darkPrimary text-center font-semibold  rounded navItem"
								>Services</a
							>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: '#work' })}
								class="mt-1 block px-2 py-1 text-darkPrimary text-center font-semibold  rounded navItem"
								>Work</a
							>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: '#clients' })}
								class="mt-1 block px-2 py-1 text-darkPrimary text-center font-semibold  rounded navItem"
								>Clients</a
							>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: '#team' })}
								class="mt-1 block px-2 py-1 text-darkPrimary text-center font-semibold  rounded navItem"
								>Team</a
							>
							<a
								href="#/"
								on:click={() => animateScroll.scrollTo({ element: '#techstack' })}
								v-scroll-to="'#techstack'"
								class="mt-1 block px-2 py-1 text-darkPrimary text-center font-semibold  rounded navItem"
								>Tech Stack</a
							>
						</div>
					</transition>
				</div>
			</div>
		</nav>
	{/if}
</header>

<style>
	.navBg {
		backdrop-filter: saturate(180%) blur(5px);
		background-color: rgba(240, 240, 240, 0.8);
	}
</style>
