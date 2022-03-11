<script>
	import { onMount } from 'svelte';

	onMount(() => {
		const btn = document.querySelector('button');
		const menu = document.querySelector('.mobile-menu');

		btn.addEventListener('click', () => {
			menu.classList.toggle('hidden');
		});
	});
</script>

<nav>
	<div class="flex justify-between items-center bg-cyan-900 text-white font-bold">
		<div class="flex items-center p-3">
			<span
				><svg
					class="w-12 h-12"
					fill="none"
					stroke="currentColor"
					viewBox="0 0 24 24"
					xmlns="http://www.w3.org/2000/svg"
					><path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M8 9l3 3-3 3m5 0h3M5 20h14a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"
					/></svg
				></span
			><span class="ml-4 text-2xl">Svelte-Tailwind</span>
		</div>
		<div class=" space-x-4 hidden md:block p-4 text-xl">
			<a href="/">Home</a>
			<a href="/about">About</a>
			<a href="/contact">Contact</a>
		</div>
		<div class="block p-4 md:hidden">
			<button
				><svg
					class="w-8 h-8"
					fill="none"
					stroke="currentColor"
					viewBox="0 0 24 24"
					xmlns="http://www.w3.org/2000/svg"
					><path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M4 6h16M4 12h16M4 18h16"
					/></svg
				></button
			>
		</div>
	</div>
	<div class="flex flex-col space-y-4 p-4 mobile-menu md:hidden text-white bg-cyan-900 text-xl">
		<a class="hover:font-bold" href="/">Home</a>
		<a class="hover:font-bold" href="/about">About</a>
		<a class="hover:font-bold" href="/contact">Contact</a>
	</div>
</nav>
