<script context="module">
	export async function preload({ params }) {
		// the `slug` parameter is available because
		// this file is called [slug].svelte
		const res = await this.fetch(`review/${params.slug}.json`);
		const data = await res.json();

		if (res.status === 200) {
			return { post: data };
		} else {
			this.error(res.status, data.message);
		}
	}
</script>

<script>
	export let post;
</script>

<svelte:head>
	<title>{post.title}</title>
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
										<h4>{post.title}</h4>
										{@html post.html}
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
