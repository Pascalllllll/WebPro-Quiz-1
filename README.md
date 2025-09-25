# WebPro-Quiz-1

## 1. Website Development Project

For this quiz, you will build a **static personal website** using **HTML, CSS, and JavaScript**.  
You are free to use libraries and frameworks like **jQuery** or **Bootstrap** for layout and styling.

---

### A. Website Content
Your website must include the following pages/sections:
- **[Homepage](#homepage)**: The main landing page.
- **[Profile](#profile)**: Information about yourself.
- **[Hometown](#hometown)**: A brief description of your hometown.
- **[Local Food](#local-food)**: A feature on local food from your hometown.
- **[Tourist Places](#tourist-places)**: A guide to tourist attractions in your hometown.

---

### B. Page Routing
The URL structure for your pages must follow this format:
```
quiz1/
├── index.html
├── style.css
├── script.js
│
├── img/
│   └── (gambar-gambar)
│
├── profile/
│   └── index.html
│
├── hometown/
│   └── index.html
│
├── food/
│   └── index.html
│
└── tourist/
    └── index.html
```
---
### You Can Access My Website From the Link Below
#### https://pascalllllll.github.io/quiz1/ target="_blank"

---

## Homepage
```index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="/quiz1/style.css" />
    <link rel="icon" type="image/png" href="/quiz1/img/avatar.png" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" />
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet" />
</head>

<body>
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
        <label class="switch">
            <input type="checkbox" id="darkToggle">
            <span class="slider"></span>
        </label>
    </header>

    <main class="center">
        <a href="#" class="sparkle-button" id="hfs">
            <svg viewBox="0 0 96 96"><path d="M93.781 51.578C95 50.969 96 49.359 96 48c0-1.375-1-2.969-2.219-3.578 0 0-22.868-1.514-31.781-10.422-8.915-8.91-10.438-31.781-10.438-31.781C50.969 1 49.375 0 48 0s-2.969 1-3.594 2.219c0 0-1.5 22.87-10.406 31.781-8.908 8.913-31.781 10.422-31.781 10.422C1 45.031 0 46.625 0 48c0 1.359 1 2.969 2.219 3.578 0 0 22.873 1.51 31.781 10.422 8.906 8.911 10.406 31.781 10.406 31.781C45.031 95 46.625 96 48 96s2.969-1 3.562-2.219c0 0 1.523-22.871 10.438-31.781 8.913-8.908 31.781-10.422 31.781-10.422Z" fill="#000" /></svg>
            <svg viewBox="0 0 96 96"><path d="M93.781 51.578C95 50.969 96 49.359 96 48c0-1.375-1-2.969-2.219-3.578 0 0-22.868-1.514-31.781-10.422-8.915-8.91-10.438-31.781-10.438-31.781C50.969 1 49.375 0 48 0s-2.969 1-3.594 2.219c0 0-1.5 22.87-10.406 31.781-8.908 8.913-31.781 10.422-31.781 10.422C1 45.031 0 46.625 0 48c0 1.359 1 2.969 2.219 3.578 0 0 22.873 1.51 31.781 10.422 8.906 8.911 10.406 31.781 10.406 31.781C45.031 95 46.625 96 48 96s2.969-1 3.562-2.219c0 0 1.523-22.871 10.438-31.781 8.913-8.908 31.781-10.422 31.781-10.422Z" fill="#000" /></svg>
            <svg viewBox="0 0 96 96"><path d="M93.781 51.578C95 50.969 96 49.359 96 48c0-1.375-1-2.969-2.219-3.578 0 0-22.868-1.514-31.781-10.422-8.915-8.91-10.438-31.781-10.438-31.781C50.969 1 49.375 0 48 0s-2.969 1-3.594 2.219c0 0-1.5 22.87-10.406 31.781-8.908 8.913-31.781 10.422-31.781 10.422C1 45.031 0 46.625 0 48c0 1.359 1 2.969 2.219 3.578 0 0 22.873 1.51 31.781 10.422 8.906 8.911 10.406 31.781 10.406 31.781C45.031 95 46.625 96 48 96s2.969-1 3.562-2.219c0 0 1.523-22.871 10.438-31.781 8.913-8.908 31.781-10.422 31.781-10.422Z" fill="#000" /></svg>
            <svg viewBox="0 0 96 96"><path d="M93.781 51.578C95 50.969 96 49.359 96 48c0-1.375-1-2.969-2.219-3.578 0 0-22.868-1.514-31.781-10.422-8.915-8.91-10.438-31.781-10.438-31.781C50.969 1 49.375 0 48 0s-2.969 1-3.594 2.219c0 0-1.5 22.87-10.406 31.781-8.908 8.913-31.781 10.422-31.781 10.422C1 45.031 0 46.625 0 48c0 1.359 1 2.969 2.219 3.578 0 0 22.873 1.51 31.781 10.422 8.906 8.911 10.406 31.781 10.406 31.781C45.031 95 46.625 96 48 96s2.969-1 3.562-2.219c0 0 1.523-22.871 10.438-31.781 8.913-8.908 31.781-10.422 31.781-10.422Z" fill="#000" /></svg>
            <svg viewBox="0 0 96 96"><path d="M93.781 51.578C95 50.969 96 49.359 96 48c0-1.375-1-2.969-2.219-3.578 0 0-22.868-1.514-31.781-10.422-8.915-8.91-10.438-31.781-10.438-31.781C50.969 1 49.375 0 48 0s-2.969 1-3.594 2.219c0 0-1.5 22.87-10.406 31.781-8.908 8.913-31.781 10.422-31.781 10.422C1 45.031 0 46.625 0 48c0 1.359 1 2.969 2.219 3.578 0 0 22.873 1.51 31.781 10.422 8.906 8.911 10.406 31.781 10.406 31.781C45.031 95 46.625 96 48 96s2.969-1 3.562-2.219c0 0 1.523-22.871 10.438-31.781 8.913-8.908 31.781-10.422 31.781-10.422Z" fill="#000" /></svg>
            <span>HOSEA FELIX SANJAYA</span>
            <span aria-hidden="true">HOSEA FELIX SANJAYA</span>
        </a>
        <h2 id="ru" style="margin-top: -20px" class="subtitle fade-text">Хосеа Феликс Санжая</h2>
        <h2 id="jp" style="margin-top: -15px" class="subtitle fade-text">ホセア・フェリックス・サンジャヤ</h2>
    </main>

<nav class="bottom-nav">
    <a href="/quiz1/">Home</a>
    <a href="/quiz1/profile/">Profile</a>
    <a href="/quiz1/hometown/">Hometown</a>
    <a href="/quiz1/food/">Food</a>
    <a href="/quiz1/tourist/">Travel</a>
</nav>

    <script src="/quiz1/script.js"></script>
</body>

</html>
```

## Profile
```index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile - Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="/quiz1/style.css">
    <link rel="icon" type="image/png" href="/quiz1/img/avatar.png">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
        <label class="switch">
            <input type="checkbox" id="darkToggle">
            <span class="slider"></span>
        </label>
    </header>

    <nav class="side-nav">
        <ul>
            <li><a href="#about-me"><span>About</span></a></li>
            <li><a href="#hobbies"><span>Hobbies</span></a></li>
            <li><a href="#skills"><span>Skills</span></a></li>
        </ul>
    </nav>

    <main class="profile-sections">
        <section id="about-me" class="section fade-text">
            <div class="section-text">
                <h2>About <span class="highlight">Me</span></h2>
                <p>
                    Hi! I’m <span class="zigzag-inline"><strong>Hosea Felix Sanjaya</strong></span>,
                    a student at <strong>Institut Teknologi Sepuluh Nopember (ITS) Surabaya</strong>,
                    majoring in <span class="zigzag-inline"><strong>Informatics Engineering</strong></span>.
                </p>
                <p>
                    I’m passionate about <strong>data-driven technologies</strong> and especially the world of
                    <span class="zigzag-inline">Web3</span>. Exploring <strong>blockchain</strong>,
                    <strong>decentralization</strong>, and <strong>smart contracts</strong> excites me,
                    and my future ambition is to become a <strong>Blockchain Developer</strong>.
                </p>
                <p class="info-line">
                    <i class="fa-solid fa-cake-candles"></i>
                    <span class="label" style="margin-left: +3.5px;">Birthday:</span>
                    <strong>19 June 2006</strong>
                </p>
                <p class="info-line">
                    <i class="fa-solid fa-user"></i>
                    <span class="label" style="margin-left: +4px;">Age:</span>
                    <strong><span id="age"></span> years old</strong>
                </p>
                <p class="info-line">
                    <i class="fa-solid fa-rocket"></i>
                    <span class="label">Goal:</span>
                    <strong><span style="margin-left: +3px;">Blockchain Developer</span></strong>
                </p>
            </div>
            
            <div class="section-image-profile">
                <div class="avatar-flip-card">
                    <div class="card-inner">
                        <div class="card-front">
                            <img src="/quiz1/img/avatar.jpg" alt="About Me">
                        </div>
                        <div class="card-back">
                            <img src="/quiz1/img/sigma.png" alt="Sigma">
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="hobbies" class="section fade-text">
            <div class="section-text">
                <h2>Hobbies</h2>
                <div class="zigzag-container">
                    <div class="zigzag-box">🏸 Badminton</div>
                    <div class="zigzag-box">🌙 Sleeping</div>
                    <div class="zigzag-box">🎮 MLBB</div>
                    <div class="zigzag-box">🍗 PUBG</div>
                    <div class="zigzag-box">⛏️ Minecraft</div>
                    <div class="zigzag-box">🎵 Music</div>
                    <div class="zigzag-box">⛩️ Anime</div>
                    <div class="zigzag-box">🎱 Billiard</div>
                    <div class="zigzag-box">🍽️ Culinary</div>
                    <div class="zigzag-box">📱 Doomscrolling</div>
                    <div class="zigzag-box">🎯 Puzzle</div>
                    <div class="zigzag-box" onclick="window.open('https://www.youtube.com/watch?v=dQw4w9WgXcQ', '_blank')">▶️ YouTube</div>
                    <div class="zigzag-box">🎬 Netflix</div>
                    <div class="zigzag-box">💪 Gym</div>
                    <div class="zigzag-box">🛍️ Shopping</div>
                    <div class="zigzag-box">🌐 Browsing</div>
                </div>
            </div>
            <div class="section-image gallery-zigzag">
                <img src="/quiz1/img/badmin.jpg" alt="Badminton">
                <img src="/quiz1/img/gaming.jpg" alt="Gaming">
                <img src="/quiz1/img/anime.jpg" alt="Anime">
                <img src="/quiz1/img/Billiard.jpg" alt="Billiard">
                <img src="/quiz1/img/windah.jpg" alt="Youtube">
            </div>
        </section>

        <section id="skills" class="section fade-text">
            <div class="section-text">
                <h2>Skills</h2>
                <h3><span class="highlight">Hard</span> Skills</h3>
                <div class="zigzag-container">
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/c/', '_blank')">💦 C</div>
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/cpp/', '_blank')">⚡ C++</div>
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/html/', '_blank')">🌐 HTML</div>
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/css/', '_blank')">🎨 CSS</div>
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/js/', '_blank')">📜 JavaScript</div>
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/bash/', '_blank')">🐧 Linux</div>
                    <div class="zigzag-box" onclick="window.open('https://www.w3schools.com/sql/', '_blank')">🗃️ MySQL</div>
                </div>
                <h3><span class="highlight">Soft</span> Skills</h3>
                <div class="zigzag-container">
                    <div class="zigzag-box">Time Management</div>
                    <div class="zigzag-box">Adaptability</div>
                    <div class="zigzag-box">Empathy</div>
                    <div class="zigzag-box">Work Ethic</div>
                    <div class="zigzag-box">Negotiation</div>
                    <div class="zigzag-box">Networking</div>
                    <div class="zigzag-box">Creativity</div>
                    <div class="zigzag-box">Plastic Smile</div>
                </div>
            </div>
            <div class="section-image gallery-zigzag">
                <img src="/quiz1/img/prog1.jpg" alt="C++ Programming">
                <img src="/quiz1/img/prog2.jpg" alt="Web Development">
                <img src="/quiz1/img/prog3.jpg" alt="Database">
            </div>
        </section>
    </main>

    <nav class="bottom-nav">
        <a href="/quiz1/">Home</a>
        <a href="/quiz1/profile/">Profile</a>
        <a href="/quiz1/hometown/">Hometown</a>
        <a href="/quiz1/food/">Food</a>
        <a href="/quiz1/tourist/">Travel</a>
    </nav>

    <script src="/quiz1/script.js"></script>
</body>

</html>
```

## Hometown
```index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hometown - Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="/quiz1/style.css">
    <link rel="icon" type="image/png" href="/quiz1/img/avatar.png">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
        <label class="switch">
            <input type="checkbox" id="darkToggle">
            <span class="slider"></span>
        </label>
    </header>

    <nav class="side-nav">
        <ul>
            <li><a href="#hometown"><span>Hometown</span></a></li>
            <li><a href="#facts"><span>Fun Facts</span></a></li>
        </ul>
    </nav>

    <main class="profile-sections">
        <section id="hometown" class="section fade-text">
            <div class="section-text">
                <h2>My Hometown: <span class="highlight">Kediri</span></h2>
                <p>
                    Kediri is one of the oldest cities in East Java, located about 130 km southwest of Surabaya.
                    Covering 63.40 km² with a population of over 300,000, the city is divided by the Brantas River,
                    which gives it a refreshing and scenic atmosphere.
                </p>
                <p>
                    Known as a major center for sugar and tobacco production and home to <em>Gudang Garam</em>,
                    Kediri also holds rich cultural and historical value. To me, it is more than just a hometown—
                    it is a place of stories, heritage, and warm community spirit.
                </p>
                <p class="source-text" style="font-size:0.9rem; margin-top:20px;">
                    Source: <a href="https://id.wikipedia.org/wiki/Kota_Kediri" target="_blank" rel="noopener noreferrer" class="source-link" style="text-decoration: none; transition: color 0.3s ease;">Kota Kediri – Wikipedia</a>
                </p>
            </div>
            <div class="section-image">
                <img style="max-width: 800px;" src="/quiz1/img/monumen.jpg" alt="Kediri City">
            </div>
        </section>

        <section id="facts" class="section fade-text">
            <div class="section-text">
                <h2>Fun Facts about <span class="highlight">Kediri</span></h2>
                <div class="zigzag-container">
                    <a class="zigzag-box" style="text-decoration: none;" href="https://id.wikipedia.org/wiki/Gunung_Kelud" target="_blank" rel="noopener noreferrer">🌋 Home to the active volcano Mount Kelud</a>
                    <a class="zigzag-box" style="text-decoration: none;" href="https://authentic-indonesia.com/blog/5-oldest-cities-in-indonesia/" target="_blank" rel="noopener noreferrer">🛕 One of the oldest cities in East Java</a>
                    <a class="zigzag-box" style="text-decoration: none;" href="https://www.kedirikota.go.id/p/dalamberita/13981/tahu-takwa-dan-getuk-pisang-khas-kediri-jajanan-favorit-pemudik" target="_blank" rel="noopener noreferrer">🧈 Famous for Tahu Takwa & Getuk Pisang</a>
                    <a class="zigzag-box" style="text-decoration: none;" href="https://kumparan.com/juniar-aleyda1106/mengenal-kebudayaan-di-kediri-yang-kaya-akan-sejarah-dan-tradisi-22jkq5myax5" target="_blank" rel="noopener noreferrer">🎭 Rich in traditional cultural performances</a>
                    <a class="zigzag-box" style="text-decoration: none;" href="https://beautyofindonesia.com/id/wisata/wisata-alam/air-terjun-irenggolo" target="_blank" rel="noopener noreferrer">🌊 Waterfalls and tea plantations nearby</a>
                </div>
            </div>
            <div class="section-image gallery-zigzag">
                <img src="/quiz1/img/kelud.jpg" alt="Mount Kelud">
                <img src="/quiz1/img/tahu.jpg" alt="Tahu Takwa">
                <img src="/quiz1/img/getuk.jpg" alt="Getuk Pisang">
            </div>
        </section>
    </main>

<nav class="bottom-nav">
    <a href="/quiz1/">Home</a>
    <a href="/quiz1/profile/">Profile</a>
    <a href="/quiz1/hometown/">Hometown</a>
    <a href="/quiz1/food/">Food</a>
    <a href="/quiz1/tourist/">Travel</a>
</nav>

    <script src="../script.js"></script>
</body>

</html>
```

## Local Food
```index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Local Food - Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="/quiz1/style.css">
    <link rel="icon" type="image/png" href="/quiz1/img/avatar.png">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
        <label class="switch">
            <input type="checkbox" id="darkToggle">
            <span class="slider"></span>
        </label>
    </header>

    <nav class="side-nav">
        <ul>
            <li><a href="#local"><span>About</span></a></li>
            <li><a href="#dream"><span>Hobbies</span></a></li>
        </ul>
    </nav>

    <main class="profile-sections">
        <section id="local" class="section fade-text">
            <div class="section-text">
                <h2>Favorite <span class="highlight">Local</span> Foods</h2>
                <p>My favorite local foods so far...</p>
                <div class="zigzag-container">
                    <div class="zigzag-box">🥞 Martabak</div>
                    <div class="zigzag-box">🍚 Nasi Goreng</div><br>
                    <div class="zigzag-box">🍜 Mie Ayam</div>
                    <div class="zigzag-box">🟤 Bakso</div>
                    <div class="zigzag-box">🍲 Soto Soup</div>
                    <div class="zigzag-box">🍢 Satay</div>
                </div>
            </div>
            <div class="food-gallery">
                <img src="/quiz1/img/martabak.jpg" alt="Martabak">
                <img src="/quiz1/img/nasigoreng.jpg" alt="Nasi Goreng">
                <img src="/quiz1/img/mieayam.jpg" alt="Mie Ayam">
                <img src="/quiz1/img/bakso.jpg" alt="Bakso">
                <img src="/quiz1/img/soto.jpg" alt="Soto Soup">
                <img src="/quiz1/img/sate.jpg" alt="Satay">
            </div>
        </section>

        <section id="dream" class="section fade-text">
            <div class="section-text">
                <h2><span class="highlight">Dream</span> Foods</h2>
                <p>Here are some international dishes I dream of trying someday.</p>
                <div class="zigzag-container">
                    <div class="zigzag-box">🍖 Tonkatsu</div>
                    <div class="zigzag-box">🍗 Turkey Leg</div>
                    <div class="zigzag-box">🥩 Beef Stroganoff</div>
                    <div class="zigzag-box">🍛 Nasi Kandar</div>
                    <div class="zigzag-box">🥙 Shawarma</div>
                    <div class="zigzag-box">🥣 Borscht</div>
                </div>
            </div>
            <div class="section-image food-gallery1">
                <img src="/quiz1/img/tonkatsu.jpg" alt="Tonkatsu">
                <img src="/quiz1/img/turkeyleg.jpg" alt="Turkey Leg">
                <img src="/quiz1/img/stroganoff.jpg" alt="Beef Stroganoff">
                <img src="/quiz1/img/nasikandar.jpg" alt="Nasi Kandar">
                <img src="/quiz1/img/shawarma.jpg" alt="Shawarma">
                <img src="/quiz1/img/borscht.jpg" alt="Borscht">
            </div>
        </section>
    </main>

<nav class="bottom-nav">
    <a href="/quiz1/">Home</a>
    <a href="/quiz1/profile/">Profile</a>
    <a href="/quiz1/hometown/">Hometown</a>
    <a href="/quiz1/food/">Food</a>
    <a href="/quiz1/tourist/">Travel</a>
</nav>

    <script src="/quiz1/script.js"></script>
</body>

</html>
```
## Tourist Places
```index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tourist Places - Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="/quiz1/style.css">
    <link rel="icon" type="image/png" href="/quiz1/img/avatar.png">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
        <label class="switch">
            <input type="checkbox" id="darkToggle">
            <span class="slider"></span>
        </label>
    </header>

    <main class="profile-sections">
        <section class="section fade-text intro" style="flex-direction: column; text-align:center; justify-content: center;">
            <div class="section-text" style="max-width:1000px;">
                <h2 style="margin-top: -130px;">A Guide to Tourist Attractions in <span class="highlight">Kediri</span></h2>
                <p>Kediri offers a variety of attractions, from natural wonders to cultural heritage. Here are some highlights you can explore when visiting my hometown:</p>
                <div class="tourist-grid">
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-mountain"></i><h3>Mount Kelud</h3></div>
                            <div class="card-back"><p>An active volcano with scenic views.</p><a href="https://id.wikipedia.org/wiki/Gunung_Kelud" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-landmark"></i><h3>Goa Selomangleng</h3></div>
                            <div class="card-back"><p>Historical cave with ancient reliefs.</p><a href="https://id.wikipedia.org/wiki/Gua_Selomangleng" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-archway"></i><h3>Simpang Lima Gumul</h3></div>
                            <div class="card-back"><p>Kediri's most Iconic landmark.</p><a href="https://id.wikipedia.org/wiki/Simpang_Lima_Gumul" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-water"></i><h3>Dolo & Irenggolo Waterfalls</h3></div>
                            <div class="card-back"><p>Refreshing natural escapes.</p><a href="https://beautyofindonesia.com/id/wisata/wisata-alam/air-terjun-irenggolo" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-utensils"></i><h3>Tahu Takwa & Getuk Pisang</h3></div>
                            <div class="card-back"><p>Local culinary you must try.</p><a href="https://www.kedirikota.go.id/p/dalamberita/13981/tahu-takwa-dan-getuk-pisang-khas-kediri-jajanan-favorit-pemudik" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-theater-masks"></i><h3>Jaranan Dance</h3></div>
                            <div class="card-back"><p>Kediri's traditional performance.</p><a href="https://kumparan.com/juniar-aleyda1106/mengenal-kebudayaan-di-kediri-yang-kaya-akan-sejarah-dan-tradisi-22jkq5myax5" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-fire"></i><h3>Gudang Garam</h3></div>
                            <div class="card-back"><p>One of the largest cigarette companies.</p><a href="https://id.wikipedia.org/wiki/Gudang_Garam" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-inner">
                            <div class="card-front"><i class="fas fa-bridge"></i><h3>Brawijaya Bridge</h3></div>
                            <div class="card-back"><p>A landmark bridge in the city.</p><a href="https://id.wikipedia.org/wiki/Jembatan_Brawijaya" target="_blank">Learn more</a></div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

<nav class="bottom-nav">
    <a href="/quiz1/">Home</a>
    <a href="/quiz1/profile/">Profile</a>
    <a href="/quiz1/hometown/">Hometown</a>
    <a href="/quiz1/food/">Food</a>
    <a href="/quiz1/tourist/">Travel</a>
</nav>

    <script src="/quiz1/script.js"></script>
</body>

</html>
```

## script.js
```script.js
document.addEventListener("DOMContentLoaded", function () {

    // --- 1. Real-time Clock ---
    const clockElement = document.getElementById("clock");
    if (clockElement) {
        const updateClock = () => {
            const now = new Date();
            const h = String(now.getHours()).padStart(2, "0");
            const m = String(now.getMinutes()).padStart(2, "0");
            const s = String(now.getSeconds()).padStart(2, "0");
            clockElement.textContent = `${h}:${m}:${s}`;
        };
        setInterval(updateClock, 1000);
        updateClock();
    }

    // --- 2. Dark Mode Toggle ---
    const toggleBtn = document.getElementById("darkToggle");
    if (toggleBtn) {
        let darkMode = localStorage.getItem("dark-mode");

        const enableDarkMode = () => {
            document.body.classList.add("dark");
            toggleBtn.checked = true;
            localStorage.setItem("dark-mode", "enabled");
        };

        const disableDarkMode = () => {
            document.body.classList.remove("dark");
            toggleBtn.checked = false;
            localStorage.setItem("dark-mode", "disabled");
        };

        if (darkMode === "enabled") {
            enableDarkMode();
        }

        toggleBtn.addEventListener("change", () => {
            darkMode = localStorage.getItem("dark-mode");
            if (darkMode !== "enabled") {
                enableDarkMode();
            } else {
                disableDarkMode();
            }
        });
    }

    // --- 3. Page-Specific Animations ---
    // For index.html fade-in
    const hfs = document.getElementById("hfs");
    if (hfs) {
        const ru = document.getElementById("ru");
        const jp = document.getElementById("jp");
        setTimeout(() => {
            hfs.classList.add("show");
            ru.classList.add("show");
            jp.classList.add("show");
        }, 100);
    }

    // For scroll-based fade-in on other pages
    const sections = document.querySelectorAll('.section');
    if (sections.length > 0) {
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('show');
                }
            });
        }, { threshold: 0.5 });
        sections.forEach(sec => observer.observe(sec));
    }
    
    // For profile.html age calculation
    const ageSpan = document.getElementById("age");
    if (ageSpan) {
        const calculateAge = (birthDate) => {
            const today = new Date();
            let age = today.getFullYear() - birthDate.getFullYear();
            const monthDiff = today.getMonth() - birthDate.getMonth();
            if (monthDiff < 0 || (monthDiff === 0 && today.getDate() < birthDate.getDate())) {
                age--;
            }
            return age;
        }
        const birthday = new Date(2006, 5, 19); // Month is 0-indexed (5 = June)
        ageSpan.textContent = calculateAge(birthday);
    }


    // --- 4. Sparkle Effect on Click ---
    document.addEventListener("click", function (e) {
        for (let i = 0; i < 9; i++) {
            const spark = document.createElement("div");
            spark.classList.add("spark");
            spark.style.left = `${e.pageX}px`;
            spark.style.top = `${e.pageY}px`;

            const angle = (360 / 9) * i;
            const distance = Math.random() * 60 + 30;

            spark.style.setProperty("--angle", `${angle}deg`);
            spark.style.setProperty("--distance", `${distance}px`);
            document.body.appendChild(spark);

            setTimeout(() => spark.remove(), 1000);
        }
    });
});

    // --- 5. Navigation Highlighting ---
document.addEventListener("DOMContentLoaded", function () {
    const navLinks = document.querySelectorAll('nav ul li a');
    const sections = document.querySelectorAll('main .section');
    const options = { threshold: 0.5 };
    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            const id = entry.target.id;
            const navLink = document.querySelector(`nav ul li a[href="#${id}"]`);
            if (entry.isIntersecting) {
                navLinks.forEach(link => link.classList.remove('active'));
                if (navLink) navLink.classList.add('active');
            }
        });
    }, options);
    sections.forEach(section => {
        if (section.id) {
            observer.observe(section);
        }
    });
});
```

## Style.css
```style.css
/* ========================
   Base & Root Styles
======================== */
:root {
    --color: #f1a829f3;
    --shadow: #e5ce9e;
    --glare: hsla(51, 88%, 77%, 0.75);
    --font-size: 4rem;
    --transition: 0.2s;
}

html {
    overflow-y: scroll;
    scrollbar-gutter: stable;
}

::-webkit-scrollbar {
    width: 0px;
}

body {
    margin: 0;
    font-family: "Poppins", sans-serif;
    background-color: #fff;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    color: #2c3e50;
    position: relative;
    overflow: hidden;
}

/* ========================
   Background & Animations
======================== */
body::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image:
        linear-gradient(90deg, rgba(70, 70, 70, 0.08) 1.3px, transparent 1px),
        linear-gradient(rgba(70, 70, 70, 0.08) 1.3px, transparent 1px);
    background-size: 40px 40px;
    animation: boxPop 17s ease-in-out infinite, boxColor 10s linear infinite;
    z-index: -1;
    opacity: 0.7;
    filter: blur(0.2px);
}

/* EFEK VIGNETTE BARU */
body::after {
    content: "";
    position: fixed;
    inset: 0;
    background: radial-gradient(ellipse at center, transparent 50%, rgba(0, 0, 0, 0.4) 125%);
    z-index: -1;
    pointer-events: none;
}

@keyframes boxPop {

    0%,
    100% {
        transform: scale(1);
        opacity: 0.4;
    }

    50% {
        transform: scale(1.3);
        opacity: 0.8;
    }
}

@keyframes boxColor {
    0% {
        filter: hue-rotate(0deg);
    }

    50% {
        filter: hue-rotate(180deg);
    }

    100% {
        filter: hue-rotate(360deg);
    }
}

@keyframes fadeDown {
    from {
        opacity: 0;
        transform: translateY(-30px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes explode {
    from {
        transform: rotate(var(--angle)) translateY(0);
        opacity: 1;
    }

    to {
        transform: rotate(var(--angle)) translateY(var(--distance));
        opacity: 0;
    }
}

.fade-text {
    opacity: 0;
}

.show {
    animation: fadeDown 1s ease forwards;
}

/* ========================
   Header & Clock
======================== */
.top-right {
    position: fixed;
    top: 15px;
    right: 25px;
    display: flex;
    align-items: center;
    gap: 20px;
    font-size: 1.5rem;
    z-index: 1000;
    font-family: "Poppins", sans-serif;
}

.top-right a {
    color: #333;
    text-decoration: none;
    transition: color 0.3s ease, transform 0.2s ease;
}

.top-right a:hover {
    color: #f39c12;
    transform: scale(1.2);
}

#clock {
    font-family: "Roboto Mono", monospace;
    font-weight: 500;
    font-size: 1.3rem;
    letter-spacing: 1px;
}

/* ========================
   Navigation
======================== */
.bottom-nav {
    position: fixed;
    bottom: 25px;
    left: 50%;
    transform: translateX(-50%);
    background: rgba(20, 20, 20, 0.705);
    color: white;
    padding: 10px 20px;
    border-radius: 30px;
    display: flex;
    gap: 15px;
    align-items: center;
    font-size: 0.9rem;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
    z-index: 1000;
    font-family: "Poppins", sans-serif;
    font-weight: 700;
    background-image: radial-gradient(#00000060 1px, transparent 1px);
    background-size: 7px 7px;
    backdrop-filter: blur(3px);
}

.bottom-nav a {
    text-decoration: none;
    color: white;
    padding: 12px 12px;
    border-radius: 40px;
    transition: 0.3s ease;
}

.bottom-nav a:hover {
    background-color: #11111146;
}

/* ========================
   Main Content & Sections
======================== */
.center {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.center .subtitle {
    font-size: 2rem;
    color: #666;
    margin-top: 10px;
}

.profile-sections {
    overflow-y: auto;
    scroll-behavior: smooth;
    margin: -70px auto 0;
    padding: 0 40px;
    max-width: 1200px;
    height: 100vh;
}

.section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 60px 40px;
    gap: 40px;
    flex-wrap: wrap;
}

.section.intro {
    flex-direction: column;
    justify-content: center;
    text-align: center;
    margin-top: 25%;
}

.section.hometown {
    justify-content: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 20px;
}

.section-text {
    flex: 1;
    padding: 0;
    text-align: left;
}

.section-text h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
}

.section-text h3 {
    font-size: 1.5rem;
    margin: 25px 0 10px;
    color: #555;
}

.section-text p {
    font-size: 1.2rem;
    line-height: 1.8;
    color: #333;
}

.section-image {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
}

.section-image img {
    max-width: 300px;
    max-height: 300px;
    border-radius: 20px;
    object-fit: cover;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease;
}

.section-image img:hover {
    transform: scale(1.1);
}

.section-image-profile {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    min-width: 300px;
}

.section-image-profile img {
    max-width: 300px;
    max-height: 300px;
    border-radius: 20px;
    object-fit: cover;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease;

}

/* ========================
   Components
======================== */
/* Dark Mode Switch */
.switch {
    position: relative;
    display: inline-block;
    width: 54px;
    height: 26px;
    margin-left: 10px;
}

.switch input {
    opacity: 0;
    width: 0;
    height: 0;
}

.slider {
    position: absolute;
    cursor: pointer;
    inset: 0;
    background-color: #ccc;
    transition: 0.4s;
    border-radius: 26px;
    box-shadow: 0 6px 20px rgba(47, 4, 68, 0.267);
}

.slider:before {
    position: absolute;
    content: "🌝";
    height: 22px;
    width: 28px;
    left: 1px;
    bottom: 2px;
    text-align: center;
    font-size: 20px;
    line-height: 22px;
    background-color: transparent;
    border-radius: 50%;
    transition: 0.5s;
}

input:checked+.slider {
    background-color: #444;
    box-shadow: 0 6px 20px rgba(172, 172, 172, 0.205);
}

input:checked+.slider:before {
    transform: translateX(24px);
    content: "🌚";
}

.highlight {
    background-color: #f39c12;
    color: #fff;
    padding: 5px 10px;
    border-radius: 10px;
}

.info-line {
    display: flex;
    align-items: center;
    gap: 10px;
    margin: 5px 0;
    font-size: 1rem;
}

.info-line .label {
    min-width: 76px;
    font-weight: 500;
}

.source-text {
    color: #777;
    font-size: 0.9rem;
    margin-top: 20px;
}

.source-link {
    color: #333;
    text-decoration: none;
    transition: color 0.3s ease;
}

.zigzag-container {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    max-width: 650px;
    margin-top: 20px;
}

.zigzag-box {
    background: #f0f2f3;
    padding: 15px 20px;
    border-radius: 15px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    font-size: 1.1rem;
    font-weight: 500;
    color: #2c3e50;
    transition: all 0.5s ease;
    cursor: pointer;
    text-decoration: none;
    position: relative;
    overflow: hidden;
}

.zigzag-box::before {
    content: '';
    position: absolute;
    top: -50%;
    left: -50%;
    width: 200%;
    height: 200%;
    background: linear-gradient(0deg, transparent, transparent 30%, rgba(170, 103, 16, 0.514));
    transform: rotate(-45deg);
    transition: all 0.5s ease;
    opacity: 0;
}

.zigzag-box:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
    background-color: #f3b95b;
    color: #fff;
}

.zigzag-box:hover::before {
    opacity: 1;
    transform: rotate(-45deg) translateY(100%);
}

.zigzag-inline {
    display: inline-block;
    padding: 2px 10px 2px 12px;
    font-size: 1em;
    border-radius: 10px;
    background: #f0f2f385;
    transition: all 0.3s ease;
}

.zigzag-inline:hover {
    background-color: #f39c12;
    color: #fff;
}

.gallery-zigzag {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 25px;
    max-width: 420px;
    margin: 50px auto 0;
    position: relative;
}

.gallery-zigzag img {
    width: 180px;
    height: 180px;
    object-fit: cover;
    border-radius: 20px;
    box-shadow: 10px 10px 20px #babecc, -10px -10px 20px #ffffff;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.gallery-zigzag img:nth-child(1) {
    transform: rotate(-6deg) translateY(15px);
}

.gallery-zigzag img:nth-child(2) {
    transform: rotate(5deg) translateY(-20px);
}

.gallery-zigzag img:nth-child(3) {
    transform: rotate(7deg) translateY(15px);
}

.gallery-zigzag img:nth-child(4) {
    transform: rotate(3deg) translateY(1px);
}

.gallery-zigzag img:nth-child(5) {
    transform: rotate(-8deg) translateY(10px);
}

.gallery-zigzag img:hover {
    transform: scale(1.3) rotate(0deg);
    box-shadow: 0 12px 35px rgba(0, 0, 0, 0.3);
}

.food-gallery,
.food-gallery1 {
    display: grid;
    grid-template-columns: repeat(2, auto);
    gap: 20px 40px;
    justify-content: center;
    margin-top: 45px;
}

.food-gallery img,
.food-gallery1 img {
    width: 180px;
    height: 180px;
    object-fit: cover;
    border-radius: 12px;
    box-shadow: 10px 10px 20px #babecc, -10px -10px 20px #ffffff;
    transition: transform 0.4s ease, box-shadow 0.4s ease;
    cursor: pointer;
}

.food-gallery img:hover,
.food-gallery1 img:hover {
    transform: scale(1.2) translateY(-5px);
    box-shadow: 10px 10px 20px #babecc, -10px -10px 20px #ffffff;
}

.food-gallery img:nth-child(3),
.food-gallery img:nth-child(4) {
    transform: translateX(40px);
}

.food-gallery img:nth-child(3):hover,
.food-gallery img:nth-child(4):hover {
    transform: translateX(40px) scale(1.2) translateY(-5px);
}

.food-gallery1 img:nth-child(1),
.food-gallery1 img:nth-child(2),
.food-gallery1 img:nth-child(5),
.food-gallery1 img:nth-child(6) {
    transform: translateX(40px);
}

.food-gallery1 img:nth-child(1):hover,
.food-gallery1 img:nth-child(2):hover,
.food-gallery1 img:nth-child(5):hover,
.food-gallery1 img:nth-child(6):hover {
    transform: translateX(40px) scale(1.2) translateY(-5px);
}

.avatar-flip-card:hover .card-inner {
    transform: rotateY(180deg);
}

.tourist-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 20px;
    justify-items: center;
}

.card {
    width: 220px;
    height: 260px;
    margin: 1rem auto;
    perspective: 1000px;
    cursor: pointer;
}

.card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    transition: transform 0.6s;
    transform-style: preserve-3d;
}

.card:hover .card-inner {
    transform: rotateY(180deg);
}

.card-front,
.card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    border-radius: 1rem;
    box-shadow: 10px 10px 20px #babecc, -10px -10px 20px #ffffff;
    text-align: center;
}

.card-front {
    background: #ffffffee;
    color: #2c3e50;
    border: 1px solid #e5e7eb;
}

.card-front i {
    font-size: 2.5em;
    margin-bottom: 15px;
    color: #f39c12;
}

.card-front h3 {
    font-size: 1.1rem;
    margin: 0 25px;
}

.card-back {
    background: #f39c12;
    color: white;
    transform: rotateY(180deg);
}

.card-back p {
    font-size: 1.1rem;
    margin: 20px;
    font-weight: 600;
    color: white;
}

.card-back a {
    color: #fff;
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
}

/* ========================
   Special Effects
======================== */
.sparkle-button {
    --padding: 1rem;
    padding: var(--padding);
    border-radius: 0.5rem;
    text-decoration: none;
    color: transparent;
    position: relative;
    transition: background 0.2s;
    margin-bottom: 1rem;
    --hover: 0.4;
    --pos: 0;
}

.sparkle-button:hover {
    --hover: 1;
    --pos: 1;
}

.sparkle-button:active {
    --hover: 0;
}

.sparkle-button:active span:last-of-type {
    --hover: 0;
    --pos: 1;
}

.sparkle-button span {
    display: inline-block;
    font-size: var(--font-size);
    font-weight: 800;
    transition: all 0.2s;
    text-decoration: none;
    text-shadow:
        calc(var(--hover) * -0px) calc(var(--hover) * 0px) var(--shadow),
        calc(var(--hover) * -2px) calc(var(--hover) * 2px) var(--shadow),
        calc(var(--hover) * -3px) calc(var(--hover) * 3px) var(--shadow),
        calc(var(--hover) * -4px) calc(var(--hover) * 4px) var(--shadow),
        calc(var(--hover) * -5px) calc(var(--hover) * 5px) var(--shadow);
    transform: translate(calc(var(--hover) * 5px), calc(var(--hover) * -5px));
}

.sparkle-button span:last-of-type {
    position: absolute;
    inset: var(--padding);
    background: linear-gradient(108deg,
            transparent 0 55%,
            var(--glare) 55% 60%,
            transparent 60% 70%,
            var(--glare) 70% 85%,
            transparent 85%) calc(var(--pos) * -200%) 0% / 200% 100%, var(--color);
    -webkit-background-clip: text;
    background-clip: text;
    z-index: 2;
    text-shadow: none;
    transition: transform 0.2s, background-position 0s;
}

.sparkle-button:hover span:last-of-type {
    transition: transform 0.2s, background-position calc(var(--hover) * 1.5s) calc(var(--hover) * 0.25s);
}

.sparkle-button svg {
    position: absolute;
    z-index: 3;
    width: calc(var(--font-size) * 0.5);
    aspect-ratio: 1;
    --delay-step: 0.15;
    top: calc(var(--y, 50) * 1%);
    left: calc(var(--x, 0) * 1%);
    transform: translate(-50%, -50%) scale(0);
}

.sparkle-button svg path {
    fill: var(--glare);
}

.sparkle-button:hover svg {
    animation: sparkle 0.75s calc((var(--delay-step) * var(--d)) * 1s) both;
}

@keyframes sparkle {
    50% {
        transform: translate(-50%, -50%) scale(var(--s, 1));
    }
}

.sparkle-button svg:nth-of-type(1) {
    --x: 0;
    --y: 20;
    --s: 1.1;
    --d: 1;
}

.sparkle-button svg:nth-of-type(2) {
    --x: 15;
    --y: 80;
    --s: 1.25;
    --d: 2;
}

.sparkle-button svg:nth-of-type(3) {
    --x: 45;
    --y: 40;
    --s: 1.1;
    --d: 3;
}

.sparkle-button svg:nth-of-type(4) {
    --x: 75;
    --y: 60;
    --s: 0.9;
    --d: 2;
}

.sparkle-button svg:nth-of-type(5) {
    --x: 100;
    --y: 30;
    --s: 0.8;
    --d: 4;
}

.spark {
    position: absolute;
    width: 3.3px;
    height: 20px;
    background: #f39d12;
    pointer-events: none;
    opacity: 0;
    transform-origin: 70% center;
    animation: explode 0.5s ease-out forwards;
}

/* ========================
   Dark Mode
======================== */
body.dark {
    color: #f5f5f5;
    background-color: rgb(41, 38, 48);
}

body.dark::before {
    background-image:
        linear-gradient(90deg, rgba(170, 147, 177, 0.08) 1.3px, transparent 1px),
        linear-gradient(rgba(170, 147, 177, 0.08) 1.3px, transparent 1px);
}

body.dark .subtitle {
    color: #a7a7a7;
}

body.dark h1,
body.dark h2,
body.dark p {
    color: #f5f5f5;
}

body.dark h3 {
    color: #d1d1d1;
}

body.dark .top-right a {
    color: #f5f5f5;
}

body.dark .top-right a:hover {
    color: #ff6dc2b0;
}

body.dark .bottom-nav {
    background-color: rgba(23, 20, 24, 0.6);
    background-image: radial-gradient(#674b6b60 1px, transparent 1px);
}

body.dark .bottom-nav a:hover {
    background-color: #5a495e46;
}

body.dark .highlight {
    background-color: #fc56b7c2;
}

body.dark .zigzag-inline {
    background: #4b3a4d85;
}

body.dark .zigzag-inline:hover {
    background-color: #ff73c59d;
}

body.dark .zigzag-box {
    background: #454049;
    color: white;
}

body.dark .zigzag-box:hover {
    background-color: #6e2b8d;
}

body.dark .zigzag-box::before {
    background: linear-gradient(0deg, transparent, transparent 30%, rgba(255, 105, 180, 0.3));
}

body.dark .gallery-zigzag img,
body.dark .food-gallery img,
body.dark .food-gallery1 img {
    box-shadow: 10px 10px 20px #2a0c3860, -10px -10px 20px #0000006c;
}

body.dark .gallery-zigzag img:hover,
body.dark .food-gallery img:hover,
body.dark .food-gallery1 img:hover {
    box-shadow: 10px 10px 20px #2d0a3d7c, -10px -10px 20px #0000006c;
}

body.dark .card-front,
body.dark .card-back {
    box-shadow: 10px 10px 20px #2a0c3860, -10px -10px 20px #0000006c;
}

body.dark .card-front {
    background: #2f2b34;
    border: 1px solid #2b2c30;
}

body.dark .card-front i {
    color: #ff6dc2b0;
}

body.dark .card-front h3 {
    color: #e8e8e8;
}

body.dark .card-back {
    background: #fc56b7c2;
}

body.dark .card-back p {
    color: white;
}

body.dark .sparkle-button span {
    --color: #ff6dc2;
    --shadow: #582d48;
    --glare: hsla(57, 100%, 75%, 0.75);
}

body.dark .spark {
    background: #fc56b7;
}

body.dark .source-text,
body.dark .source-link {
    color: #fff;
}

/* ========================
   RESPONSIVE DESIGN
======================== */
@media (max-width: 1200px) {

    .profile-sections,
    .section {
        padding: 50px 30px;
    }
}

@media (max-width: 900px) {
    .section {
        flex-direction: column;
        text-align: center;
        padding: 40px 20px;
        margin-top: 150px;
    }

    .section-text {
        text-align: center;
        margin: 0 auto;
    }

    .section-image {
        margin: 20px auto 0;
    }

    .section-image.avatar-image {
        margin-top: -1000px;
    }

    .section-image img {
        max-width: 220px;
        max-height: 220px;
    }

    .gallery-zigzag {
        margin: 0 auto;
    }

    .profile-sections {
        padding: 0 20px;
    }

    .section.hometown {
        flex-direction: column;
        text-align: center;
        padding: 40px 20px;
    }

    .section.hometown .section-text {
        text-align: center;
        padding: 0;
    }

    .section.hometown .section-text h2 {
        font-size: 1.8rem;
        text-align: center;
        margin-top: 70px;
    }

    .section.hometown .section-image {
        margin-top: 25px;
    }

    .section.hometown .section-image img {
        max-width: 300px;
    }
}

@media (max-width: 600px) {
    h1 {
        font-size: 3rem;
    }

    h2 {
        font-size: 2rem;
    }

    p {
        font-size: 1rem;
        line-height: 1.6;
    }

    .section {
        margin-top: 120px;
    }

    .section-text h2 {
        font-size: 2rem;
    }

    .section-text p {
        font-size: 1rem;
        line-height: 1.6;
    }

    .section-image img {
        max-width: 180px;
        max-height: 180px;
    }

    .section-image.avatar-image {
        margin-top: -900px;
    }

    .bottom-nav {
        padding: 12px 20px;
        gap: 18px;
        font-size: 0.8rem;
    }

    .gallery-zigzag {
        opacity: 0;
    }

    .section.hometown {
        padding: 30px 15px;
    }

    .section.hometown .section-text h2 {
        font-size: 1.8rem;
        margin-top: 70px;
    }

    .section.hometown .section-text p {
        font-size: 1rem;
        line-height: 1.6;
    }

    .section.hometown .section-image img {
        max-width: 220px;
    }

    .top-right {
        top: 10px;
        right: 15px;
        gap: 15px;
        font-size: 1.2rem;
    }

    .side-nav {
        right: 15px;
    }

    .zigzag-container {
        max-width: 100%;
        gap: 15px;
    }

    .zigzag-box {
        padding: 10px 15px;
        font-size: 1rem;
    }

    .tourist-grid {
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 15px;
    }

    .card {
        width: 200px;
        height: 240px;
    }

    .food-gallery,
    .food-gallery1 {
        grid-template-columns: repeat(1, auto);
        gap: 15px;
    }

    .food-gallery img,
    .food-gallery1 img {
        width: 160px;
        height: 160px;
    }

    .sparkle-button span {
        font-size: 3rem;
    }

    .sparkle-button svg {
        width: calc(3rem * 0.5);
    }
}

@media (max-width: 400px) {
    h1 {
        font-size: 2.5rem;
    }

    .profile-sections {
        padding: 0 15px;
    }

    .section {
        padding: 20px;
    }

    .section-image img,
    .section-image-profile img {
        max-width: 160px;
        max-height: 160px;
    }

    .sparkle-button {
        --padding: 0.5rem;
    }

    .bottom-nav {
        padding: 10px 15px;
        gap: 10px;
        font-size: 0.75rem;
    }

    .gallery-zigzag img {
        width: 140px;
        height: 140px;
    }

    .food-gallery img,
    .food-gallery1 img {
        width: 140px;
        height: 140px;
    }

    .sparkle-button span {
        font-size: 2.5rem;
    }

    .sparkle-button svg {
        width: calc(2.5rem * 0.5);
    }
}

/* ========================
   ACCESSIBILITY & FOCUS STYLES
======================== */

/* Reduced Motion */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
        scroll-behavior: auto !important;
    }

    body::before {
        animation: none;
    }
}

/* High Contrast Mode */
@media (prefers-contrast: high) {

    .zigzag-box,
    .card-front,
    .card-back {
        border: 2px solid currentColor;
    }

    .gallery-zigzag img,
    .food-gallery img,
    .food-gallery1 img {
        border: 2px solid #333;
    }

    body.dark .gallery-zigzag img,
    body.dark .food-gallery img,
    body.dark .food-gallery1 img {
        border: 2px solid #fff;
    }
}

/* Print Styles */
@media print {

    body::before,
    body::after {
        display: none;
    }

    .top-right,
    .bottom-nav,
    .side-nav {
        display: none;
    }

    .sparkle-button svg {
        display: none;
    }

    .section {
        break-inside: avoid;
        page-break-inside: avoid;
    }

    body {
        background: white !important;
        color: black !important;
    }
}

/* ========================
   Profile Page Scroll Effect
======================== */
.profile-page {
    scroll-snap-type: y mandatory;
    overflow-y: scroll;
}

.profile-scroll-container {
    width: 100%;
}

.profile-section {
    height: 100vh;
    width: 100%;
    scroll-snap-align: start;
    scroll-snap-stop: always;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 5%;
    box-sizing: border-box;
}

.profile-section .section-content {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 40px;
    flex-wrap: wrap;
    max-width: 1200px;
}

/* Navigasi Titik di Samping */
.side-nav {
    position: fixed;
    top: 50%;
    right: 30px;
    transform: translateY(-50%);
    z-index: 1001;
}

.side-nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
}

.side-nav li {
    margin: 20px 0;
}

.side-nav a {
    display: block;
    width: 12px;
    height: 12px;
    background-color: rgba(0, 0, 0, 0.3);
    border-radius: 50%;
    position: relative;
    transition: all 0.3s ease;
}

.side-nav a:hover {
    background-color: #f39c12;
    transform: scale(1.3);
}

.side-nav a span {
    position: absolute;
    right: 25px;
    top: 50%;
    transform: translateY(-50%) translateX(10px);
    background-color: #ffffff;
    color: #2c3e50;
    padding: 6px 12px;
    border-radius: 8px;
    white-space: nowrap;
    opacity: 0;
    visibility: hidden;
    transition: opacity 0.3s ease, transform 0.3s ease;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
}

.side-nav a:hover span {
    opacity: 1;
    visibility: visible;
    transform: translateY(-50%) translateX(0);
}

body.dark .side-nav a {
    background-color: rgba(255, 255, 255, 0.3);
}

body.dark .side-nav a:hover {
    background-color: #fc56b7c2;
}

body.dark .side-nav a span {
    background-color: #2f2b34;
    color: #f5f5f5;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.25);
}

.side-nav a.active {
    background-color: #f39c12;
    transform: scale(1.6);
}

body.dark .side-nav a.active {
    background-color: #fc56b7c2;
}

.side-nav a.active-click {
    background-color: #f3b95b;
    transform: scale(1.6);
}

body.dark .side-nav a.active-click {
    background-color: #f3b95b;
}
```
