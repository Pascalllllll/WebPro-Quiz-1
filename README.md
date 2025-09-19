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
- `(Your Domain)/quiz1` → Homepage  
- `(Your Domain)/quiz1/profile` → Profile page  
- `(Your Domain)/quiz1/hometown` → Hometown page  
- `(Your Domain)/quiz1/food` → Local Food page  
- `(Your Domain)/quiz1/tourist` → Tourist Places page

---

## Homepage
```index.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="style.css">
    <link rel="icon" type="image/png" href="avatar.png">
    <!-- Font dan icon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
    <!-- Header kanan atas -->
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i
                class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
    </header>

    <!-- Isi -->
    <main class="center">
        <h1 id="name" class="fade-text">HOSEA FELIX SANJAYA</h1>
        <h2 id="ru" class="subtitle fade-text">Хосеа Феликс Санжая</h2>
        <h2 id="jp" style="margin-top: -15px;" class="subtitle fade-text">ホセア・フェリックス・サンジャヤ</h2>
    </main>

    <!-- Navbar bawah -->
    <nav class="bottom-nav">
        <a href="index.html">Home</a>
        <a href="profile.html">Profile</a>
        <a href="hometown.html">Hometown</a>
        <a href="food.html">Food</a>
        <a href="tourist.html">Travel</a>
    </nav>

    <!-- Script jam & animasi -->
    <script>
        // Jam realtime
        function updateClock() {
            const now = new Date();
            let h = String(now.getHours()).padStart(2, "0");
            let m = String(now.getMinutes()).padStart(2, "0");
            let s = String(now.getSeconds()).padStart(2, "0");
            document.getElementById("clock").textContent = `${h}:${m}:${s}`;
        }
        setInterval(updateClock, 1000);
        updateClock();

        // Animasi fade
        window.onload = () => {
            const name = document.getElementById("name");
            const ru = document.getElementById("ru");
            const jp = document.getElementById("jp");

            setTimeout(() => name.classList.add("show"), 500);
            setTimeout(() => ru.classList.add("show"), 1500);
            setTimeout(() => jp.classList.add("show"), 2500);
        };
    </script>
</body>

</html>
```

## Profile
```profile.html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile - Hosea Felix Sanjaya</title>
    <link rel="stylesheet" href="style.css">
    <link rel="icon" type="image/png" href="avatar.png">
    <!-- Font dan icon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
    <!-- Header kanan atas -->
    <header class="top-right">
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank"><i class="fab fa-instagram"></i></a>
        <a href="https://github.com/Pascalllllll" target="_blank"><i class="fab fa-github"></i></a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank"><i
                class="fab fa-linkedin"></i></a>
        <span id="clock"></span>
    </header>

    <!-- Profile Sections -->
    <main class="profile-sections">
        <!-- About Me -->
        <section class="section fade-text">
            <div class="section-text">
                <h2>About Me</h2>
                <p>
                    Hello! My name is <strong>Hosea Felix Sanjaya</strong>.
                    I am currently pursuing my studies at <strong>Institut Teknologi Sepuluh Nopember (ITS)
                        Surabaya</strong>,
                    majoring in <strong>Informatics Engineering</strong>.
                </p>
                <p>
                    I enjoy exploring data, technology, and problem-solving.
                    My main interests are in <em>data analysis, software development</em>, and creating impactful
                    digital solutions.
                    Beyond academics, I love working on collaborative projects that mix creativity with technical depth.
                </p>
            </div>
            <div class="section-image">
                <img src="avatar.jpg" alt="About Me">
            </div>
        </section>

        <!-- Hobbies -->
        <section class="section fade-text">
            <div class="section-text">
                <h2>Hobbies</h2>
                <div class="zigzag-container">
                    <div class="zigzag-box">🏸 Badminton</div>
                    <div class="zigzag-box">😴 Sleeping</div>
                    <div class="zigzag-box">🔫 PUBG</div>
                    <div class="zigzag-box">⛏️ Minecraft</div>
                    <div class="zigzag-box">🦔 MLBB</div>
                </div>

            </div>
            <div class="section-image gallery-zigzag">
                <img src="badmin.jpg" alt="Badminton">
                <img src="gaming.jpg" alt="Gaming">
                <img src="sleep.jpg" alt="Sleeping">
            </div>
        </section>

        <!-- Skills -->
        <section class="section fade-text">
            <div class="section-text">
                <h2>Skills</h2>
                <h3>Hard Skills</h3>
                <div class="zigzag-container">
                    <div class="zigzag-box">💻 C</div>
                    <div class="zigzag-box">⚡ C++</div>
                    <div class="zigzag-box">🌐 HTML</div>
                    <div class="zigzag-box">🎨 CSS</div>
                    <div class="zigzag-box">📜 JavaScript</div>
                    <div class="zigzag-box">🐧 Linux</div>
                    <div class="zigzag-box">📂 MySQL</div>
                </div>

                <h3>Soft Skills</h3>
                <div class="zigzag-container">
                    <div class="zigzag-box">Environmental Analysis</div>
                    <div class="zigzag-box">Emotion Prediction</div>
                    <div class="zigzag-box">Remote Observation</div>
                </div>
            </div>
            <div class="section-image gallery-zigzag">
                <img src="prog1.jpg" alt="C++ Programming">
                <img src="prog2.jpg" alt="Web Development">
                <img src="prog3.jpg" alt="Database">
            </div>
        </section>
    </main>

    <!-- Navbar bawah -->
    <nav class="bottom-nav" style="padding: 12px 26px; font-size: 15.1px;">
        <a href="index.html">Home</a>
        <a href="profile.html">Profile</a>
        <a href="hometown.html">Hometown</a>
        <a href="food.html">Food</a>
        <a href="tourist.html">Travel</a>
    </nav>

    <!-- Jam + Animasi -->
    <script>
        function updateClock() {
            const now = new Date();
            let h = String(now.getHours()).padStart(2, "0");
            let m = String(now.getMinutes()).padStart(2, "0");
            let s = String(now.getSeconds()).padStart(2, "0");
            document.getElementById("clock").textContent = `${h}:${m}:${s}`;
        }
        setInterval(updateClock, 1000);
        updateClock();

        // Animasi fade saat scroll
        const sections = document.querySelectorAll('.section');
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('show');
                }
            });
        }, { threshold: 0.5 });

        sections.forEach(sec => observer.observe(sec));
    </script>
</body>

</html>
```

## Hometown
A brief description of your hometown.

## Local Food
A feature on local food from your hometown.

## Tourist Places
A guide to tourist attractions in your hometown.

## Style.css
```style.css
/* ========================
   Base Style
======================== */

/* Pastikan ukuran konsisten walaupun scrollbar muncul */
html {
    overflow-y: scroll;
    /* selalu ada scrollbar */
    scrollbar-gutter: stable;
    /* cegah layout shifting */
}

body {
    margin: 0;
    font-family: "Poppins", sans-serif;
    background-color: #fff;
    background-image: linear-gradient(#eee 1px, transparent 1px),
        linear-gradient(90deg, #eee 1px, transparent 1px);
    background-size: 40px 40px;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    color: #2c3e50;
}

/* ========================
   Header Top Right
======================== */
.top-right {
    position: fixed;
    top: 15px;
    right: 25px;
    display: flex;
    align-items: center;
    gap: 18px;
    font-size: 1.3rem;
    z-index: 1000;
    font-family: "Poppins", sans-serif;
    /* sama di semua halaman */
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
    /* sama dengan index */
    font-weight: 500;
    font-size: 1.1rem;
    letter-spacing: 1px;
}

/* ========================
   Center Content (Index)
======================== */
.center {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.center h1 {
    font-size: 3rem;
    margin: 0;
    font-weight: 800;
    letter-spacing: 2px;
}

.center .subtitle {
    font-size: 2rem;
    color: #666;
    margin-top: 10px;
}

/* ========================
   Bottom Navbar (global)
======================== */
.bottom-nav {
    position: fixed;
    bottom: 25px;
    left: 50%;
    transform: translateX(-50%);
    background: rgba(0, 0, 0, 0.85);
    color: white;
    padding: 12px 25px;
    border-radius: 40px;
    display: flex;
    gap: 22px;
    align-items: center;
    font-size: 0.95rem;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
    z-index: 1000;
}

.bottom-nav a {
    text-decoration: none;
    color: white;
    transition: 0.3s ease;
}

.bottom-nav a:hover {
    color: #f1ba61;
}

/* ========================
   Animations
======================== */
@keyframes fadeDown {
    0% {
        opacity: 0;
        transform: translateY(-30px);
    }

    100% {
        opacity: 1;
        transform: translateY(0);
    }
}

.fade-text {
    opacity: 0;
}

.show {
    animation: fadeDown 1s ease forwards;
}

/* ========================
   Profile Page Sections
======================== */
.profile-sections {
    overflow-y: auto;
    scroll-behavior: smooth;
    margin-left: 200px;
    margin-top: -100px;
}

.section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 60px 80px;
    gap: 40px;
}

.section-text {
    flex: 1;
    padding-left: 80px;
    /* geser agak kanan */
}

.section-text h2 {
    font-size: 2.5rem;
    margin-bottom: 20px;
}

.section-text h3 {
    font-size: 1.5rem;
    margin-top: 25px;
    margin-bottom: 10px;
    color: #555;
}

.section-text p,
.section-text ul {
    font-size: 1.2rem;
    line-height: 1.8;
    color: #333;
}

.section-text ul {
    list-style: none;
    padding: 0;
}

.section-text ul li {
    margin-bottom: 10px;
}

.section-image {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-right: 150px;
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
    transform: scale(1.05);
}

/* ========================
   Zigzag Boxes (Kiri)
======================== */
.zigzag-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    max-width: 650px;
    /* maksimal lebar */
    margin-top: 20px;
}

.zigzag-box {
    background: #eefcff;
    padding: 15px 20px;
    border-radius: 15px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    font-size: 1.1rem;
    font-weight: 500;
    color: #2c3e50;
    transition: all 0.3s ease, box-shadow 0.3s ease;
}

.zigzag-box:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
    background-color: #f3b95b;
    color: rgb(255, 255, 255);
}

/* ========================
   Gallery Zigzag (Kanan)
======================== */
.gallery-zigzag {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 25px;
    max-width: 420px;
    /* sedikit lebih besar */
    position: relative;
    margin-right: 200px;
}

.gallery-zigzag img {
    width: 180px;
    height: 180px;
    object-fit: cover;
    border-radius: 20px;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.25);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.gallery-zigzag img:nth-child(1) {
    transform: rotate(-6deg) translateY(15px);
}

.gallery-zigzag img:nth-child(2) {
    transform: rotate(5deg) translateY(-20px);
}

.gallery-zigzag img:nth-child(3) {
    transform: rotate(-4deg) translateY(25px);
}

.gallery-zigzag img:hover {
    transform: scale(1.1) rotate(0deg);
    box-shadow: 0 12px 35px rgba(0, 0, 0, 0.3);
}

/* ========================
   Responsive
======================== */
@media (max-width: 900px) {
    .section {
        flex-direction: column;
        text-align: center;
        padding: 40px 20px;
    }

    .section-text {
        padding-left: 0;
    }
}
```
