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
        <a href="https://www.instagram.com/hoseafelix_/" target="_blank">
            <i class="fab fa-instagram"></i>
        </a>
        <a href="https://github.com/Pascalllllll" target="_blank">
            <i class="fab fa-github"></i>
        </a>
        <a href="https://www.linkedin.com/in/hosea-felix-sanjaya-3a9a0931b" target="_blank">
            <i class="fab fa-linkedin"></i>
        </a>
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
        // Jam
        function updateClock() {
            const now = new Date();
            let h = String(now.getHours()).padStart(2, "0");
            let m = String(now.getMinutes()).padStart(2, "0");
            let s = String(now.getSeconds()).padStart(2, "0");
            document.getElementById("clock").textContent = `${h}:${m}:${s}`;
        }
        setInterval(updateClock, 1000);
        updateClock();

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
Information about yourself.

## Hometown
A brief description of your hometown.

## Local Food
A feature on local food from your hometown.

## Tourist Places
A guide to tourist attractions in your hometown.

## Style.css
```style.css
/* Base */
body {
    margin: 0;
    font-family: "Poppins", sans-serif;
    background-color: #fff;
    background-image: linear-gradient(#eee 1px, transparent 1px), linear-gradient(90deg, #eee 1px, transparent 1px);
    background-size: 40px 40px;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

/* Top Right */
.top-right {
    position: absolute;
    top: 20px;
    right: 30px;
    display: flex;
    align-items: center;
    gap: 18px;
    font-size: 1.3rem;
}

.top-right a {
    color: #333;
    transition: color 0.3s ease;
}

.top-right a:hover {
    color: #f39c12;
}

#clock {
    font-family: "Poppins", sans-serif;
    font-weight: 700;
    font-size: 1.1rem;
    letter-spacing: 1px;
    color: #2c3e50;
}

/* Center Content */
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

/* Bottom Navbar */
.bottom-nav {
    position: fixed;
    bottom: 25px;
    left: 50%;
    transform: translateX(-50%);
    background: rgba(0, 0, 0, 0.85);
    color: white;
    padding: 14px 30px;
    border-radius: 40px;
    display: flex;
    gap: 25px;
    align-items: center;
    font-size: 0.95rem;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
}

.bottom-nav a {
    text-decoration: none;
    color: white;
    transition: 0.3s ease;
}

.bottom-nav a:hover {
    color: #f39c12;
}

/* Animasi fade dari atas */
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

.subtitle {
    font-size: 2rem;
    color: #666;
    margin-top: 15px;
}




/* Profile Page Layout */
.profile-container {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 50px; /* jarak foto dan teks */
    padding: 80px 100px; /* ruang atas-bawah & kiri-kanan */
    max-width: 1200px;
    margin: 0 auto;
}

.profile-photo img {
    width: 250px;   /* diperbesar dari default (misalnya 180px) */
    height: 250px;
    border-radius: 50%; /* tetap lingkaran */
    object-fit: cover;
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease;
}

.profile-photo img:hover {
    transform: scale(1.05); /* efek hover membesar sedikit */
}

.profile-info h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

.profile-info h2 {
    font-size: 1.5rem;
    margin-bottom: 20px;
    color: #555;
}

.profile-info p {
    font-size: 1.1rem;
    line-height: 1.7;
    color: #333;
    max-width: 600px;
}

```
