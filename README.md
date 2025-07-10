<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Testing website - Create by Prasetya</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      darkMode: 'class',
    }
  </script>
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      transition: background-color 0.5s, color 0.5s;
    }
  </style>
</head>
<body class="bg-white text-gray-800 dark:bg-gray-900 dark:text-gray-100">

  <!-- Navbar -->
  <header class="bg-white dark:bg-gray-800 shadow-md fixed w-full top-0 z-50 transition">
    <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between items-center">
      <h1 class="text-2xl font-bold text-indigo-600 dark:text-indigo-400">JUST A TESTING</h1>
      <nav class="space-x-6 hidden md:block">
        <a href="#home" class="hover:text-indigo-600 dark:hover:text-indigo-400">Home</a>
        <a href="#about" class="hover:text-indigo-600 dark:hover:text-indigo-400">About</a>
        <a href="#contact" class="hover:text-indigo-600 dark:hover:text-indigo-400">Contact</a>
      </nav>
      <button id="darkToggle" class="ml-4 px-3 py-1 border rounded-full text-sm dark:text-white">
        🌙 Dark
      </button>
    </div>
  </header>

  <!-- Hero Section -->
  <section id="home" class="h-screen flex items-center justify-center bg-gradient-to-r from-indigo-500 to-purple-600 text-white pt-20">
    <div class="text-center px-6" data-aos="fade-up">
      <h2 class="text-4xl md:text-6xl font-bold mb-4">Welcome to my website broo! hahaaha</h2>
      <p class="text-lg md:text-xl mb-6">website paling ramah.</p>
      <a href="#about" class="px-6 py-3 bg-white text-indigo-600 font-semibold rounded-full shadow hover:bg-gray-100 transition">press to scroll</a>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="py-20 bg-gray-50 dark:bg-gray-800 transition">
    <div class="max-w-5xl mx-auto px-6">
      <h3 class="text-3xl font-bold text-center mb-10 text-indigo-700 dark:text-indigo-400" data-aos="fade-down">about Us</h3>
      <div class="grid md:grid-cols-2 gap-10 items-center">
        <img src="https://images.hdqwalls.com/wallpapers/skull-monochrome-dark-art-x3.jpg" alt="About Us?" class="rounded-xl shadow-md" data-aos="zoom-in">
        <div data-aos="fade-left">
          <p class="text-lg leading-relaxed">
            Saya adalah manusia individu kreatif yang berfokus pada pengembangan website profesional dan modern. Menggabungkan estetika visual dengan performa tinggi.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-20 bg-white dark:bg-gray-900 transition">
    <div class="max-w-3xl mx-auto px-6">
      <h3 class="text-3xl font-bold text-center mb-10 text-indigo-700 dark:text-indigo-400" data-aos="fade-up">contact Us</h3>
      <form class="space-y-6" data-aos="fade-up" data-aos-delay="100">
        <input type="text" placeholder="Your name ladies and gentleman?" class="w-full border rounded-lg px-4 py-3 dark:bg-gray-800 dark:border-gray-700 dark:text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" />
        <input type="email" placeholder="Your Email" class="w-full border rounded-lg px-4 py-3 dark:bg-gray-800 dark:border-gray-700 dark:text-white focus:outline-none focus:ring-2 focus:ring-indigo-500" />
        <textarea placeholder="kasih kata kata bang!!" rows="5" class="w-full border rounded-lg px-4 py-3 dark:bg-gray-800 dark:border-gray-700 dark:text-white focus:outline-none focus:ring-2 focus:ring-indigo-500"></textarea>
        <button type="submit" class="w-full bg-indigo-600 text-white font-semibold py-3 rounded-lg hover:bg-indigo-700 transition">Sent a Message</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-100 dark:bg-gray-800 py-6 text-center text-gray-600 dark:text-gray-300 transition">
    <p>&copy; 2025 SSATFYXX INC. Dibuat dengan akal dan sedikit imajinasi.</p>
  </footer>

  <!-- Scripts -->
  <script>
    AOS.init();

    const toggle = document.getElementById('darkToggle');
    toggle.addEventListener('click', () => {
      document.documentElement.classList.toggle('dark');
    });
  </script>
</body>
</html>
