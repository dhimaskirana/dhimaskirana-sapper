<script context="module">
	export function preload() {
		return this.fetch(`review.json`)
			.then((r) => r.json())
			.then((posts) => {
				return { posts };
			});
	}
</script>

<script>
	export let posts;
</script>

<svelte:head>
	<title>Paid Post Review</title>
</svelte:head>

<!-- ======= Blog Single ======= -->
<div class="main-content paddsection">
	<div class="container">
		<div class="row justify-content-center">
			<div class="col-md-8 col-md-offset-2">
				<div class="row">
					<div class="container-main single-main">
						<div class="col-md-12">
							<div class="block-main mb-30">
								<div class="content-main single-post padDiv">
									<div class="journal-txt">
										<h4>Paid Post Review</h4>

										<ul>
											{#each posts as post}
												<!-- we're using the non-standard `rel=prefetch` attribute to
				tell Sapper to load the data for the page as soon as
				the user hovers over the link or taps it, instead of
				waiting for the 'click' event -->
												<li>
													<a
														rel="prefetch"
														href="review/{post.slug}"
														>{post.title}</a
													>
												</li>
											{/each}
										</ul>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
<!-- End Blog Single -->
