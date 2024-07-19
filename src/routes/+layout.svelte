<script>
	import '../app.css';
	import Navbar from '$lib/components/Navbar.svelte';
</script>

<div class="bg-[url('/heroSectionBG.jpg')] h-screen bg-cover">
	<Navbar />
	<slot></slot>
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Readex+Pro:wght@160..700&display=swap');
</style>
