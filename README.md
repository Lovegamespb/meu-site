# meu-site<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LoveGamesPB - Tudo sobre jogos de todas as gerações</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #0f172a;
            color: #e2e8f0;
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #1e3a8a 0%, #7c3aed 50%, #db2777 100%);
        }
        
        .game-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.3);
        }
        
        .game-card {
            transition: all 0.3s ease;
        }
        
        .console-icon {
            filter: drop-shadow(0 0 8px rgba(255, 255, 255, 0.3));
        }
        
        .nav-link:hover {
            color: #db2777;
        }
        
        .pulse {
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.05);
            }
            100% {
                transform: scale(1);
            }
        }
    </style>
</head>
<body>
    <!-- Header/Navigation -->
    <header class="bg-gray-900 sticky top-0 z-50 shadow-lg">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <i class="fas fa-gamepad text-purple-500 text-2xl"></i>
                <h1 class="text-2xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-purple-400 to-pink-600">
                    LoveGamesPB
                </h1>
            </div>
            
            <nav class="hidden md:flex space-x-8">
                <a href="#home" class="nav-link text-gray-300 hover:text-purple-400 transition">Home</a>
                <a href="#news" class="nav-link text-gray-300 hover:text-purple-400 transition">Notícias</a>
                <a href="#reviews" class="nav-link text-gray-300 hover:text-purple-400 transition">Reviews</a>
                <a href="#consoles" class="nav-link text-gray-300 hover:text-purple-400 transition">Consoles</a>
                <a href="#pc" class="nav-link text-gray-300 hover:text-purple-400 transition">PC Gamer</a>
                <a href="#retro" class="nav-link text-gray-300 hover:text-purple-400 transition">Retro</a>
            </nav>
            
            <div class="flex items-center space-x-4">
                <button class="bg-purple-600 hover:bg-purple-700 text-white px-4 py-2 rounded-full transition">
                    Login
                </button>
                <button class="md:hidden text-gray-300">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero-gradient py-20">
        <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <h2 class="text-4xl md:text-5xl font-bold mb-6 text-white">
                    Tudo sobre jogos <span class="text-pink-300">de todas as gerações</span>
                </h2>
                <p class="text-xl text-gray-200 mb-8">
                    Do Atari ao PlayStation 5, do PC master race aos portáteis. Notícias, reviews, guias e muito mais sobre o universo dos games!
                </p>
                <div class="flex space-x-4">
                    <button class="bg-white text-purple-700 px-6 py-3 rounded-full font-bold hover:bg-gray-100 transition pulse">
                        Explorar
                    </button>
                    <button class="border-2 border-white text-white px-6 py-3 rounded-full font-bold hover:bg-white hover:text-purple-700 transition">
                        Assinar Newsletter
                    </button>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <img src="https://images.unsplash.com/photo-1542751371-adc38448a05e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                     alt="Coleção de consoles e controles" 
                     class="rounded-xl shadow-2xl max-w-md w-full">
            </div>
        </div>
    </section>

    <!-- Featured News -->
    <section id="news" class="py-16 bg-gray-800">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center mb-12">
                <h2 class="text-3xl font-bold text-white">
                    <span class="border-b-4 border-purple-500 pb-2">Últimas Notícias</span>
                </h2>
                <a href="#" class="text-purple-400 hover:text-purple-300 flex items-center">
                    Ver todas <i class="fas fa-arrow-right ml-2"></i>
                </a>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- News Card 1 -->
                <div class="bg-gray-700 rounded-xl overflow-hidden shadow-lg game-card">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1598550476439-6847785fcea6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                             alt="Novo jogo anunciado" 
                             class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-purple-600 text-white px-3 py-1 rounded-full text-sm font-bold">
                            Exclusivo
                        </span>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-gray-400 text-sm">15 Jun 2023</span>
                            <span class="text-yellow-400 text-sm">
                                <i class="fas fa-star"></i> 4.8
                            </span>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-white">Novo RPG da FromSoftware anunciado para 2024</h3>
                        <p class="text-gray-300 mb-4">A desenvolvedora de Elden Ring revela novo título com foco em narrativa e combate inovador.</p>
                        <a href="#" class="text-purple-400 hover:text-purple-300 font-medium flex items-center">
                            Ler mais <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- News Card 2 -->
                <div class="bg-gray-700 rounded-xl overflow-hidden shadow-lg game-card">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1542751371-adc38448a05e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                             alt="Lançamento de console" 
                             class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-pink-600 text-white px-3 py-1 rounded-full text-sm font-bold">
                            Hardware
                        </span>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-gray-400 text-sm">10 Jun 2023</span>
                            <span class="text-yellow-400 text-sm">
                                <i class="fas fa-star"></i> 4.5
                            </span>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-white">Nintendo Switch 2: vazamentos sugerem lançamento em 2024</h3>
                        <p class="text-gray-300 mb-4">Novos rumores indicam que o sucessor do Switch pode ter hardware comparável ao PS4 Pro.</p>
                        <a href="#" class="text-purple-400 hover:text-purple-300 font-medium flex items-center">
                            Ler mais <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
                
                <!-- News Card 3 -->
                <div class="bg-gray-700 rounded-xl overflow-hidden shadow-lg game-card">
                    <div class="relative">
                        <img src="https://images.unsplash.com/photo-1585771724684-38269d6639fd?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" 
                             alt="Jogo indie premiado" 
                             class="w-full h-48 object-cover">
                        <span class="absolute top-4 left-4 bg-green-600 text-white px-3 py-1 rounded-full text-sm font-bold">
                            Indie
                        </span>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-2">
                            <span class="text-gray-400 text-sm">5 Jun 2023</span>
                            <span class="text-yellow-400 text-sm">
                                <i class="fas fa-star"></i> 5.0
                            </span>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-white">Jogo indie brasileiro ganha prêmio internacional</h3>
                        <p class="text-gray-300 mb-4">"A Lenda do Saci" conquista prêmio de melhor narrativa no Independent Games Festival.</p>
                        <a href="#" class="text-purple-400 hover:text-purple-300 font-medium flex items-center">
                            Ler mais <i class="fas fa-arrow-right ml-2"></i>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Console Generations -->
    <section id="consoles" class="py-16 bg-gray-900">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-white mb-12 text-center">
                <span class="border-b-4 border-purple-500 pb-2">Gerações de Consoles</span>
            </h2>
            
            <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-6">
                <!-- Console 1 -->
                <div class="bg-gray-800 rounded-lg p-6 text-center hover:bg-gray-700 transition cursor-pointer">
                    <div class="console-icon mb-4 text-4xl text-blue-400">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3 class="font-bold text-white">Atari</h3>
                    <p class="text-gray-400 text-sm">1ª Geração</p>
                </div>
                
                <!-- Console 2 -->
                <div class="bg-gray-800 rounded-lg p-6 text-center hover:bg-gray-700 transition cursor-pointer">
                    <div class="console-icon mb-4 text-4xl text-red-400">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3 class="font-bold text-white">NES</h3>
                    <p class="text-gray-400 text-sm">3ª Geração</p>
                </div>
                
                <!-- Console 3 -->
                <div class="bg-gray-800 rounded-lg p-6 text-center hover:bg-gray-700 transition cursor-pointer">
                    <div class="console-icon mb-4 text-4xl text-green-400">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3 class="font-bold text-white">SNES</h3>
                    <p class="text-gray-400 text-sm">4ª Geração</p>
                </div>
                
                <!-- Console 4 -->
                <div class="bg-gray-800 rounded-lg p-6 text-center hover:bg-gray-700 transition cursor-pointer">
                    <div class="console-icon mb-4 text-4xl text-purple-400">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3 class="font-bold text-white">PlayStation</h3>
                    <p class="text-gray-400 text-sm">5ª Geração</p>
                </div>
                
                <!-- Console 5 -->
                <div class="bg-gray-800 rounded-lg p-6 text-center hover:bg-gray-700 transition cursor-pointer">
                    <div class="console-icon mb-4 text-4xl text-yellow-400">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3 class="font-bold text-white">Xbox 360</h3>
                    <p class="text-gray-400 text-sm">7ª Geração</p>
                </div>
                
                <!-- Console 6 -->
                <div class="bg-gray-800 rounded-lg p-6 text-center hover:bg-gray-700 transition cursor-pointer">
                    <div class="console-icon mb-4 text-4xl text-pink-400">
                        <i class="fas fa-gamepad"></i>
                    </div>
                    <h3 class="font-bold text-white">PS5</h3>
                    <p class="text-gray-400 text-sm">9ª Geração</p>
                </div>
            </div>
        </div>
    </section>

    <!-- PC Gaming Section -->
    <section id="pc" class="py-16 bg-gray-800">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-10">
                    <h2 class="text-3xl font-bold text-white mb-6">
                        <span class="border-b-4 border-purple-500 pb-2">PC Gamer</span>
                    </h2>
                    <p class="text-gray-300 mb-6">
                        Tudo sobre o mundo do PC gaming: benchmarks, hardware, otimizações, e as melhores configurações para rodar os jogos mais pesados.
                    </p>
                    <div class="grid grid-cols-2 gap-4 mb-8">
                        <div class="bg-gray-700 p-4 rounded-lg">
                            <h4 class="font-bold text-purple-400 mb-2">RTX 4090</h4>
                            <p class="text-gray-300 text-sm">Análise da nova placa da NVIDIA</p>
                        </div>
                        <div class="bg-gray-700 p-4 rounded-lg">
                            <h4 class="font-bold text-purple-400 mb-2">AMD Ryzen 9</h4>
                            <p class="text-gray-300 text-sm">Processadores para jogos</p>
                        </div>
                    </div>
                    <button class="bg-purple-600 hover:bg-purple-700 text-white px-6 py-3 rounded-full font-bold transition">
                        Ver Guias de Hardware
                    </button>
                </div>
                <div class="md:w-1/2">
                    <img src="https://images.unsplash.com/photo-1593508512255-86ab42a8e620?ixlib=rb-
</html>
