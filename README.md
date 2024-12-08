1-қадам: HTML файлын жасау
1. Компьютеріңізде кез келген мәтіндік редакторды ашыңыз (мысалы, Notepad, VS Code, Sublime Text).
2. Жаңа файл жасап, оны index.html деп сақтаңыз. 
   - Файлды .html кеңейтімімен сақтау керек.


2-қадам: HTML құрылымын жасау
HTML файлында барлық сайтқа қажет негізгі құрылымды жазамыз. Бұл барлық HTML құжаттары үшін стандартты.

html
<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Бұл сайт физика тақырыбы бойынша қазақ тілінде ақпарат береді.">
    <meta name="keywords" content="физика, қазақша физика, ғылым">
    <meta name="author" content="Сіздің атыңыз">
    <title>Физика туралы</title>
</head>
<body>
    <h1>Физика туралы сайт</h1>
    <p>Бұл сайтта физика ғылымы туралы қазақ тілінде пайдалы ақпарат таба аласыз.</p>
</body>
</html>


- <head> бөлімі*: Бет атауы мен мета-тегтерді енгізу үшін қолданылады.
- <body> бөлімі*: Сайттың негізгі мазмұны осында жазылады.


3-қадам: Сайттың құрылымын толықтыру
HTML-ге қосымша элементтер қосып, мазмұнды байытамыз.

html
<!DOCTYPE html>
<html lang="kk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Бұл сайт физика тақырыбы бойынша қазақ тілінде ақпарат береді.">
    <meta name="keywords" content="физика, қазақша физика, ғылым">
    <meta name="author" content="Сіздің атыңыз">
    <title>Физика туралы</title>
</head>
<body>
    <header>
        <h1>Физика туралы</h1>
        <nav>
            <ul>
                <li><a href="#about">Физика жайлы</a></li>
                <li><a href="#topics">Тақырыптар</a></li>
                <li><a href="#contact">Байланыс</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>Физика жайлы</h2>
        <p>Физика – табиғатты зерттейтін ғылым. Ол әлемдегі құбылыстарды түсіндіруге арналған заңдарды зерттейді.</p>
    </section>

    <section id="topics">
        <h2>Тақырыптар</h2>
        <ul>
            <li>Механика</li>
            <li>Электр және магнетизм</li>
            <li>Оптика</li>
            <li>Термодинамика</li>
        </ul>
    </section>

    <footer id="contact">
        <h2>Байланыс</h2>
        <p>Сұрақтарыңыз болса, бізге <a href="mailto:example@email.com">жазыңыз</a>.</p>
    </footer>
</body>
</html>


- <header>: Бұл жерде сайттың тақырыбы мен мәзірі орналасады.
- <section>: Сайттың әрбір бөлігін көрсету үшін қолданылады.
- <footer>: Байланыс ақпаратын қосу үшін.

4-қадам: Сайт дизайнын жақсарту (CSS қосу)
Сіз дизайнды жақсарту үшін CSS қолдана аласыз. HTML-ге CSS қосудың үш жолы бар:
1. Ішкі стильдер (HTML файлына жазылады).
2. Сыртқы CSS файл жасау (ұсынылады).
3. HTML элементтеріне тікелей стиль беру.

Мысал: Ішкі CSS қосу
html
<head>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
        }
        section {
            margin: 20px;
            padding: 20px;
            background: white;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background: #333;
            color: white;
        }
    </style>
</head>


Бұл стильдер сайтты заманауи әрі ыңғайлы етеді.

5-қадам: Файлды браузерде ашу
1. Сақтау:HTML кодты сақтаңыз.
2. Файлды браузерде ашу үшін оған екі рет басыңыз немесе файлды браузерге сүйреп апарыңыз.
3. Браузерде сайт ашылады.
