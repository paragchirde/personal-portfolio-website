<script>
	import Header from '$lib/WebSections/Index/Row1.svelte';
	import Footer from '$lib/Footer/footer.svelte';
	import '../app.css';
</script>	
<!-- 
<Header /> -->

<main class="w-full">
	<Header></Header>
	<slot />
</main>

<Footer/>
<style>
</style>
