<header>
    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/links">Links</a></li>
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

    footer{
            bottom: 0;
        }

    header{
        top: 0;
    }
</style>
    