<script>
	import { onMount } from "svelte";
	let typed;
	let options = {
		strings: [
			"Dhimas Kirana.",
			"WordPress Developer.",
			"from Yogyakarta, Indonesia.",
		],
		typeSpeed: 100,
		loop: true,
	};
	onMount(() => {
		runtypedjs();
	});
	function runtypedjs() {
		typed = new Typed(".typed", options);
	}
</script>

<svelte:head>
	<title>Dhimas Kirana - WordPress Developer</title><script
		src="https://cdn.jsdelivr.net/npm/typed.js">
	</script></svelte:head
>

<!-- start section hero -->
<div
	id="hero"
	class="home"
	style="background: url('/uploads/dhimaskirana.jpg') repeat scroll left center / cover;"
>
	<div class="container">
		<div class="hero-content">
			<h1>I'm <span class="typed" /></h1>
			<p>WP DEV</p>

			<!-- <ul class="list-unstyled list-social">
					<li><a href="#"><i class="ion-social-facebook"></i></a></li>
					<li><a href="#"><i class="ion-social-twitter"></i></a></li>
					<li><a href="#"><i class="ion-social-instagram"></i></a></li>
					<li><a href="#"><i class="ion-social-googleplus"></i></a></li>
					<li><a href="#"><i class="ion-social-tumblr"></i></a></li>
					<li><a href="#"><i class="ion-social-dribbble"></i></a></li>
				</ul> -->
		</div>
	</div>
</div>
<!-- End section hero -->

<!-- start sectoion contact -->
<div id="contact" class="paddsection">
	<div class="container">
		<div class="contact-block1">
			<div class="row">
				<div class="col-lg-6">
					<div class="contact-contact">
						<h2 class="mb-30">ABOUT ME</h2>
						<hr />
						<p>
							Hello, my name is Dhimas Kirana. I'm WordPress
							Developer from Yogyakarta, Indonesia.
						</p>
						<ul class="contact-details">
							<li>
								<span
									>Blog: <a
										href="https://blog.dhimaskirana.com/"
										target="_blank"
										>https://blog.dhimaskirana.com/</a
									></span
								>
							</li>
							<li>
								<span
									>Github: <a
										href="https://github.com/dhimaskirana"
										target="_blank"
										>https://github.com/dhimaskirana</a
									></span
								>
							</li>
						</ul>
						<br />
						<a class="btn btn-block" href="http://bit.ly/2peNfV7"
							>Download Printable Resume</a
						>
						<br /><br />
					</div>
				</div>

				<div class="col-lg-6">
					<h2 class="mb-30">MY EXPERIENCE</h2>
					<hr />
					<p>
						Hello, my name is Dhimas Kirana. I'm a WordPress
						Developer from Yogyakarta, Indonesia. I have been
						working as a Freelance WordPress Developer since 2018. I
						love developing WordPress and doing customization on the
						WordPress backend.
					</p>
					<p>
						More about me, check <a
							href="https://www.linkedin.com/in/dhimaskirana"
							target="_blank">my Linkedin Profile</a
						>.
					</p>
					<p>
						<a rel="prefetch" href="review">Review Post Page</a>
					</p>
				</div>
			</div>

			<div class="row">
				<div class="col-lg-12 text-center">
					<hr />
					<p>
						Interested in working with me? Let's discuss it
						together!
					</p>
					<p>
						Just email me (<a href="mailto:me@dhimaskirana.com"
							>me@dhimaskirana.com</a
						>)
					</p>
				</div>
			</div>
		</div>
	</div>
</div>

<!-- start sectoion contact -->
<style>
	.hero-content {
		text-align: right !important;
	}
</style>
