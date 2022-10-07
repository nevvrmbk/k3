<script lang='ts'>
    import Counter from "$lib/Counter.svelte";
    import Lists from "$lib/Lists.svelte";
</script>

<svelte:head>
    <title>Document</title>
</svelte:head>

<section class="container text-center m-2 p-4">
    <h1 class="border-bottom">Welcome to SvelteKit</h1>
    <p class="lead pt-4">Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
</section>

<Counter />

<Lists />
