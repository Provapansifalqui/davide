<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu Insuflaggi Stondato</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            position: relative;
            width: 100%;
            background-color: #333;
            color: #fff;
            padding: 10px;
        }

        .hamburger-menu {
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            width: 30px;
            height: 25px;
            cursor: pointer;
        }

        .bar {
            width: 100%;
            height: 4px;
            background-color: #fff;
            border-radius: 30px;
        }

        .menu {
            display: none;
            position: absolute;
            top: 50px;
            right: 10px;
            background-color: #333;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            border-radius: 30px;
            overflow: hidden;
            width: 200px;
        }

        .menu.active {
            display: block;
        }

        .menu ul {
            list-style: none;
            margin: 0;
            padding: 0;
        }

        .menu ul li {
            padding: 15px;
            text-align: center;
            border-bottom: 1px solid #444;
        }

        .menu ul li:last-child {
            border-bottom: none;
        }

        .menu ul li a {
            text-decoration: none;
            color: #fff;
            display: block;
        }

        .menu ul li a:hover {
            background-color: #575757;
        }
    </style>
</head>
<body>
    <header>
        <div class="hamburger-menu" onclick="toggleMenu()">
            <div class="bar"></div>
            <div class="bar"></div>
            <div class="bar"></div>
        </div>
        <nav class="menu">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Chi Siamo</a></li>
                <li><a href="#">Servizi</a></li>
                <li><a href="#">Progetti</a></li>
                <li><a href="#">Contatti</a></li>
            </ul>
        </nav>
    </header>

    <script>
        function toggleMenu() {
            const menu = document.querySelector('.menu');
            menu.classList.toggle('active');
        }
    </script>
</body>
</html>

