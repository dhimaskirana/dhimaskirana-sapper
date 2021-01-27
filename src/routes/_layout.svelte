<script>
	// import Nav from '../components/Nav.svelte';
	import Footer from "../components/Footer.svelte";
	import GoogleAnalytics from "../components/GoogleAnalytics.svelte";
	export let segment;
</script>

<!-- <Nav {segment}/> -->
<GoogleAnalytics />
<main id="main">
	<slot />
</main>

<Footer />
