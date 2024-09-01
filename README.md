<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Artículos sobre Videojuegos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #000000;
            color: #ffffff;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #000000;
            padding: 15px 20px;
            text-align: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid #333333;
        }

        header h1 {
            margin: 0;
            color: #ffffff;
            font-size: 1.8rem;
        }

        main {
            margin-top: 80px;
            padding: 20px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .article {
            background-color: #121212;
            padding: 15px;
            margin-bottom: 20px;
            border-radius: 5px;
            border: 1px solid #333333;
        }

        .article img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
            margin-bottom: 10px;
        }

        .article h2 {
            color: #ffffff;
            margin-top: 0;
        }

        .article p {
            line-height: 1.6;
        }

        .like-button {
            display: inline-block;
            color: #00ffcc;
            text-decoration: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .like-count {
            margin-left: 5px;
            color: #00ffcc;
        }

        .admin-options {
            display: none;
            margin-top: 10px;
            text-align: right;
        }

        .admin-options a {
            color: #00ffcc;
            text-decoration: none;
            margin-right: 10px;
            cursor: pointer;
        }

        .link-container {
            margin-top: 20px;
            text-align: center;
        }

        .link-container a {
            color: #00ffcc;
            text-decoration: none;
            padding: 10px 20px;
            border: 1px solid #00ffcc;
            border-radius: 5px;
            display: inline-block;
            margin: 5px;
        }

        .ad-space {
            background-color: #121212;
            padding: 20px;
            text-align: center;
            margin-top: 40px;
            border-radius: 5px;
            color: #00ffcc;
            border: 1px solid #333333;
        }

        .language-switcher {
            position: fixed;
            top: 15px;
            left: 20px;
            color: #00ffcc;
            cursor: pointer;
            font-size: 0.9rem;
        }

        .cookie-banner {
            position: fixed;
            bottom: 0;
            width: 100%;
            background-color: #121212;
            color: #ffffff;
            padding: 15px;
            text-align: center;
            z-index: 1001;
            border-top: 1px solid #333333;
        }

        .cookie-banner button {
            background-color: #00ffcc;
            color: #000000;
            padding: 8px 15px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.9rem;
        }

        .redirect-button {
            background-color: #00ffcc;
            color: #000000;
            padding: 15px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            display: block;
            width: 200px;
            margin: 40px auto;
            text-align: center;
            text-decoration: none;
            font-size: 1rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>Artículos sobre Videojuegos</h1>
    </header>

    <div class="language-switcher" onclick="switchLanguage()">Cambiar a Inglés</div>

    <main id="main-content">
        <article class="article" id="article1">
            <img src="https://via.placeholder.com/800x400" alt="Imagen del Artículo">
            <h2>El Impacto de los Videojuegos en la Cultura Moderna</h2>
            <p>Los videojuegos han influenciado la cultura popular de maneras inimaginables, desde el cine hasta la música y la moda. Su influencia es innegable y sigue creciendo.</p>
            <a class="like-button" onclick="likeArticle('article1')">Me gusta</a><span class="like-count" id="likes-article1">0</span>
            <div class="admin-options" id="admin1">
                <a onclick="editArticle('article1')">Editar</a>
                <a onclick="deleteArticle('article1')">Eliminar</a>
            </div>
        </article>

        <article class="article" id="article2">
            <img src="https://via.placeholder.com/800x400" alt="Imagen del Artículo">
            <h2>Los Mejores Juegos de 2024</h2>
            <p>El año 2024 ha sido un año excepcional para los videojuegos, con lanzamientos que han superado las expectativas y han marcado un nuevo estándar en la industria.</p>
            <a class="like-button" onclick="likeArticle('article2')">Me gusta</a><span class="like-count" id="likes-article2">0</span>
            <div class="admin-options" id="admin2">
                <a onclick="editArticle('article2')">Editar</a>
                <a onclick="deleteArticle('article2')">Eliminar</a>
            </div>
        </article>

        <article class="article" id="article3">
            <img src="https://via.placeholder.com/800x400" alt="Imagen del Artículo">
            <h2>La Evolución de los eSports</h2>
            <p>Los eSports han pasado de ser un nicho a convertirse en un fenómeno global, con millones de seguidores y competencias que rivalizan con los deportes tradicionales en audiencia.</p>
            <a class="like-button" onclick="likeArticle('article3')">Me gusta</a><span class="like-count" id="likes-article3">0</span>
            <div class="admin-options" id="admin3">
                <a onclick="editArticle('article3')">Editar</a>
                <a onclick="deleteArticle('article3')">Eliminar</a>
            </div>
        </article>

        <div class="ad-space">
            Espacio Publicitario
        </div>

        <div class="link-container">
            <a href="#">Ver más artículos</a>
            <a href="#">Suscribirse</a>
        </div>
    </main>

    <div class="cookie-banner">
        Este sitio utiliza cookies para mejorar tu experiencia. <button onclick="acceptCookies()">Aceptar</button>
    </div>

    <script>
        function switchLanguage() {
            // Función para cambiar el idioma
        }

        function likeArticle(articleId) {
            // Función para agregar un like al artículo
            const likesSpan = document.getElementById(`likes-${articleId}`);
            let currentLikes = parseInt(likesSpan.textContent);
            likesSpan.textContent = currentLikes + 1;
        }

        function editArticle(articleId) {
            // Función para editar el artículo (solo para administradores)
            alert(`Editar artículo: ${articleId}`);
        }

        function deleteArticle(articleId) {
            // Función para eliminar el artículo (solo para administradores)
            const articleElement = document.getElementById(articleId);
            articleElement.remove();
        }

        function acceptCookies() {
            // Función para aceptar cookies
            const cookieBanner = document.querySelector('.cookie-banner');
            cookieBanner.style.display = 'none';
        }
    </script>
</body>
</html>
