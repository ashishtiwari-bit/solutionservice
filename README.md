# solutionservice
This is my 1st one github project
Auther-Ashish Tiwari

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome to My Website</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        body { font-family: 'Inter', sans-serif; }
        .gradient-bg { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); }
        .card-hover { transition: transform 0.3s ease, box-shadow 0.3s ease; }
        .card-hover:hover { transform: translateY(-5px); box-shadow: 0 20px 40px rgba(0,0,0,0.1); }
    </style>
</head>
<body class="bg-gray-50">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex items-center">
                    <div class="text-2xl font-bold text-indigo-600">MyWebsite</div>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-8">
                        <a href="#home" class="text-gray-700 hover:text-indigo-600 px-3 py-2 text-sm font-medium transition-colors">Home</a>
                        <a href="#about" class="text-gray-700 hover:text-indigo-600 px-3 py-2 text-sm font-medium transition-colors">About</a>
                        <a href="#services" class="text-gray-700 hover:text-indigo-600 px-3 py-2 text-sm font-medium transition-colors">Services</a>
                        <a href="#contact" class="text-gray-700 hover:text-indigo-600 px-3 py-2 text-sm font-medium transition-colors">Contact</a>
                    </div>
                </div>
                <button id="mobile-menu-btn" class="md:hidden text-gray-700 hover:text-indigo-600">
                    <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                    </svg>
                </button>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-white border-t">
            <div class="px-2 pt-2 pb-3 space-y-1">
                <a href="#home" class="block px-3 py-2 text-gray-700 hover:text-indigo-600">Home</a>
                <a href="#about" class="block px-3 py-2 text-gray-700 hover:text-indigo-600">About</a>
                <a href="#services" class="block px-3 py-2 text-gray-700 hover:text-indigo-600">Services</a>
                <a href="#contact" class="block px-3 py-2 text-gray-700 hover:text-indigo-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="gradient-bg text-white py-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h1 class="text-5xl md:text-6xl font-bold mb-6">Welcome to Our Website</h1>
            <p class="text-xl md:text-2xl mb-8 opacity-90">Creating amazing digital experiences that inspire and engage</p>
            <button onclick="scrollToSection('about')" class="bg-white text-indigo-600 px-8 py-3 rounded-full font-semibold text-lg hover:bg-gray-100 transition-colors shadow-lg">
                Get Started
            </button>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-900 mb-4">About Us</h2>
                <p class="text-xl text-gray-600 max-w-3xl mx-auto">We're passionate about creating exceptional digital experiences that make a difference in people's lives.</p>
            </div>
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div>
                    <h3 class="text-2xl font-semibold text-gray-900 mb-4">Our Mission</h3>
                    <p class="text-gray-600 mb-6">To deliver innovative solutions that empower businesses and individuals to achieve their goals through cutting-edge technology and thoughtful design.</p>
                    <div class="space-y-4">
                        <div class="flex items-center">
                            <div class="w-2 h-2 bg-indigo-600 rounded-full mr-3"></div>
                            <span class="text-gray-700">Innovation-driven approach</span>
                        </div>
                        <div class="flex items-center">
                            <div class="w-2 h-2 bg-indigo-600 rounded-full mr-3"></div>
                            <span class="text-gray-700">Customer-focused solutions</span>
                        </div>
                        <div class="flex items-center">
                            <div class="w-2 h-2 bg-indigo-600 rounded-full mr-3"></div>
                            <span class="text-gray-700">Quality and excellence</span>
                        </div>
                    </div>
                </div>
                <div class="bg-gradient-to-br from-indigo-100 to-purple-100 p-8 rounded-2xl">
                    <div class="text-center">
                        <div class="text-6xl mb-4">🚀</div>
                        <h4 class="text-xl font-semibold text-gray-900 mb-2">Ready to Launch</h4>
                        <p class="text-gray-600">We're here to help you succeed with our expertise and dedication.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-900 mb-4">Our Services</h2>
                <p class="text-xl text-gray-600">Comprehensive solutions tailored to your needs</p>
            </div>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">💻</div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Web Development</h3>
                    <p class="text-gray-600 mb-4">Custom websites and web applications built with modern technologies and best practices.</p>
                    <button onclick="showServiceDetails('web')" class="text-indigo-600 font-medium hover:text-indigo-800 transition-colors">Learn More →</button>
                </div>
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">📱</div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Mobile Apps</h3>
                    <p class="text-gray-600 mb-4">Native and cross-platform mobile applications that deliver exceptional user experiences.</p>
                    <button onclick="showServiceDetails('mobile')" class="text-indigo-600 font-medium hover:text-indigo-800 transition-colors">Learn More →</button>
                </div>
                <div class="bg-white p-8 rounded-2xl shadow-lg card-hover">
                    <div class="text-4xl mb-4">🎨</div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">UI/UX Design</h3>
                    <p class="text-gray-600 mb-4">Beautiful, intuitive designs that enhance user engagement and satisfaction.</p>
                    <button onclick="showServiceDetails('design')" class="text-indigo-600 font-medium hover:text-indigo-800 transition-colors">Learn More →</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl font-bold text-gray-900 mb-4">Get In Touch</h2>
                <p class="text-xl text-gray-600">Ready to start your project? We'd love to hear from you!</p>
            </div>
            <div class="max-w-2xl mx-auto">
                <form id="contact-form" class="space-y-6">
                    <div class="grid md:grid-cols-2 gap-6">
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Name</label>
                            <input type="text" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent transition-colors">
                        </div>
                        <div>
                            <label class="block text-sm font-medium text-gray-700 mb-2">Email</label>
                            <input type="email" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent transition-colors">
                        </div>
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-gray-700 mb-2">Subject</label>
                        <input type="text" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent transition-colors">
                    </div>
                    <div>
                        <label class="block text-sm font-medium text-gray-700 mb-2">Message</label>
                        <textarea rows="5" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-indigo-500 focus:border-transparent transition-colors resize-none"></textarea>
                    </div>
                    <div class="text-center">
                        <button type="submit" class="bg-indigo-600 text-white px-8 py-3 rounded-lg font-semibold hover:bg-indigo-700 transition-colors shadow-lg">
                            Send Message
                        </button>
                    </div>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-4 gap-8">
                <div>
                    <div class="text-2xl font-bold mb-4">MyWebsite</div>
                    <p class="text-gray-400">Creating amazing digital experiences since 2024.</p>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Quick Links</h4>
                    <div class="space-y-2">
                        <a href="#home" class="block text-gray-400 hover:text-white transition-colors">Home</a>
                        <a href="#about" class="block text-gray-400 hover:text-white transition-colors">About</a>
                        <a href="#services" class="block text-gray-400 hover:text-white transition-colors">Services</a>
                    </div>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Services</h4>
                    <div class="space-y-2">
                        <span class="block text-gray-400">Web Development</span>
                        <span class="block text-gray-400">Mobile Apps</span>
                        <span class="block text-gray-400">UI/UX Design</span>
                    </div>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Contact Info</h4>
                    <div class="space-y-2 text-gray-400">
                        <p>📧 hello@mywebsite.com</p>
                        <p>📞 (555) 123-4567</p>
                        <p>📍 123 Web Street, Digital City</p>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-800 mt-8 pt-8 text-center text-gray-400">
                <p>&copy; 2024 MyWebsite. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Service Details Modal -->
    <div id="service-modal" class="fixed inset-0 bg-black bg-opacity-50 hidden items-center justify-center z-50">
        <div class="bg-white rounded-2xl p-8 max-w-md mx-4">
            <div class="text-center">
                <div id="modal-icon" class="text-6xl mb-4"></div>
                <h3 id="modal-title" class="text-2xl font-bold text-gray-900 mb-4"></h3>
                <p id="modal-description" class="text-gray-600 mb-6"></p>
                <button onclick="closeModal()" class="bg-indigo-600 text-white px-6 py-2 rounded-lg hover:bg-indigo-700 transition-colors">
                    Close
                </button>
            </div>
        </div>
    </div>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-btn').addEventListener('click', function() {
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenu.classList.toggle('hidden');
        });

        // Smooth scrolling for navigation links
        function scrollToSection(sectionId) {
            document.getElementById(sectionId).scrollIntoView({
                behavior: 'smooth'
            });
        }

        // Add smooth scrolling to all navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
                // Close mobile menu if open
                document.getElementById('mobile-menu').classList.add('hidden');
            });
        });

        // Service details modal
        function showServiceDetails(service) {
            const modal = document.getElementById('service-modal');
            const icon = document.getElementById('modal-icon');
            const title = document.getElementById('modal-title');
            const description = document.getElementById('modal-description');

            const serviceDetails = {
                web: {
                    icon: '💻',
                    title: 'Web Development',
                    description: 'We create responsive, fast, and secure websites using the latest technologies. From simple landing pages to complex web applications, we deliver solutions that drive results.'
                },
                mobile: {
                    icon: '📱',
                    title: 'Mobile Apps',
                    description: 'Our mobile app development services cover iOS and Android platforms. We build user-friendly apps that provide seamless experiences across all devices.'
                },
                design: {
                    icon: '🎨',
                    title: 'UI/UX Design',
                    description: 'We design beautiful and intuitive user interfaces that enhance user experience. Our design process focuses on usability, accessibility, and visual appeal.'
                }
            };

            const details = serviceDetails[service];
            icon.textContent = details.icon;
            title.textContent = details.title;
            description.textContent = details.description;

            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeModal() {
            const modal = document.getElementById('service-modal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }

        // Close modal when clicking outside
        document.getElementById('service-modal').addEventListener('click', function(e) {
            if (e.target === this) {
                closeModal();
            }
        });

        // Contact form submission
        document.getElementById('contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Show success message
            const button = this.querySelector('button[type="submit"]');
            const originalText = button.textContent;
            button.textContent = 'Message Sent! ✓';
            button.classList.remove('bg-indigo-600', 'hover:bg-indigo-700');
            button.classList.add('bg-green-600');
            
            // Reset form
            this.reset();
            
            // Reset button after 3 seconds
            setTimeout(() => {
                button.textContent = originalText;
                button.classList.remove('bg-green-600');
                button.classList.add('bg-indigo-600', 'hover:bg-indigo-700');
            }, 3000);
        });

        // Add scroll effect to navigation
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('nav');
            if (window.scrollY > 100) {
                nav.classList.add('shadow-xl');
            } else {
                nav.classList.remove('shadow-xl');
            }
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9663e16f940fff68',t:'MTc1MzcwMDUwOC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
