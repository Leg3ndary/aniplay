<script>
    // Parse out all animes into array from https://gogoanime.news/img/background.jpg asynchronously
    // and then display them in a grid
    import { onMount } from 'svelte';

    let animes = [];

    onMount(async () => {
        let response = await fetch('https://gogoanime.news/img/background.jpg');
        let text = await response.text();
        let regex = /<a href="\/category\/(.+?)">/g;
        let match;
        while ((match = regex.exec(text)) !== null) {
            animes.push(match[1]);
        }
        console.log(animes);
    });
    
</script>

<div class="animes">
    {#each animes as anime}
        <div class="anime">
            <a href="/anime/{anime}">{anime}</a>
        </div>
    {/each}
</div>