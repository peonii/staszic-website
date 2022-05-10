<script>
    export let name;
    export let route;
    export let desc;
</script>

<a href={route} class="w-1/2">
    <div class="rounded-2xl mx-12 p-4 my-6 min-w-1/3 border-slate-100 border-2 hover:shadow-lg hover:border-white hover:scale-105 transition">
            <h1 class="text-xl font-bold text-red-500">{name}</h1>
            <p class="text-slate-700">{desc}</p>
            <p class="text-slate-400 italic">{route}</p>
    </div>
</a>