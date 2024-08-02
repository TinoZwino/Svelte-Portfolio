
<script>
    let letters = ["W","e","l","c","o","m","e"]
</script>
<h1>
{#each letters as letter, i}
    <span class="welcome" style="animation-delay: {i}s">{letter}</span>
{/each}
</h1>

<style>
    @keyframes welcomeAnimation {
    0% {font-weight: 600;}
    100% {font-weight: 1000;}
    }


    h1, .welcome{
    font-weight: 600;
    font-style: normal;
    font-variation-settings:
      "slnt" 0,
      "wdth" 800,
      "GRAD" 0,
      "XOPQ" 96, /* Thick Stroke */
      "XTRA" 468, /* Counter Width */
      "YOPQ" 79, /* Thin Stroke */
      "YTAS" 750, /* Ascender Height */
      "YTDE" -203, /* Descender depth */
      "YTFI" 738, /* Figure height */
      "YTLC" 560, /* Lowercase height */
      "YTUC" 712; /* Uppercase height */

      animation: welcomeAnimation 3s;
      animation-timing-function: cubic-bezier(.45,.05,.55,.95);
      animation-iteration-count: alternate;
      animation-play-state: running;
    }

</style>