<script>
    import photoEnzo from '$lib/images/image_accueil_navbar.png';
</script>
<nav>
    <img class="photoEnzo" src={photoEnzo} alt="">
    <ul>
        <li>
            <a href="/">Accueil</a>
        </li>
        <li>
            <a href="/Experiences">Expériences</a>
        </li>
        <li>
            <a href="/Projets">Mes Projets</a>
        </li>
        <li>
            <a href="/Contact" class="button">Contact</a>
        </li>
    </ul>
</nav>

<slot/>

<style>
    ul {
        display: flex;
        justify-content: flex-end;
        margin-right: 100px;
        padding: 0;
        list-style: none;
    }

    li {
        margin-left: 64px;
    }

    a {
        text-decoration: none;
        color: #FFFFFF;
        font-weight: 700;
        transition: color 0.3s;
        font-family: Montserrat, sans-serif;
    }

    a:hover {
        color: #002333;
    }

    button {
        background-color: #002333;
    }

    .photoEnzo {
        right: 0;
        top: 0;
        z-index: -1;
        position: absolute;
        height: 110%;
    }
</style>