<script>
	import "../app.css";
	import Navbar from "$lib/components/Navbar.svelte";
	import Footer from "$lib/components/Footer.svelte";
</script>

<div>
	<Navbar />
	<main class=" bg-neutral-950/50 text-white">
		<slot></slot>
	</main>
	<Footer />
</div>