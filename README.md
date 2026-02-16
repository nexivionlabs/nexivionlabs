<!DOCTYPE html>
<html lang="tr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nexivion Labs | Fatih Özgel</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- Mermaid.js for Diagrams -->
    <script type="module">
        import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
        mermaid.initialize({ startOnLoad: true, theme: 'dark', securityLevel: 'loose' });
    </script>
    <style>
        body { 
            font-family: 'Inter', sans-serif;
            background: linear-gradient(-45deg, #0f172a, #1e293b, #020617, #111827);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        .glass-panel {
            background: rgba(30, 41, 59, 0.6);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .glass-panel:hover {
            background: rgba(30, 41, 59, 0.8);
            border-color: rgba(6, 182, 212, 0.3); /* Cyan border on hover */
            transform: translateY(-5px);
            box-shadow: 0 10px 40px -10px rgba(0, 0, 0, 0.5);
        }

        .nav-glass {
            background: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
        }

        /* Language Toggle Animation */
        .fade-in {
            animation: fadeIn 0.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Scroll Reveal Animation Classes */
        .reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease-out;
        }
        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body class="text-slate-200 antialiased min-h-screen relative selection:bg-cyan-500 selection:text-white">

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 w-full z-50 nav-glass transition-all duration-300" id="navbar">
        <div class="max-w-4xl mx-auto px-4 py-3 flex justify-between items-center">
            <a href="#" class="text-xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-cyan-400 to-blue-500 hover:opacity-80 transition-opacity">
                Nexivion Labs
            </a>
            
            <div class="flex items-center gap-6">
                <!-- Desktop Menu -->
                <div class="hidden md:flex gap-6 text-sm font-medium text-slate-400">
                    <a href="#about" class="hover:text-cyan-400 transition-colors"><span class="lang-tr">Hakkımda</span><span class="lang-en hidden">About</span></a>
                    <a href="#stack" class="hover:text-cyan-400 transition-colors"><span class="lang-tr">Teknolojiler</span><span class="lang-en hidden">Stack</span></a>
                    <a href="#projects" class="hover:text-cyan-400 transition-colors"><span class="lang-tr">Projeler</span><span class="lang-en hidden">Projects</span></a>
                    <a href="#contact" class="hover:text-cyan-400 transition-colors"><span class="lang-tr">İletişim</span><span class="lang-en hidden">Contact</span></a>
                </div>

                <!-- Language Button -->
                <button onclick="toggleLanguage()" class="px-3 py-1 rounded-full border border-slate-700 bg-slate-800/50 hover:bg-slate-700 text-xs font-bold text-cyan-400 transition-all flex items-center gap-2">
                    <span id="lang-icon">🇹🇷</span>
                    <span id="lang-text">TR</span>
                </button>
            </div>
        </div>
    </nav>

    <!-- Scroll to Top Button -->
    <button id="scrollToTopBtn" onclick="window.scrollTo({top: 0, behavior: 'smooth'})" class="fixed bottom-8 right-8 z-40 bg-cyan-600 hover:bg-cyan-500 text-white p-3 rounded-full shadow-lg opacity-0 transition-opacity duration-300 pointer-events-none translate-y-10">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18" />
        </svg>
    </button>

    <!-- Main Container -->
    <div class="max-w-4xl mx-auto px-4 pt-28 pb-12 space-y-16">

        <!-- Hero Section -->
        <header class="text-center space-y-8 reveal active">
            <div class="relative inline-block group">
                <div class="absolute -inset-1 bg-gradient-to-r from-cyan-400 to-blue-600 rounded-lg blur opacity-25 group-hover:opacity-50 transition duration-1000 group-hover:duration-200"></div>
                <h1 class="relative text-5xl md:text-6xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 via-blue-400 to-cyan-400 bg-300% animate-gradient">
                    🚀 Nexivion Labs
                </h1>
            </div>
            
            <div class="flex justify-center h-16">
                <img src="https://readme-typing-svg.herokuapp.com?size=26&duration=3000&color=00C4FF&center=true&vCenter=true&width=700&lines=Full+Stack+Developer;AI-Oriented+Backend+Architect;Flutter+%7C+FastAPI+%7C+AI+Systems;Building+Systems%2C+Not+Just+Apps" alt="Typing Animation" class="max-w-full">
            </div>
        </header>

        <!-- Vision Section -->
        <section id="vision" class="glass-panel p-8 rounded-2xl shadow-lg text-center reveal">
            <h2 class="text-2xl font-bold text-white mb-4 flex justify-center items-center gap-2">
                <span>🌟</span> <span class="lang-tr">Vizyon</span><span class="lang-en hidden">Vision</span>
            </h2>
            
            <p class="lang-tr text-lg text-slate-300 leading-relaxed fade-in">
                <strong class="text-cyan-400">Nexivion</strong>, geliştiriciler için akıllı dijital sistemler ve araçlar oluşturmaya odaklanmış, AI-öncelikli bir platform ve ekosistemdir. Açık kaynak topluluklarına katkıda bulunmayı ve ölçeklenebilir, yapay zeka odaklı ürünler geliştirmeyi vizyon ediniyoruz.
            </p>
            
            <p class="lang-en hidden text-lg text-slate-300 leading-relaxed fade-in">
                <strong class="text-cyan-400">Nexivion</strong> is an AI-first platform and ecosystem focused on building intelligent digital systems and tools for developers. We envision contributing to open-source communities and building scalable, AI-driven products.
            </p>
        </section>

        <!-- About Me Section -->
        <section id="about" class="glass-panel p-8 rounded-2xl shadow-lg reveal">
            <div class="flex flex-col md:flex-row items-center gap-10">
                <!-- Profile Image with Glow -->
                <div class="relative group flex-shrink-0">
                    <div class="absolute -inset-0.5 bg-gradient-to-r from-cyan-500 to-blue-500 rounded-2xl blur opacity-30 group-hover:opacity-75 transition duration-500"></div>
                    <div class="relative">
                        <img src="assets/fatih.jpg" onerror="this.src='https://ui-avatars.com/api/?name=Fatih+Ozgel&background=0D8ABC&color=fff&size=200'" alt="Fatih Özgel" class="w-48 h-48 rounded-2xl object-cover shadow-2xl bg-slate-800">
                    </div>
                    <h3 class="mt-4 text-center text-xl font-bold text-white">Fatih Özgel</h3>
                </div>
                
                <!-- Bio Text -->
                <div class="flex-grow text-center md:text-left">
                    <h3 class="text-2xl font-bold text-cyan-400 mb-4">Full Stack & AI-Oriented Developer</h3>
                    
                    <div class="lang-tr fade-in">
                        <p class="text-slate-300 mb-6 leading-relaxed">
                            Ben sadece endpoint'ler değil, <b class="text-white">yaşayan sistemler</b> tasarlamaya odaklanmış bir geliştiriciyim. Çalışmalarım temiz mimariyi, yapay zeka karar katmanlarını ve mobil/frontend deneyimini birleştirir.
                        </p>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-3 text-sm">
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">🧠</span> <b>Core Focus:</b> Temiz Mimari</div>
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">🤖</span> <b>AI Integration:</b> Karar Katmanları</div>
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">📱</span> <b>Mobile:</b> Flutter & Dart</div>
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">🏗️</span> <b>Scalability:</b> Sistem Tasarımı</div>
                        </div>
                    </div>

                    <div class="lang-en hidden fade-in">
                        <p class="text-slate-300 mb-6 leading-relaxed">
                            I am a developer focused on designing <b class="text-white">living systems</b>, not just endpoints. My work combines clean architecture, AI decision layers, and mobile/frontend experience.
                        </p>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-3 text-sm">
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">🧠</span> <b>Core Focus:</b> Clean Architecture</div>
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">🤖</span> <b>AI Integration:</b> Decision Layers</div>
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">📱</span> <b>Mobile:</b> Flutter & Dart</div>
                            <div class="bg-slate-800/40 p-3 rounded-lg border border-slate-700/50"><span class="mr-2">🏗️</span> <b>Scalability:</b> System Design</div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Tech Stack Section -->
        <section id="stack" class="space-y-8 reveal">
            <h2 class="text-3xl font-bold text-center text-white mb-8 relative">
                <span class="bg-clip-text text-transparent bg-gradient-to-r from-slate-200 to-slate-400">
                    <span class="lang-tr">Teknoloji Yığını</span><span class="lang-en hidden">Tech Stack</span>
                </span>
            </h2>

            <div class="grid md:grid-cols-2 gap-6">
                <!-- Backend -->
                <div class="glass-panel p-6 rounded-xl hover:shadow-cyan-500/10">
                    <h3 class="text-xl font-semibold text-cyan-400 mb-4 border-b border-slate-700 pb-2 flex items-center gap-2">
                        🔧 <span>Backend & AI</span>
                    </h3>
                    <div class="flex flex-wrap gap-2">
                        <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=chainlink&logoColor=white" class="hover:scale-105 transition-transform">
                    </div>
                </div>

                <!-- Frontend -->
                <div class="glass-panel p-6 rounded-xl hover:shadow-blue-500/10">
                    <h3 class="text-xl font-semibold text-blue-400 mb-4 border-b border-slate-700 pb-2 flex items-center gap-2">
                        🎨 <span>Frontend & Mobile</span>
                    </h3>
                    <div class="flex flex-wrap gap-2">
                        <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" class="hover:scale-105 transition-transform">
                    </div>
                </div>

                <!-- Tools - Full Width on Mobile, Centered below on Desktop if wanted, or just part of grid -->
                <div class="glass-panel p-6 rounded-xl md:col-span-2 hover:shadow-yellow-500/10">
                    <h3 class="text-xl font-semibold text-yellow-400 mb-4 border-b border-slate-700 pb-2 flex items-center gap-2">
                        🛠️ <span>Tools & DevOps</span>
                    </h3>
                    <div class="flex flex-wrap gap-2">
                        <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" class="hover:scale-105 transition-transform">
                        <img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" class="hover:scale-105 transition-transform">
                    </div>
                </div>
            </div>
        </section>

        <!-- Featured Project -->
        <section id="projects" class="glass-panel p-8 rounded-2xl shadow-lg border-l-4 border-cyan-500 reveal">
            <div class="flex justify-between items-start mb-6">
                <h2 class="text-2xl font-bold text-white">🚀 Featured Project: Nexivion Backend</h2>
                <span class="bg-cyan-500/20 text-cyan-300 text-xs px-2 py-1 rounded border border-cyan-500/30">v1.0 Beta</span>
            </div>
            
            <div class="lang-tr fade-in">
                <p class="text-slate-300 mb-8 text-lg">
                    Kullanıcı niyetini anlayan ve akıllı sistem kararları üreten AI-öncelikli backend mimarisi.
                </p>
                <div class="grid md:grid-cols-3 gap-6 mb-8">
                    <div class="bg-slate-800/50 p-5 rounded-xl border border-white/5 hover:border-cyan-500/30 transition-colors">
                        <div class="text-2xl mb-2">🎯</div>
                        <h4 class="font-bold text-cyan-400 mb-1">Niyet Analizi</h4>
                        <p class="text-sm text-slate-400">Statik mantık yerine dinamik AI karar mekanizması.</p>
                    </div>
                    <div class="bg-slate-800/50 p-5 rounded-xl border border-white/5 hover:border-cyan-500/30 transition-colors">
                        <div class="text-2xl mb-2">⚡</div>
                        <h4 class="font-bold text-cyan-400 mb-1">Yüksek Performans</h4>
                        <p class="text-sm text-slate-400">FastAPI tabanlı asenkron yapı.</p>
                    </div>
                    <div class="bg-slate-800/50 p-5 rounded-xl border border-white/5 hover:border-cyan-500/30 transition-colors">
                        <div class="text-2xl mb-2">🧩</div>
                        <h4 class="font-bold text-cyan-400 mb-1">Modular Design</h4>
                        <p class="text-sm text-slate-400">Geliştirici dostu SDK entegrasyonu.</p>
                    </div>
                </div>
            </div>

            <div class="lang-en hidden fade-in">
                <p class="text-slate-300 mb-8 text-lg">
                    AI-first backend architecture designed to understand user intent and produce intelligent decisions.
                </p>
                <div class="grid md:grid-cols-3 gap-6 mb-8">
                    <div class="bg-slate-800/50 p-5 rounded-xl border border-white/5 hover:border-cyan-500/30 transition-colors">
                        <div class="text-2xl mb-2">🎯</div>
                        <h4 class="font-bold text-cyan-400 mb-1">Intent Analysis</h4>
                        <p class="text-sm text-slate-400">Dynamic AI decision engine instead of static logic.</p>
                    </div>
                    <div class="bg-slate-800/50 p-5 rounded-xl border border-white/5 hover:border-cyan-500/30 transition-colors">
                        <div class="text-2xl mb-2">⚡</div>
                        <h4 class="font-bold text-cyan-400 mb-1">High Performance</h4>
                        <p class="text-sm text-slate-400">FastAPI-based asynchronous architecture.</p>
                    </div>
                    <div class="bg-slate-800/50 p-5 rounded-xl border border-white/5 hover:border-cyan-500/30 transition-colors">
                        <div class="text-2xl mb-2">🧩</div>
                        <h4 class="font-bold text-cyan-400 mb-1">Modular Design</h4>
                        <p class="text-sm text-slate-400">Developer-friendly SDK integration.</p>
                    </div>
                </div>
            </div>

            <h3 class="text-xl font-bold text-white mb-4 flex items-center gap-2">
                <span>🧩</span> <span class="lang-tr">Sistem Mimarisi</span><span class="lang-en hidden">System Architecture</span>
            </h3>
            <div class="bg-[#0f172a] p-4 rounded-xl overflow-x-auto border border-slate-700 shadow-inner">
                <div class="mermaid">
                    flowchart TD
                    Client[Client / Mobile / Web] -- Request --> API[FastAPI Routers]
                    API -- Validation --> Schemas[Pydantic Models]
                    Schemas -- Logic --> Services[Service Layer]
                    
                    subgraph Engine[Nexivion Core]
                    Services --> AI[AI Decision Engine]
                    Services --> Logic[Business Logic]
                    end
                    
                    AI -- Strategy --> Response[Final Decision]
                    Logic -- Data --> Response
                    
                    Response -- Result --> API
                    API -- Response --> Client
                    
                    classDef default fill:#1e293b,stroke:#38bdf8,color:#fff;
                    classDef subgraphStyle fill:#0f172a,stroke:#64748b,color:#fff,stroke-dasharray: 5 5;
                    class Engine subgraphStyle;
                </div>
            </div>
        </section>

        <!-- Roadmap -->
        <section class="glass-panel p-6 rounded-2xl reveal">
            <h2 class="text-2xl font-bold text-white mb-6">🗺️ Roadmap</h2>
            
            <div class="space-y-4">
                <!-- Checkbox Style List -->
                <div class="lang-tr space-y-3 fade-in">
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">AI Decision Engine v1</strong> - Dinamik niyet çözümleme motoru.</span>
                    </div>
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">Developer SDK</strong> - Diğer projeler için kolay entegrasyon kütüphanesi.</span>
                    </div>
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">Open-source Flutter Integrations</strong> - Hazır AI-ready UI bileşenleri.</span>
                    </div>
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">Community Tools</strong> - Geliştiriciler için açık kaynaklı verimlilik araçları.</span>
                    </div>
                </div>

                <div class="lang-en hidden space-y-3 fade-in">
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">AI Decision Engine v1</strong> - Dynamic intent resolution engine.</span>
                    </div>
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">Developer SDK</strong> - Easy integration library.</span>
                    </div>
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">Open-source Flutter Integrations</strong> - Ready-to-use AI UI components.</span>
                    </div>
                    <div class="flex items-center gap-3 p-3 rounded-lg hover:bg-white/5 transition-colors">
                        <div class="w-6 h-6 rounded border-2 border-slate-600 flex items-center justify-center bg-slate-800"></div>
                        <span class="text-slate-300"><strong class="text-white">Community Tools</strong> - Open-source tools for developers.</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- GitHub Stats -->
        <section class="text-center space-y-6 reveal">
            <h2 class="text-2xl font-bold text-white">📊 GitHub Stats</h2>
            <div class="flex justify-center items-center gap-4 hover:scale-105 transition-transform duration-300">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=nexivionlabs&theme=tokyonight" class="h-44 shadow-2xl rounded-lg" alt="GitHub Streak">
            </div>
        </section>

        <!-- Connect Footer -->
        <footer id="contact" class="text-center pt-10 pb-12 border-t border-slate-800 reveal">
            <h2 class="text-3xl font-bold text-white mb-8">🌐 <span class="lang-tr">İletişim & Topluluk</span><span class="lang-en hidden">Connect & Community</span></h2>
            
            <div class="flex flex-wrap justify-center gap-6 mb-8">
                <!-- Social Links with Hover Effects -->
                <a href="https://github.com/nexivionlabs" target="_blank" class="group relative">
                    <div class="absolute -inset-2 bg-purple-500 rounded-full blur opacity-20 group-hover:opacity-60 transition duration-200"></div>
                    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" class="relative block transform group-hover:scale-110 transition-transform shadow-lg" alt="GitHub">
                </a>
                
                <a href="https://www.linkedin.com/in/fatihozgel" target="_blank" class="group relative">
                    <div class="absolute -inset-2 bg-blue-600 rounded-full blur opacity-20 group-hover:opacity-60 transition duration-200"></div>
                    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" class="relative block transform group-hover:scale-110 transition-transform shadow-lg" alt="LinkedIn">
                </a>
                
                <a href="https://x.com/fatihozgell" target="_blank" class="group relative">
                    <div class="absolute -inset-2 bg-white rounded-full blur opacity-10 group-hover:opacity-40 transition duration-200"></div>
                    <img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" class="relative block transform group-hover:scale-110 transition-transform shadow-lg" alt="X">
                </a>

                <a href="https://www.instagram.com/nexivion/" target="_blank" class="group relative">
                    <div class="absolute -inset-2 bg-pink-500 rounded-full blur opacity-20 group-hover:opacity-60 transition duration-200"></div>
                    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" class="relative block transform group-hover:scale-110 transition-transform shadow-lg" alt="Instagram">
                </a>
            </div>

            <!-- Emails -->
            <div class="flex flex-wrap justify-center gap-4 mb-10">
                <a href="mailto:fatih@nexivionlabs.com" class="hover:opacity-80 transition-opacity">
                    <img src="https://img.shields.io/badge/Email-fatih%40nexivionlabs.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
                </a>
                <a href="mailto:nexivion.dev@gmail.com" class="hover:opacity-80 transition-opacity">
                    <img src="https://img.shields.io/badge/Email-nexivion.dev%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
                </a>
            </div>

            <p class="text-slate-500 text-sm italic">
                &copy; <span id="year"></span> Nexivion Labs. "Building Systems, Not Just Apps."
            </p>
        </footer>

    </div>

    <script>
        // Set Current Year
        document.getElementById('year').textContent = new Date().getFullYear();

        // Language Toggle Logic
        function toggleLanguage() {
            const trElements = document.querySelectorAll('.lang-tr');
            const enElements = document.querySelectorAll('.lang-en');
            const langIcon = document.getElementById('lang-icon');
            const langText = document.getElementById('lang-text');

            const isEnglish = langText.innerText === 'EN';

            if (isEnglish) {
                // Switch to Turkish
                trElements.forEach(el => el.classList.remove('hidden'));
                enElements.forEach(el => el.classList.add('hidden'));
                langIcon.innerText = '🇹🇷';
                langText.innerText = 'TR';
            } else {
                // Switch to English
                trElements.forEach(el => el.classList.add('hidden'));
                enElements.forEach(el => el.classList.remove('hidden'));
                langIcon.innerText = '🇺🇸';
                langText.innerText = 'EN';
            }
        }

        // Scroll Animation Observer
        const observerOptions = {
            threshold: 0.1,
            rootMargin: "0px 0px -50px 0px"
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.reveal').forEach(el => {
            observer.observe(el);
        });

        // Show/Hide Scroll to Top Button
        const scrollToTopBtn = document.getElementById('scrollToTopBtn');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 300) {
                scrollToTopBtn.classList.remove('opacity-0', 'pointer-events-none', 'translate-y-10');
            } else {
                scrollToTopBtn.classList.add('opacity-0', 'pointer-events-none', 'translate-y-10');
            }
        });
    </script>
</body>
</html>
