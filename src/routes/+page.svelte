
<script>
    let letters = ["W","e","l","c","o","m","e"]
</script>
<h1>
{#each letters as letter, i}
    <span class="welcome" style="animation-delay: {i/2}s">{letter}</span>
{/each}
</h1>

<style>
    @keyframes welcomeAnimation {
    0% {font-variation-settings: "YTLC" 440, /* Lowercase height */ "YTUC" 600, /* Uppercase height */ "YTFI" 560; /* Figure height */}
    25% {font-weight: 300;
        font-variation-settings: "YTLC" 570, /* Lowercase height */ "YTUC" 760, /* Uppercase height */ "YTFI" 788; /* Figure height */}
    75% {font-weight: 1000;
        font-variation-settings: "YTLC" 570, /* Lowercase height */ "YTUC" 760, /* Uppercase height */ "YTFI" 788; /* Figure height */}
    100% {font-variation-settings: "YTLC" 440, /* Lowercase height */ "YTUC" 600, /* Uppercase height */ "YTFI" 560; /* Figure height */}
    }


    .welcome{
    font-weight: 300;
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
/*       "YTLC" 560, /* Lowercase height */
      "YTUC" 712; /* Uppercase height */

      animation: welcomeAnimation 1s;
      animation-timing-function: cubic-bezier(.45,.05,.55,.95);
      animation-iteration-count: infinite;
      animation-direction: alternate;
      animation-play-state: running;


    }
</style>