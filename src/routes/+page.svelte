<head>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
</head>

<script>
    import photoEnzo from '$lib/images/image_accueil_navbar.png';
    import iconGithub from '$lib/images/logo_github.svg';
    import iconLinkedin from '$lib/images/logo_linkedin.svg';
    import iconMail from '$lib/images/logo_mail.svg';
</script>
<body>
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
<div class="Presentation">
    <h2 class="presentationh2">Bonjour, je suis</h2>
    <h1 class="presentationh1">Enzo Duval</h1>
    <h2 class="presentationh3">Développeur FullStack</h2>
</div>
<div class="Icon-container">
    <div class="icon">
        <img src={iconMail} alt="Icon Mail"/>
    </div>
    <div class="icon">
        <img src={iconGithub} alt="Icon Github"/>
    </div>
    <div class="icon">
        <img src={iconLinkedin} alt="Icon Linkedin"/>
    </div>
</div>
</body>

<style>
    body {
        font-family: Montserrat, sans-serif;
    }

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

    .Presentation {
        color: #002333;
        margin-top: 10%;
    }

    .presentationh1 {
        font-size: 300%;
        margin-left: 20%;
    }

    .presentationh2 {
        font-size: 150%;
        font-weight: 600;
        margin-left: 22%;
    }

    .presentationh3 {
        font-weight: 600;
        font-size: 150%;
        color: #B4BEC9;
        margin-left: 20%;
    }

    .Icon-container {
        display: flex;
        justify-content: flex-start;
        gap: 20px; /* Espace entre les icônes */
        margin-left: 22%;
        margin-top: 2%;
    }

  
    .icon img {
        width: 40px;
        height: 40px;
        transition: transform 0.2s ease;
    }


    .icon img:hover {
        transform: scale(1.2);
    }

</style>