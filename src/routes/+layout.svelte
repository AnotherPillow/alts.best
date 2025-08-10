<script lang="ts">
    import '@fontsource/lato';
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
	
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
    <meta content="alts.best" property="og:title">
    <meta content="The best alts place." property="og:description">
</svelte:head>

{@render children?.()}
