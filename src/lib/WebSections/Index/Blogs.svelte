<script>
	export let blogs;
	import BlogCard from '$lib/Cards/Blog.svelte';
</script>

<div class="grid grid-flow-row grid-cols-12 border-t border-collapse font-light">
	<div class="col-span-0 lg:col-span-2 border-r" />
	<div class=" col-span-12 lg:col-span-8 w-full p-4 flex justify-between items-center ">
		<div class="grid grid-flow-row grid-cols-2 lg:grid-cols-4 gap-2 lg:gap-4">
			<!-- svelte-ignore empty-block -->
			{#each blogs as blog}
                <a href={blog.link} target="_blank" rel="noopener noreferrer">
                    <div class="border flex flex-col h-full">
                        <div>
                            <img class="h-16 lg:h-24 w-full object-cover" alt={blog.title} src={blog.thumbnail}/>
                        </div>
                        <div class="p-2 lg:p-4">
                            <p class="text-sm lg:text-sm font-base"> {blog.title} </p>
                        </div>
                        <div class="px-2 lg:px-4 pb-4">
                            <div class="text-xxs lg:text-xxs font-base flex flex-wrap gap-2">
                                {#each blog.categories as c }
                                       <div class="rounded-full px-4 py-0.5 border"> {c} </div> 
                                {/each}
                            </div>
                        </div>
                    </div>
                </a>
			{/each}
		</div>
	</div>
	<div class="border-r border-l col-span-0 lg:col-span-2 p-2 " />
</div>
