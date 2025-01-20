<!DOCTYPE html>
<html lang="sk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Oravská Polhora</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }

        .video-background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            object-fit: cover;
        }

        .hidden {
            display: none;
        }

        .flag-container {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 10px;
        }

        .flag-container img {
            width: 30px;
            height: 20px;
            cursor: pointer;
        }

        .image-container {
            position: relative;
            display: block;
        }

        .image-container img, .image-container iframe {
            width: 100%;
            height: 200px;
            transition: opacity 0.3s ease;
        }

        .image-container img {
            object-fit: cover;
        }

        .image-container:hover img {
            opacity: 0;
        }

        .image-container:hover iframe {
            opacity: 1;
        }

        .image-container iframe {
            opacity: 0;
            border: 0;
            position: absolute;
            top: 0;
            left: 0;
        }

        .lang-text {
            text-align: center;
            margin-top: 10px;
        }

        /* Styling for the video in the bottom right corner */
        .video-iframe {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 400px;
            height: 225px;
            border: none;
            z-index: 10;
        }
    </style>
    <script>
        function changeLanguage(lang) {
            // Hide all language sections
            document.querySelectorAll('.lang').forEach(function(element) {
                element.classList.add('hidden');
            });

            // Show the selected language
            document.querySelectorAll(`.lang-${lang}`).forEach(function(element) {
                element.classList.remove('hidden');
            });
        }

        window.onload = function() {
            // Set the default language to Slovak
            changeLanguage('sk');
        };
    </script>
</head>
<body class="bg-gray-100 font-sans leading-normal tracking-normal">

    <!-- Video Background -->
    <video class="video-background" autoplay loop muted>
        <source src="https://www.youtube.com/watch?v=s7H_0heCNgo" type="video/mp4">
        Váš prehliadač nepodporuje prehrávanie videí.
    </video>

    <!-- Header -->
    <header class="bg-green-700 text-white py-6">
        <div class="container mx-auto text-center">
            <h1 class="text-4xl font-bold lang lang-sk">Vitajte v Oravskej Polhore</h1>
            <h1 class="text-4xl font-bold lang lang-en hidden">Welcome to Oravská Polhora</h1>
            <h1 class="text-4xl font-bold lang lang-hu hidden">Üdvözöljük Oravská Polhora-ban</h1>
            <h1 class="text-4xl font-bold lang lang-pl hidden">Witaj w Oravská Polhora</h1>
            <p class="text-lg mt-2 lang lang-sk">Najsevernejšia obec Slovenska</p>
            <p class="text-lg mt-2 lang lang-en hidden">The northernmost village of Slovakia</p>
            <p class="text-lg mt-2 lang lang-hu hidden">Szlovákia legészakibb falva</p>
            <p class="text-lg mt-2 lang lang-pl hidden">Najbardziej na północ wysunięta wioska Słowacji</p>

            <!-- Language Flags -->
            <div class="flag-container">
                <img src="https://cdn.pixabay.com/photo/2015/11/06/13/29/union-jack-1027898_1280.jpg" alt="English" title="English" onclick="changeLanguage('en')">
                <img src="https://cdn.britannica.com/55/1455-050-CCDFFCF0/Flag-Hungary.jpg" alt="Hungarian" title="Hungarian" onclick="changeLanguage('hu')">
                <img src="https://www.buyflags.eu/sites/default/files/styles/colorbox_full/public/flags-image/polskokopie.png?itok=dk9-wAP9" alt="Polish" title="Polish" onclick="changeLanguage('pl')">
                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRBM_ClbvlcfeClH-5E-1ugxryXtz3JYo1dvA&s" alt="Slovak" title="Slovak" onclick="changeLanguage('sk')">
            </div>
        </div>
    </header>

    <!-- Divider Image -->
    <section>
        <img src="https://lh3.googleusercontent.com/p/AF1QipN-Ku8HoR9oXMaqU6hXyoXAhxjsuXGLihQEv9yK=s1360-w1360-h1020" alt="Oravská Polhora Scenery" class="w-full h-auto">
    </section>

    <!-- About Section -->
    <section id="about" class="py-8 px-4">
        <div class="container mx-auto">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4 lang lang-sk">O dedine</h2>
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4 lang lang-en hidden">About the village</h2>
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4 lang lang-hu hidden">A faluról</h2>
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4 lang lang-pl hidden">O wiosce</h2>

            <p class="text-gray-700 text-lg text-center lang lang-sk">
                Oravská Polhora je malá dedinka na severnom okraji Slovenska, ktorá vás očarí svojou prírodnou krásou a pokojnou atmosférou.
            </p>
            <p class="text-gray-700 text-lg text-center lang lang-en hidden">
                Oravská Polhora is a small village on the northern edge of Slovakia, charming with its natural beauty and peaceful atmosphere.
            </p>
            <p class="text-gray-700 text-lg text-center lang lang-hu hidden">
                Oravská Polhora egy kis falu Szlovákia északi szélén, amely elbűvöli Önt természeti szépségével.
            </p>
            <p class="text-gray-700 text-lg text-center lang lang-pl hidden">
                Oravská Polhora to mała wieś na północnej krawędzi Słowacji, która oczaruje Cię swoją naturalną urodą.
            </p>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="py-8 px-4 bg-gray-50">
        <div class="container mx-auto">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-sk">Fotogaléria</h2>
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-en hidden">Gallery</h2>
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-hu hidden">Galéria</h2>
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-pl hidden">Galeria</h2>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                <!-- Image 1 -->
                <div class="image-container bg-gray-200 p-4 rounded-lg">
                    <img src="https://lh5.googleusercontent.com/p/AF1QipP4nhhrDAkcpqah6kN3opNJdex2vqlqBjL17EDd=w675-h390-n-k-no" alt="Obrázok 1">
                    <iframe src="https://www.openstreetmap.org/export/embed.html?bbox=19.4628%2C49.5116%2C19.5494%2C49.5566&layer=mapnik&marker=49.5340%2C19.5060" allowfullscreen></iframe>
                    <div class="lang-text lang lang-sk">Hviezdoslavova Hájovňa</div>
                    <div class="lang-text lang lang-en hidden">Hviezdoslavova Hájovňa</div>
                    <div class="lang-text lang lang-hu hidden">Hviezdoslavova Hájovňa</div>
                    <div class="lang-text lang lang-pl hidden">Hviezdoslavova Hájovňa</div>
                </div>
                <!-- Image 2 -->
                <div class="image-container bg-gray-200 p-4 rounded-lg">
                    <img src="https://lh5.googleusercontent.com/p/AF1QipPI4tsM0M4eruO7MTdpTjh15owj-0ZtaVZS7J0n=w675-h390-n-k-no" alt="Obrázok 2">
                    <iframe src="https://www.openstreetmap.org/export/embed.html?bbox=19.4683%2C49.5232%2C19.4788%2C49.5288&layer=mapnik&marker=49.5262%2C19.4730" allowfullscreen></iframe>
                    <div class="lang-text lang lang-sk">Babia Hora</div>
                    <div class="lang-text lang lang-en hidden">Babia Hora</div>
                    <div class="lang-text lang lang-hu hidden">Babia Hora</div>
                    <div class="lang-text lang lang-pl hidden">Babia Hora</div>
                </div>
                <!-- Image 3 -->
                <div class="image-container bg-gray-200 p-4 rounded-lg">
                    <img src="https://lh5.googleusercontent.com/p/AF1QipPw1OnbBY9PgtSiTfoRN9EvhBLySIysaP8envs6=w675-h390-n-k-no" alt="Obrázok 3">
                    <iframe src="https://www.openstreetmap.org/export/embed.html?bbox=19.4532%2C49.5322%2C19.4735%2C49.5443&layer=mapnik&marker=49.5373%2C19.4632" allowfullscreen></iframe>
                    <div class="lang-text lang lang-sk">Chata Slaná Voda</div>
                    <div class="lang-text lang lang-en hidden">Chata Slaná Voda</div>
                    <div class="lang-text lang lang-hu hidden">Chata Slaná Voda</div>
                    <div class="lang-text lang lang-pl hidden">Chata Slaná Voda</div>
                </div>

                <!-- Image 4 -->
                <div class="image-container bg-gray-200 p-4 rounded-lg">
                    <img src="https://www.euroregion-tatry.sk/images/pamiatky/1679521368.jpg" alt="Obrázok 4">
                    <iframe src="https://osm.org/go/0La2xGcGt--?relation=2166354" allowfullscreen></iframe>
                    <div class="lang-text lang lang-sk">Rozhľadňa</div>
                    <div class="lang-text lang lang-en hidden">Rozhľadňa</div>
                    <div class="lang-text lang lang-hu hidden">Rozhľadňa</div>
                    <div class="lang-text lang lang-pl hidden">Rozhľadňa</div>
                </div>

                <!-- Image 5 -->
                <div class="image-container bg-gray-200 p-4 rounded-lg">
                    <img src="https://www.skioravskapolhora.sk/wp-content/uploads/2022/01/FDB1E8A3-0793-42F2-84C1-72662080422D.jpeg" alt="Obrázok 5">
                    <iframe src="https://osm.org/go/0La2VimhF-?relation=2166354" allowfullscreen></iframe>
                    <div class="lang-text lang lang-sk">Vlek</div>
                    <div class="lang-text lang lang-en hidden">Ski resort</div>
                    <div class="lang-text lang lang-hu hidden">Vlek</div>
                    <div class="lang-text lang lang-pl hidden">Vlek</div>
                </div>

                <!-- Image 6 -->
                <div class="image-container bg-gray-200 p-4 rounded-lg">
                    <img src="https://lh3.googleusercontent.com/p/AF1QipMOdsSx1y316obnbIWFxjxdaKp6L7kZ5f5vFYm9=s1360-w1360-h1020" alt="Obrázok 6">
                    <iframe src="https://www.openstreetmap.org/#map=15/49.55995/19.43911" allowfullscreen></iframe>
                    <div class="lang-text lang lang-sk">Rašeliniská</div>
                    <div class="lang-text lang lang-en hidden">Swamps</div>
                    <div class="lang-text lang lang-hu hidden">Rašeliniská</div>
                    <div class="lang-text lang lang-pl hidden">Rašeliniská</div>
                </div>
            </div>
        </div>
    </section>

   <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> História Oravskej Polhory</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f1f5f9;
            margin: 0;
            padding: 0;
        }

        .timeline {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 50px auto;
            position: relative;
            max-width: 1200px;
            padding: 30px 0;
        }

        .timeline::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 0;
            width: 100%;
            height: 4px;
            background-color: #d1d5db;
            transform: translateY(-50%);
            z-index: 0;
        }

        .timeline-item {
            position: relative;
            z-index: 1;
            width: 120px;
            text-align: center;
        }

        .timeline-item .tooltip {
            visibility: hidden;
            background-color: #ffffff;
            color: #333;
            text-align: center;
            border-radius: 6px;
            padding: 10px;
            position: absolute;
            top: 120%;
            left: 50%;
            transform: translateX(-50%);
            opacity: 0;
            transition: opacity 0.3s, transform 0.3s;
            width: 250px;
            font-size: 0.9rem;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .timeline-item:hover .tooltip {
            visibility: visible;
            opacity: 1;
            transform: translateY(10px);
        }

        .timeline-item .dot {
            width: 30px;
            height: 30px;
            background-color: #48bb78;
            border-radius: 50%;
            margin: 0 auto;
            cursor: pointer;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .timeline-item:hover .dot {
            transform: scale(1.2);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
        }

        .timeline-item h2 {
            margin-top: 10px;
            font-size: 1.1rem;
            font-weight: bold;
            color: #4a5568;
        }

        .timeline-item p {
            font-size: 1rem;
            color: #4a5568;
            margin-top: 5px;
        }

        .timeline-item .dot::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 10px;
            height: 10px;
            background-color: #fff;
            border-radius: 50%;
            transform: translate(-50%, -50%);
            box-shadow: 0 0 0 4px #48bb78;
        }
    </style>
<header class="bg-green-700 text-white py-6">
    <div class="container mx-auto text-center">
        <h1 class="text-4xl font-bold lang lang-sk">História Oravskej Polhory</h1>
        <h1 class="text-4xl font-bold lang lang-en hidden">History of Oravská Polhora</h1>
        <h1 class="text-4xl font-bold lang lang-hu hidden">Oravská Polhora idővonala</h1>
        <h1 class="text-4xl font-bold lang lang-pl hidden">Oś czasu Oravská Polhora</h1>
    </div>
</header>
<section class="timeline">
    <div class="timeline-item">
        <div class="dot"></div>
        <div class="tooltip">
            <h2 class="lang lang-sk">1588</h2>
            <h2 class="lang lang-en hidden">1588</h2>
            <h2 class="lang lang-hu hidden">1588</h2>
            <h2 class="lang lang-pl hidden">1588</h2>
            <p class="lang lang-sk">Prvá písomná zmienka o Oravskej Polhore.</p>
            <p class="lang lang-en hidden">First written mention of Oravská Polhora.</p>
            <p class="lang lang-hu hidden">Az első írásos említés Oravská Polhora-ról.</p>
            <p class="lang lang-pl hidden">Pierwsza wzmianka pisemna o Oravskiej Polhorze.</p>
        </div>
    </div>

    <div class="timeline-item">
        <div class="dot"></div>
        <div class="tooltip">
            <h2 class="lang lang-sk">17. storočie</h2>
            <h2 class="lang lang-en hidden">17th century</h2>
            <h2 class="lang lang-hu hidden">17. század</h2>
            <h2 class="lang lang-pl hidden">XVII wiek</h2>
            <p class="lang lang-sk">Postavená hájovňa, neskôr nazývaná Hviezdoslavova.</p>
            <p class="lang lang-en hidden">Creation of Hviezdoslav's lodge.</p>
            <p class="lang lang-hu hidden">Hviezdoslav-kunyhó létrehozása.</p>
            <p class="lang lang-pl hidden">Powstanie chaty Hviezdoslava.</p>
        </div>
    </div>

    <div class="timeline-item">
        <div class="dot"></div>
        <div class="tooltip">
            <h2 class="lang lang-sk">19. storočie</h2>
            <h2 class="lang lang-en hidden">19th century</h2>
            <h2 class="lang lang-hu hidden">19. század</h2>
            <h2 class="lang lang-pl hidden">XIX wiek</h2>
            <p class="lang lang-sk">Hviezdoslav nachádza inšpiráciu v okolitej prírode.</p>
            <p class="lang lang-en hidden">Hviezdoslav finds inspiration in the surrounding nature.</p>
            <p class="lang lang-hu hidden">Hviezdoslav ihletet talál a környező természetben.</p>
            <p class="lang lang-pl hidden">Hviezdoslav znajduje inspirację w okolicznej przyrodzie.</p>
        </div>
    </div>

    <div class="timeline-item">
        <div class="dot"></div>
        <div class="tooltip">
            <h2 class="lang lang-sk">1963</h2>
            <h2 class="lang lang-en hidden">1963</h2>
            <h2 class="lang lang-hu hidden">1963</h2>
            <h2 class="lang lang-pl hidden">1963</h2>
            <p class="lang lang-sk">Vyhlásenie Chránenej krajinnej oblasti Horná Orava.</p>
            <p class="lang lang-en hidden">Declaration of the Horná Orava Protected Landscape Area.</p>
            <p class="lang lang-hu hidden">A Horná Orava védett tájegység kijelentése.</p>
            <p class="lang lang-pl hidden">Ogłoszenie Chránenej krajinnej oblasti Horná Orava.</p>
        </div>
    </div>

    <div class="timeline-item">
        <div class="dot"></div>
        <div class="tooltip">
            <h2 class="lang lang-sk">1981</h2>
            <h2 class="lang lang-en hidden">1981</h2>
            <h2 class="lang lang-hu hidden">1981</h2>
            <h2 class="lang lang-pl hidden">1981</h2>
            <p class="lang lang-sk">Rekonštrukcia Hviezdoslavovej hájovne.</p>
            <p class="lang lang-en hidden">Reconstruction of Hviezdoslav's lodge.</p>
            <p class="lang lang-hu hidden">Hviezdoslav-kunyha rekonstrukciója.</p>
            <p class="lang lang-pl hidden">Rekonstrukcja chaty Hviezdoslava.</p>
        </div>
    </div>

    <div class="timeline-item">
        <div class="dot"></div>
        <div class="tooltip">
            <h2 class="lang lang-sk">2008</h2>
            <h2 class="lang lang-en hidden">2008</h2>
            <h2 class="lang lang-hu hidden">2008</h2>
            <h2 class="lang lang-pl hidden">2008</h2>
            <p class="lang lang-sk">Oslava 420. výročia obce.</p>
            <p class="lang lang-en hidden">Celebration of the 420th anniversary of the village.</p>
            <p class="lang lang-hu hidden">Az falu 420. évfordulójának ünneplése.</p>
            <p class="lang lang-pl hidden">Obchody 420-lecia wioski.</p>
        </div>
    </div>
</section>
</body>





            <!-- Prázdne riadky --><!-- Akcie v dedine -->
<section id="events" class="py-8 px-4 bg-gray-50">
    <div class="container mx-auto">
        <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-sk">Akcie v dedine</h2>
        <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-en hidden">Events in the village</h2>
        <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-hu hidden">Rendezvények a faluban</h2>
        <h2 class="text-3xl font-bold text-center text-gray-800 mb-8 lang lang-pl hidden">Wydarzenia w wiosce</h2>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
            <!-- Event 1 -->
            <div class="bg-white shadow-lg rounded-lg p-6">
                <h3 class="text-xl font-semibold text-gray-800 lang lang-sk">Odber krvi</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-en hidden">Blood Donation</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-hu hidden">Véradás</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-pl hidden">Oddawanie krwi</h3>
                <p class="text-gray-600 lang lang-sk">20. januára 2025 v obci Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-en hidden">January 20, 2025, in Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-hu hidden">2025. január 20-án, Oravská Polhorában.</p>
                <p class="text-gray-600 lang lang-pl hidden">20 stycznia 2025 roku w Oravskiej Polhorze.</p>
            </div>

            <!-- Event 2 -->
            <div class="bg-white shadow-lg rounded-lg p-6">
                <h3 class="text-xl font-semibold text-gray-800 lang lang-sk">Ples športovcov</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-en hidden">Sportsmen's Ball</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-hu hidden">Sportoló bál</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-pl hidden">Bal sportowców</h3>
                <p class="text-gray-600 lang lang-sk">1. februára 2025 v obci Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-en hidden">February 1, 2025, in Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-hu hidden">2025. február 1-jén, Oravská Polhorában.</p>
                <p class="text-gray-600 lang lang-pl hidden">1 lutego 2025 roku w Oravskiej Polhorze.</p>
            </div>

            <!-- Event 3 -->
            <div class="bg-white shadow-lg rounded-lg p-6">
                <h3 class="text-xl font-semibold text-gray-800 lang lang-sk">Maškarný ples</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-en hidden">Masquerade Ball</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-hu hidden">Álarcos bál</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-pl hidden">Bal maskowy</h3>
                <p class="text-gray-600 lang lang-sk">8. februára 2025 v obci Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-en hidden">February 8, 2025, in Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-hu hidden">2025. február 8-án, Oravská Polhorában.</p>
                <p class="text-gray-600 lang lang-pl hidden">8 lutego 2025 roku w Oravskiej Polhorze.</p>
            </div>

            <!-- Event 4 -->
            <div class="bg-white shadow-lg rounded-lg p-6">
                <h3 class="text-xl font-semibold text-gray-800 lang lang-sk">Seleziansky ples</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-en hidden">Salesian Ball</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-hu hidden">Szaleziánus bál</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-pl hidden">Bal salezjański</h3>
                <p class="text-gray-600 lang lang-sk">15. februára 2025 v obci Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-en hidden">February 15, 2025, in Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-hu hidden">2025. február 15-én, Oravská Polhorában.</p>
                <p class="text-gray-600 lang lang-pl hidden">15 lutego 2025 roku w Oravskiej Polhorze.</p>
            </div>

            <!-- Event 5 -->
            <div class="bg-white shadow-lg rounded-lg p-6">
                <h3 class="text-xl font-semibold text-gray-800 lang lang-sk">Gajdovačka (19.9.2025 - 21.9.2025)</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-en hidden">Gajdovačka (19.9.2025 - 21.9.2025)</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-hu hidden">Gajdovačka (19.9.2025 - 21.9.2025)</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-pl hidden">Gajdovačka (19.9.2025 - 21.9.2025)</h3>
                <p class="text-gray-600 lang lang-sk">19. - 21. septembra 2025 v obci Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-en hidden">September 19 - 21, 2025, in Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-hu hidden">2025. szeptember 19-21-ig, Oravská Polhorában.</p>
                <p class="text-gray-600 lang lang-pl hidden">19 - 21 września 2025 roku w Oravskiej Polhorze.</p>
            </div>

            <!-- Event 6 -->
            <div class="bg-white shadow-lg rounded-lg p-6">
                <h3 class="text-xl font-semibold text-gray-800 lang lang-sk">Gajdovačka (18.9.2026 - 20.9.2026)</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-en hidden">Gajdovačka (18.9.2026 - 20.9.2026)</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-hu hidden">Gajdovačka (18.9.2026 - 20.9.2026)</h3>
                <h3 class="text-xl font-semibold text-gray-800 lang lang-pl hidden">Gajdovačka (18.9.2026 - 20.9.2026)</h3>
                <p class="text-gray-600 lang lang-sk">18. - 20. septembra 2026 v obci Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-en hidden">September 18 - 20, 2026, in Oravská Polhora.</p>
                <p class="text-gray-600 lang lang-hu hidden">2026. szeptember 18-20-ig, Oravská Polhorában.</p>
                <p class="text-gray-600 lang lang-pl hidden">18 - 20 września 2026 roku w Oravskiej Polhorze.</p>
            </div>
        </div>
    </div>
</section>
 
   <!-- Kontaktné údaje a práva -->
    <section class="bg-gray-800 text-white py-8">
        <div class="container mx-auto text-center">
            <p>&copy; 2024 Oravská Polhora. Všetky práva vyhradené.</p>
            <p>Email: <a href="mailto:info@oravskapolhora.sk" class="text-blue-300">info@oravskapolhora.sk</a></p>
            <p>Telefón: +421 912 345 678</p>

            <!-- Made by text -->
            <p class="mt-4">Made by Martin Skurčák</p>
            <div class="mt-6">
                <p>&nbsp;</p>
                <p>&nbsp;</p>
                <p>&nbsp;</p> <!-- Pridaný ďalší prázdny riadok -->
            </div>
        </div>
    </section>

 <!-- YouTube Video in the Bottom Right Corner -->
    <iframe class="video-iframe" src="https://www.youtube.com/embed/s7H_0heCNgo?autoplay=1&mute=1" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</body>
</html>
