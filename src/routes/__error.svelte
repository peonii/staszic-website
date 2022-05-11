<script context="module">
    export function load({error, status}) {
        return {
            props: {
                status: `${status}`,
                error: `${error.message}`
            }
        }
    }
</script>

<script>
    export let status;
    export let error;
</script>

<h1 class="text-5xl text-center m-12">{status}</h1>
<h2 class="text-slate-600 text-center m-6 text-3xl">Coś poszło nie tak!</h2>

<p class="text-center text-xl">{error}</p>

<div class="text-center my-10 underline text-3xl">
    <a href="/" class="text-center">Powróć do strony</a>
</div>