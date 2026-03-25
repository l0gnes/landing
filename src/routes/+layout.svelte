<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<title>lognes.dev</title>
	<link rel="icon" href={favicon} />
</svelte:head>

<div class="h-full w-full flex">
	{@render children()}
</div>
