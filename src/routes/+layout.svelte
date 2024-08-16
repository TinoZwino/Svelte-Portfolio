

<header>
    <nav>
        <ul>
            <li><a href="/"><span class="material-symbols-outlined icon">home</span><span>Home</span></a></li>
            <li><a href="/links"><span class="material-symbols-outlined icon">link</span><span>Links</span></a></li>
        </ul>
    </nav>
</header>

<slot></slot>

<footer>
    <p>© Tino_Zwino 2024</p>
</footer>

<style>
    @import '/main.css';

    header, footer{
        display:flex;
        position: fixed;
        width: 100%;
        justify-content:center;
        align-items:center;

    }

    header{
        top: 0;
    }

    footer{
            bottom: 0;
        }

    footer p{
        font-variation-settings:
        "GRAD" -200,
        "YTLC" 440, /* Lowercase height */
        "YTUC" 600, /* Uppercase height */
        "YTFI" 560; /* Figure height */

        transition: font-variation-settings 0.25s cubic-bezier(.45,.05,.55,.95);
    }

    footer p:hover{
        font-variation-settings:
        "GRAD" 150,
        "YTLC" 570, /* Lowercase height */
        "YTUC" 760, /* Uppercase height */
        "YTFI" 788; /* Figure height */

      }
</style>
    