<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-crimson.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import NavBar from '$lib/components/nav-bar.svelte';
	import { AppShell } from '@skeletonlabs/skeleton';
	import Footer from '$lib/components/footer.svelte';
</script>

<AppShell>
	<svelte:fragment slot="header">
		<NavBar />
	</svelte:fragment>

	<!-- <div class="flex flex-col justify-between"> -->
	<slot />
	<!-- </div> -->

	<svelte:fragment slot="pageFooter">
		<Footer />
	</svelte:fragment>
</AppShell>
