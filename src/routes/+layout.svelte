<script lang="ts">
	// Your selected Skeleton theme:
	import "@skeletonlabs/skeleton/themes/theme-skeleton.css";

	// This contains the bulk of Skeletons required styles:
	import "@skeletonlabs/skeleton/styles/all.css";

	// Finally, your application's global stylesheet (sometimes labeled 'app.css')
	import "../app.postcss";

	import "../app.postcss";

	import Nav from "$lib/Nav.svelte";
	import Header from "$lib/Header.svelte";
	import Footer from "$lib/Footer.svelte";
</script>

<svelte:head>
	<title>SvelteKit Deployment Configuration</title>
	<meta
		name="description"
		content="Learn how to configuration your SvelteKit app to use Edge Functions, Serverless Functions, and Incremental Static Regeneration on Vercel"
	/>
</svelte:head>

<div class="px-8 lg:px-0 h-screen flex flex-col justify-between">
	<Header />
	<div class="flex-grow w-full max-w-4xl mx-auto flex flex-col md:flex-row">
		<Nav />
		<div class="md:ml-12">
			<slot />
		</div>
	</div>
	<Footer />
</div>
