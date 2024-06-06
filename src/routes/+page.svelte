<script lang="ts">
    import {arrSplit} from '$lib/arrUtil';
    import HeroSection from './components/heroSection.svelte';

    let count = 0;

    const increment = (val:number) => {
        count = count + val
    }

    console.log(arrSplit('h,ello worl,d'))
</script>


<HeroSection title="Home hero section"></HeroSection>

<button on:click={() => increment(2)}>
increment ({count})
</button>
<p>
    {count}
</p>
