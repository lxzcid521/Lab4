<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Демонстрація використання тегів для роботи з формами">
    <meta name="keywords" content="теги, робота з формами, HTML">
    <title>Робота з формами</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            position: relative;
        }
        header {
            background-color: #051243;
            width: 100%;
            height: 120px;
            text-align: center;
            padding-top: 30px;
            color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            position: relative;
        }
        .panel {
            max-width: 1000px;
            text-align: left;
            position: absolute;
            left: 20px;
            top: 50%;
            transform: translateY(-50%);
        }
        .panel__title {
            font-size: larger;
        }
        .panel__links {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-top: 20px;
            position: relative;
        }
        .panel__links a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            margin-right: 20px;
            font-size: 18px;
        }
        .underline {
            position: absolute;
            width: 100%;
            bottom: 0;
            height: 2px;
            background-color: white;
        }
        .profile-icon {
            position: absolute;
            top: 50%;
            right: 20px;
            transform: translateY(-50%);
            height: 80px;
        }
        .photo-container {
            position: relative;
            text-align: center;
            margin-top: 0;
        }
        .photo-container img {
            width: 100%;
            height: auto;
        }
        .photo-text {
            position: absolute;
            top: 30%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            font-size: 32px;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        .line {
            position: absolute;
            width: 80%;
            height: 2px;
            background-color: white;
            bottom: 15%;
            left: 50%;
            transform: translateX(-50%);
        }
        .gallery {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            display: flex;
            justify-content: space-between;
            align-items: center;
            width: 80%;
        }
        .gallery img {
            width: 150px;
            height: 150px;
            object-fit: cover;
        }
        .artist-names {
            text-align: center;
            color: white;
            margin-top: 10px;
        }
        .artist-names a {
            color: white;
            text-decoration: none;
        }
        .view-all-button {
            margin-top: 40px; /* Новое значение отступа сверху */
            background-color: #051243;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            position: absolute; /* Добавлено */
            left: 50%; /* Добавлено */
            bottom: 10%; /* Новое значение отступа снизу */
            transform: translateX(-50%); /* Добавлено */
        }
        .start-button {
            background-color: #ffffff;
            color: rgb(0, 0, 0);
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            position: absolute;
            top: 90%;
            left: 50%;
            transform: translateX(-50%);
        }
        footer {
            background-color: #051243;
            color: white;
            padding: 20px 0;
            text-align: center;
            position: relative;
            margin-top: auto;
            display: flex;
            flex-direction: row;
        }
        .footer-panel {
            max-width: 1000px;
            margin: 0 auto;
        }
        .footer-title {
            font-size: larger;
        }
        .footer-links {
            margin-top: 20px;
        }
        .footer-links a {
            color: white;
            text-decoration: none;
            margin-left: 20px;
            margin-right: 20px;
            font-size: 18px;
            display: block;
            margin-bottom: 10px;
        }
        .footer-info {
            margin-top: 20px;
        }
    </style>
</head>
<body>
<header>
    <div class="panel">
        <div class="panel__title">YPLUGIN</div>
        <div class="panel__title">Buy FL Studio</div>
    </div>
    <div class="panel__links">
        <a href="#">Каталог</a>
        <a href="#">Створи</a>
        <a href="#">Свої Плагіни</a>
        <a href="#">Магазин</a>
        <a href="#">Підтримка</a>
        <div class="underline"></div>
    </div>
    <img src="c:\Users\lvxcid\Downloads\Account-Avatar-Profile-PNG-Photo.png" alt="Иконка профиля" class="profile-icon">
</header>
<div class="photo-container">
    <img src="c:\Users\lvxcid\Downloads\1866114.webp" alt="Фото">
    <div class="photo-text">Навчіться створювати власні плагіни для музики. Продавайте їх на нашому ринку, а також купуйте плагіни від популярних музикантів і малобюджетних виробників.</div>
</div>
<div class="photo-container">
    <div class="photo-text">Плагіни відомих музикантів</div>
    <div class="line"></div>
    <img src="c:\Users\lvxcid\Downloads\R (3).jfif" alt="second-photo">\
    <div class="gallery">
        <img src="c:\Users\lvxcid\Downloads\OIP (2).jfif" alt="photo1">
        <div class="artist-names"><a href="#">Martin Garix</a></div>
        <img src="c:\Users\lvxcid\Downloads\OIP (3).jfif" alt="photo2">
        <div class="artist-names"><a href="#">Kygo</a></div>
        <img src="c:\Users\lvxcid\Downloads\OIP (4).jfif" alt="photo3">
        <div class="artist-names"><a href="#">Kanye West</a></div>
        <img src="c:\Users\lvxcid\Downloads\OIP (5).jfif" alt="photo4">
        <div class="artist-names"><a href="#">Metro Boomin</a></div>
        <img src="c:\Users\lvxcid\Downloads\загрузка.jfif" alt="photo5">
        <div class="artist-names"><a href="#">Avicci</a></div>
    </div>
    <button class="view-all-button" style="bottom: 20%;">Подивитись усіх!</button> <!-- Кнопка внизу -->
</div>
<div class="photo-container">
    <img src="c:\Users\lvxcid\Downloads\image078-31-scaled.jpg" alt="Третя фотографія">
    <div class="photo-text">Почніть створювати свої плагіни прямо зараз і опубліковати їх (синтезатори, барабанні партії, бас, тощо)</div>
    <img src="c:\Users\lvxcid\Downloads\meilleurs-logiciels-de-studio-a-choisir-768x512.png" alt="Ваш текст зображення" style="width: 40%; position: absolute; top: 85%; left: 50%; transform: translate(-50%, -90%);">
    <button class="start-button" style="top: 93%;">Почати!</button>
</div>

</body>
<footer>
    <div class="footer-panel">
        <div class="footer-title">Контакти</div>
        <div class="footer-info">
            <p>(093)135-25-44</p>
            <p>(094)000-00-00</p>
            <p>(095)000-00-00</p>
        </div>
    </div>
    <div class="footer-panel">
        <div class="footer-title">YPLUGIN</div>
        <div class="footer-title">Copyright Ⓒ 2022</div>
        </div>
    <div class="footer-panel">
        <div class="footer-title">Інформація</div>
        <div class="footer-links">
            <a href="#">Про нас</a>
            <a href="#">Хіт продажу</a>
            <a href="#">Відгуки</a>
        </div>
    </div>
</footer>
</html>

