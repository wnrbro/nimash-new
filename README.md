<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>W. Nimash Rashmika - Personal Brand</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Poppins', 'sans-serif'],
                    },
                    colors: {
                        primary: '#3B82F6',
                        secondary: '#10B981',
                    },
                }
            }
        }
    </script>
</head>
<body class="bg-gray-100 font-sans">
    <header class="bg-white shadow-md fixed w-full z-10">
        <nav class="container mx-auto px-6 py-3">
            <div class="flex justify-between items-center">
                <a href="#" class="text-2xl font-bold text-primary">NR</a>
                <div class="hidden md:flex space-x-4">
                    <a href="#about" class="text-gray-700 hover:text-primary transition">About</a>
                    <a href="#academics" class="text-gray-700 hover:text-primary transition">Academics</a>
                    <a href="#interests" class="text-gray-700 hover:text-primary transition">Interests</a>
                    <a href="#contact" class="text-gray-700 hover:text-primary transition">Contact</a>
                </div>
                <button class="md:hidden focus:outline-none">
                    <svg class="h-6 w-6 fill-current text-gray-700" viewBox="0 0 24 24">
                        <path d="M4 6h16M4 12h16M4 18h16" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                </button>
            </div>
        </nav>
    </header>

    <main>
        <section id="hero" class="bg-gradient-to-r from-primary to-secondary text-white min-h-screen flex items-center">
            <div class="container mx-auto px-6 text-center">
                <h1 class="text-5xl md:text-6xl font-bold mb-4">W. Nimash Rashmika</h1>
                <p class="text-xl md:text-2xl mb-8">A Journey of Determination and Passion</p>
                <a href="#about" class="bg-white text-primary px-6 py-3 rounded-full font-semibold hover:bg-gray-100 transition">Learn More</a>
            </div>
        </section>

        <section id="about" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl font-bold text-center mb-8">About Me</h2>
                <div class="max-w-3xl mx-auto text-gray-700 leading-relaxed">
                    <p class="mb-4">I'm a 19-year-old from Ambalangoda, Sri Lanka, driven by curiosity and dedication. Currently, I'm preparing for my Advanced Level (A/L) exams in 2024, focusing on the Maths stream with a special interest in ICT.</p>
                    <p>My journey is defined by a balance between academic pursuits and personal interests, always striving for excellence and growth in everything I do.</p>
                </div>
            </div>
        </section>

        <section id="academics" class="bg-white py-20">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl font-bold text-center mb-8">Academic Achievements</h2>
                <div class="grid md:grid-cols-2 gap-8">
                    <div class="bg-gray-100 p-6 rounded-lg">
                        <h3 class="text-xl font-semibold mb-4">O/L Exams (2021)</h3>
                        <ul class="list-disc list-inside text-gray-700">
                            <li>Science -      A</li>
                            <li>Mathamatics -  A</li>
                            <li>ICT -          A</li>
                            <li>Music -        A</li>
                            <li>Buddisum -     A</li>
                            <li>Sinhala -      A</li>
                            <li>Commerce -     A</li>
                            <li>English -      B</li>
                            <li>Histriy -      C</li>
                        </ul>
                    </div>
                    <div class="bg-gray-100 p-6 rounded-lg">
                        <h3 class="text-xl font-semibold mb-4">A/L Preparation</h3>
                        <p class="text-gray-700">Currently focusing on the Maths stream, with a special emphasis on ICT for the upcoming 2024 exams.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="interests" class="py-20">
            <div class="container mx-auto px-6">
                <h2 class="text-3xl font-bold text-center mb-8">Interests & Hobbies</h2>
                <div class="grid md:grid-cols-2 gap-8">
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold mb-4">Video Gaming</h3>
                        <p class="text-gray-700">A passionate gamer, finding balance and creativity in virtual worlds.</p>
                    </div>
                    <div class="bg-white p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-semibold mb-4">YouTube Channel</h3>
                        <p class="text-gray-700">"Rash Collection" - Sharing gaming experiences with 1.6K subscribers.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="bg-gray-800 text-white py-20">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-3xl font-bold mb-8">Get In Touch</h2>
                <p class="mb-8">Interested in connecting or collaborating? Feel free to reach out!</p>
                <a href="mailto:contact@nimashrashmika.com" class="bg-primary text-white px-6 py-3 rounded-full font-semibold hover:bg-blue-600 transition">Contact Me</a>
            </div>
        </section>
    </main>

    <footer class="bg-gray-900 text-white py-6">
        <div class="container mx-auto px-6 text-center">
            <p>&copy; 2023 W. Nimash Rashmika. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Simple scroll animation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Mobile menu toggle
        const mobileMenuButton = document.querySelector('button');
        const mobileMenu = document.querySelector('.md\\:flex');
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
    </script>
</body>
</html>
