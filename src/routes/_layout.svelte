<style>
	@import url("https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css");
</style>
<script>
	// import Nav from '../components/Nav.svelte';
	import Footer from "../components/Footer.svelte";
	export let segment;
</script>

<!-- <Nav {segment}/> -->

<main id="main">
	<slot />
</main>

<Footer />
