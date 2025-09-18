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
    <!-- Font Awesome untuk icon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Mono:wght@500&display=swap" rel="stylesheet">
</head>

<body>
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

    <!-- Konten utama -->
    <main class="center">
        <h1>HOSEA FELIX SANJAYA</h1>
        <h2 class="subtitle">5025241177</h2>
    </main>

    <!-- Navbar bawah -->
    <nav class="bottom-nav">
        <a href="index.html">Home</a>
        <a href="profile.html">Profile</a>
        <a href="hometown.html">Hometown</a>
        <a href="food.html">Food</a>
        <a href="tourist.html">Travel</a>
    </nav>

    <!-- Script jam interaktif -->
    <script>
        function updateClock() {
            const now = new Date();
            let hours = now.getHours();
            let minutes = now.getMinutes();
            let seconds = now.getSeconds();
            if (hours < 10) {
                hours = "0" + hours;
            }
            if (minutes < 10) {
                minutes = "0" + minutes;
            }
            if (seconds < 10) {
                seconds = "0" + seconds;
            }
            const timeString = hours + ":" + minutes + ":" + seconds;
            document.getElementById("clock").textContent = timeString;
        }
        setInterval(updateClock, 1000);
        updateClock();
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
