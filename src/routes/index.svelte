<script>
    import Site from './components/Site.svelte'

    let pages = [
        { name: 'iPhone', desc: 'Kup już teraz gato gratis darmowe!', route: '/iphone' },
        { name: 'Zwierzę', desc: 'Zaliczenie na informatykę - 31/05/2022', route: '/zwierze' },
        { name: 'Personal', desc: 'Osobista strona internetowa', route: 'https://querter.me/' }
    ]
</script>

<svelte:head>
    <title>qtr's site selector</title>
</svelte:head>

<div class="border-slate-300 border-b-2 mx-6 select-none pointer-events-none">
    <h1 class="text-4xl font-bold text-center my-4">qtr's site selector</h1>
</div>

<div class="flex justify-center w-full flex-row flex-wrap">
    {#each pages as page}
        <Site {...page} />
    {/each}
</div>

<div class="select-none cursor-default text-slate-200 text-4xl text-center my-32 animate-pulse">
    More sites coming soon...
</div>