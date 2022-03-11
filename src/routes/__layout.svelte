<script>
	import '../app.css';
	import Nav from '../components/Nav.svelte';
	import Footer from '../components/Footer.svelte';
</script>

<div class="flex flex-col bg-gradient-to-r from-zinc-800 to-gray-600 h-screen">
	<Nav />
	<div class="mb-auto"><slot /></div>
	<Footer />
</div>
